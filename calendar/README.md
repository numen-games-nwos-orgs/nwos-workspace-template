# Calendar

The gatherings of this organization. One file per gathering:

```
calendar/<YYYY>/<YYYY-MM-DD>-<id>.md
```

Each file opens with these fields, and every time is UTC:

```
---
id: 
title: 
starts: 2027-01-31T18:00:00Z
ends: 2027-01-31T19:30:00Z
all_day: false
mode: online            # in-person | online | mixed
where:                  # the venue or the city, for a gathering in person
world:                  # the 3D world it happens in, if any
recurs:                 # yearly, for a gathering that returns every year
cancelled_at:           # set when it is cancelled; the file stays
note: 
---
```

Rules:

- A cancelled gathering keeps its file: what was announced stays on record.
- No people's data: not who created it, not who is coming.
- The files are written by numinia.com when a gathering is created or changed there. An `.ics` calendar can be made from them.
