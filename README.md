# MAS SREAC redirect — hosted pages

Static frontend for the Malaysia Airlines self-reaccommodation redirect on the
Ada sandbox. The AI Agent's handoff fires an event, and these pages rebuild the
Amadeus form and POST it.

- `index.html` / `mas-sreac-redirect_sandbox.html` — the page, with the
  `flight_booking` and self-reac event callbacks.
- `sreac-relay.html` — debug page: logs every `ada:*` event and accepts a payload
  by paste or `#p=<base64url json>`.

Both refuse to POST anywhere outside their `ALLOWED_HOSTS` list.
