# Portal Status Indicator

[`status.json`](status.json) is used to communicate current NSW Portal status to the NSW Digital Twin frontend.

If the portal goes down, replace `status.json` with the contents of [`examples/bad.json`](examples/bad.json).
When the portal comes back up replace `status.json` again with [`examples/good.json`](examples/good.json).

Text in `message` and `title` can be freely changed for both portal down and up notifications. A new notification will only be shown if the portal status changes or if a user hasn't yet seen the portal down notification (changing the text of a portal down notice won't re-notify users).
