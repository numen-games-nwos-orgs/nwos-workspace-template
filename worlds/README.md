# Worlds

The 3D worlds of this organization. One folder per world:

```
worlds/<world-name>/
  mundo.json      the world's card: what it is, who made it, who owns it
  aventura/       what happens in it
  entorno/        how it looks: sky, light, ground
  tools/          the scripts that rebuild the world
  LICENSES.md     the licence of every piece
  CREATORS.md     who made every piece
  PROGRESS.md     what is done, what is left, and the command that rebuilds it
  releases/       the published versions: v1.zip, v2.zip, … and index.json
```

Rules:

- A version is a published zip with its number. A published version is never rewritten: a change is a new number.
- `releases/` keeps the last 10 published versions of each world. Older ones stay in the history of this repository.
- GitHub refuses a file over 100 MB. A zip of up to 50 MB lives in `releases/`; a larger one is attached to a release of this repository, and `releases/vN.json` says where it is, its size and its SHA-256.
- Owner and creator are different fields. The owner is the organization; the creator is whoever built the piece.
- No keys and no people's data: no `.env`, no `claves.env`, no tokens, no user tables.
