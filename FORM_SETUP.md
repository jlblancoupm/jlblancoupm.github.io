# Supervision form setup (Formspree)

The public site contains **no recipient email address**.

## 1. Create the Formspree form

Create a form in Formspree and configure its notification recipient in the Formspree dashboard.

Copy the form ID from the endpoint:

    https://formspree.io/f/YOUR_FORM_ID

Then edit:

    _data/contact.yml

and replace:

    form_id: REPLACE_WITH_FORMSPREE_FORM_ID

with your actual form ID.

The form ID is public by design. The recipient email is not.

## 2. Configure the automatic reply

In the Formspree dashboard, add an **Auto Response** action.

Suggested values:

From name:
    José Luis Blanco Murillo / GAPS-UPM

Subject:
    Your supervision enquiry has been received

Message:
    Thank you for contacting José Luis Blanco Murillo / GAPS-UPM regarding student supervision.
    Your enquiry has been received and will be reviewed.
    A response will be sent if the proposed topic and profile are a suitable match.

The HTML form has an input named `email`, which Formspree uses for the response recipient.

## 3. File uploads

The form requests:
- updated CV
- academic transcript / marks
- motivation letter

Accepted browser file types are PDF, DOC and DOCX.

## 4. Recommended Formspree settings

- Restrict submissions to `jlblancoupm.github.io`
- Keep Formspree spam filtering enabled
- Add server-side validation for required fields and uploaded files
- Consider Turnstile/reCAPTCHA if spam becomes a problem

## Plan note

As of August 2026, Formspree file uploads require Personal, Professional or Business,
while the dashboard Auto Response action requires Professional or Business.
Therefore, the complete workflow used by this site requires Professional or Business
unless the confirmation step is implemented separately.
