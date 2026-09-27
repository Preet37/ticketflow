# TicketFlow

A tiny single-file Flask helpdesk: list tickets, download attachments, preview
linked URLs, and run a quick network diagnostic.

## Run

```bash
pip install -r requirements.txt
python app.py          # http://127.0.0.1:5001  (or $PORT)
```

## Routes
- `GET /tickets` — list tickets
- `GET /attachments?file=welcome.txt` — download an attachment
- `GET /link-preview?url=...` — server-side preview of a link
- `GET /tools/ping?host=...` — network reachability check

> Demo app — not production-hardened. Do not deploy publicly.
