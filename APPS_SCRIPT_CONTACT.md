# GitJL Contact — V4.8

V4.8 adds email attachments.

Replace the complete Apps Script `Code.gs` with the supplied
`GitJL_Contact_v4_8_Code.gs`.

Then update the EXISTING web-app deployment:

1. Save `Code.gs`.
2. Deploy -> Manage deployments.
3. Select the current Web app.
4. Edit (pencil).
5. Version -> New version.
6. Description: `GitJL Contact v4.8 - attachments`.
7. Keep:
   - Execute as: Me
   - Who has access: Anyone
8. Deploy.

Update the existing deployment rather than creating a new one so the `/exec` URL
used by the website remains unchanged.

## Private recipient

`CONTACT_EMAIL` remains only in:
Project Settings -> Script Properties.

Do not put the recipient address into GitHub.

## Attachments

The website accepts PDF, DOC and DOCX.

Student supervision:
- CV — required
- academic transcript — required
- motivation letter — required

Other contact reasons:
- one optional document

Limits enforced by both browser and Apps Script:
- 5 MB per file
- 15 MB combined

Apps Script reconstructs the Base64 data as Blob objects and sends them directly
with MailApp. The website does not store the files.
