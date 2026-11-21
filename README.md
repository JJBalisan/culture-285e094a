# Culture (unlisted)

Weekly spoken guide to the week in London, narrated from the culture digest
by the `weekly-culture-podcast` scheduled task. The repo is public only
because free GitHub Pages needs that; the name is random and the page
carries noindex. Treat the feed URL as a secret.

This repo holds data only: `show.json` (the show's feed settings),
`episodes.json`, `feed.xml`, covers and audio. The task publishes with the
shared kit (`podcast-kit`):
`~/.local/share/threshold-and-bar/bin/publish_episode.py` adds an episode,
and `python3 ~/.local/share/threshold-and-bar/bin/build_feed.py .` rebuilds
`feed.xml` by hand on the Mac. On the Windows PC use the kit's
`venv-mlx/bin/python` wrapper with `PYTHONUTF8=1` set: without it the
rebuild writes cp1252 bytes and CRLF line ends into a feed that declares
UTF-8 (podcast-kit #58).
