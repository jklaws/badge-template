# badge-template

A starter for your **GitHub Universe badge** repo. Your badge reads its agenda
(and, later, other capabilities) from a repo named **`badge`** in your account.

> **Heads up: your agenda is public.** This repo is public so your badge can read
> it with no login or token. That also means anyone who knows your GitHub username
> can see your schedule. Keep it to things you're fine sharing, and leave out
> anything private (home address, private meeting spots, and so on).

## Set it up (one tap)

1. Click **Use this template ▸ Create a new repository** (top of this page), or
   open **https://github.com/jklaws/badge-template/generate**
2. Name the new repo exactly **`badge`** and create it.
3. On your badge, open the **Agenda** app and hold **A+C** (or press **B**) to sync.

That's it — no token, no install. The badge only *reads* your public repo.

## Editing your agenda

Edit **`agenda/agenda.json`**:

```json
{
  "event": "My Universe '26",
  "year": 2026,
  "days": [
    { "title": "OCT 28 - DAY 1", "date": "2026-10-28", "sessions": [
      { "start": "09:00", "end": null,    "title": "Keynote",  "subtitle": "Main Stage" },
      { "start": "10:30", "end": "12:00", "title": "Workshop", "subtitle": "Hall A" }
    ]}
  ]
}
```

- `start` / `end` are `"HH:MM"` (24h); `end` may be `null` for open-ended items.
- `date` is `"YYYY-MM-DD"` — the badge highlights the session happening **now**
  and counts down to the event.
- Hold **A+C** (or press **B**) in the Agenda app to pull your latest changes.

## Folder layout

| Folder | Used by | What it is |
|--------|---------|------------|
| `agenda/` | Agenda app | `agenda.json` — your schedule |

More folders show up here as the badge gains capabilities.
