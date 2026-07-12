# Tapestry Acres — Meet the Herd (public mirror)

Read-only public mirror of the Meet the Herd app, embedded in the
[Down the Farm Lane](https://trashpanda62.github.io/tapestry-game/) journey site.
Guests browse the herd and take the quiz here.

Naming, photo-filing, and other admin happen in the **live app** on the farm
tailnet (`vault_animal_api.py`), which writes straight to the vault. This mirror
ships a static `herd.json` and auto-detects the missing daemon (`/healthz` 404s)
to run in read-only mode.

Refresh this mirror with `scripts/animal-app/deploy-mirror.ps1` in the vault.
Do not hand-edit — it is overwritten on each deploy.
