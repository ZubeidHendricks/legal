# Hendricks Arcade — policies

Public mirror of the privacy policy, terms of service and data deletion
instructions for **Flux Runner**, **Ember Forge** and **Hyper Olympic Clicker**.

This repository exists only to give those documents public URLs. Facebook blocks
publishing an Instant Game until they are reachable, and GitHub Pages needs a
public repository on a free account — so the pages live here rather than in the
game repository, which stays private.

Served at:

- <https://zubeidhendricks.github.io/legal/privacy.html>
- <https://zubeidhendricks.github.io/legal/terms.html>
- <https://zubeidhendricks.github.io/legal/data-deletion.html>

These URLs are the ones to paste into Meta's Settings → Basic. An earlier set
pointed at a DigitalOcean app that has since been destroyed, which is the exact
failure this repository exists to avoid: GitHub Pages has no instance to lose.

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
