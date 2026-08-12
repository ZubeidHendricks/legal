# Hendricks Arcade — policies

Public mirror of the privacy policy and data deletion instructions for
**Flux Runner**, **Ember Forge** and **Hyper Olympic Clicker**.

This repository exists only to give those two documents public URLs. Facebook
blocks publishing an Instant Game until both are reachable, and GitHub Pages
needs a public repository on a free account — so the pages live here rather
than in the game repository, which stays private.

Served at:

- <https://zubeidhendricks.github.io/legal/privacy.html>
- <https://zubeidhendricks.github.io/legal/data-deletion.html>

## Keeping it in step

The source of truth is `docs/` in the private game repository. These files are
copies. When either page changes there, copy it here and push, or the two will
drift and the version Meta reads will be the stale one:

```sh
cp "<game repo>/docs/privacy.html" "<game repo>/docs/data-deletion.html" .
git commit -am "Sync policy pages" && git push
```

The compliance documents under `docs/dpa/` are deliberately **not** mirrored —
they are working papers for Meta's Data Protection Assessment, not published
pages.
