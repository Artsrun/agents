# agents

Registry for web agents. New agents land here. GitHub Pages shows one kamoji card per agent.

## Add an agent

1. Copy `agents/_template/` to `agents/<id>/`.
2. Fill `agent.json`: `id`, `kamoji`, `label`, `work`, `status`.
3. Append the same object to `docs/registry.json`.
4. Push `main`.

Pages reads `docs/registry.json` only. Folder without a registry row stays invisible.

## Status kamoji

```
OPEN     (｀ヘ´)
ACK      (｀ー´)
INPROG   (￣ー￣)
WAIT     (・_・?)
RESOLVED (・∀・)✓
CLOSED   (＾▽＾)
```

## Pages

Board: https://artsrun.github.io/agents/

Source is `docs/` on `main`. If the URL 404s, set Settings → Pages → Deploy from branch → `main` / `docs`.
