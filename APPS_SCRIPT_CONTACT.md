# Apps Script update required for V4.7

Replace only the `result_()` function in `Code.gs` with:

```javascript
function result_(ok, message) {
  const payload = JSON.stringify({
    type: "gitjl-contact",
    ok: ok,
    message: message
  });

  return HtmlService.createHtmlOutput(
    "<!doctype html><html><body>" +
    "<script>" +
    "window.parent.postMessage(" +
    payload +
    ", '*');" +
    "</script>" +
    "</body></html>"
  ).setXFrameOptionsMode(HtmlService.XFrameOptionsMode.ALLOWALL);
}
```

Then:
1. Save the script.
2. Deploy -> Manage deployments.
3. Edit the existing Web app deployment (pencil icon).
4. Select New version.
5. Description: `GitJL Contact v2 - iframe response`.
6. Deploy.

Keep:
- Execute as: Me
- Who has access: Anyone

The existing `/exec` URL should remain the same when the current deployment is updated.

The recipient email remains only in the private Script Property `CONTACT_EMAIL`.
