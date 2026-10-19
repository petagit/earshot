# Hookova integration

This fork preserves Earshot by Leon Lin and its MIT license.

The hosted bank lives at https://www.hookova.com/sound-effects/earshot.
It contains 201 default MP3 renders, searchable tags, cue kinds, audio audit
results, source-WAV sync points, and credits for fitted CC0 recordings.

- Catalog: https://www.hookova.com/api/earshot?all=1
- Search: https://www.hookova.com/api/earshot?q=whoosh&clean=1
- MCP download: https://www.hookova.com/hookova-sfx-mcp.zip
- MCP setup: https://www.hookova.com/guides/video-sound-effects

In the Hookova sound-effects MCP 1.2.0+, use `library: "earshot"` with
`search_sounds`, `list_sounds`, or `list_groups`. Use the returned `earshot-...`
ID with the get/download tools. Resources: `hookova://sound-libraries` and
`hookova://earshot/catalog`. Existing meme/reaction sounds remain separate.

The website serves ready-made sounds. This fork provides the full local tools:
install as described in README.md, then use `earshot sfx render`, `earshot kit`,
or the Earshot MCP for custom sounds and audio analysis. Web results include
`bankId` and `knobs` for that local renderer. Sync times describe the original
WAV; MP3 decoder timing can differ.

Hookova import/export code and the pinned upstream revision are maintained in
https://github.com/petagit/hookova-code/blob/main/hooklab/EARSHOT.md.
No private reference recordings or model weights are copied into the website.
