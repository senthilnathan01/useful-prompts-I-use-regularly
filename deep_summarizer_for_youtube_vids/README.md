This prompt set is for turning a YouTube video into a high-fidelity knowledge capture and then integrating it into an Obsidian-style vault.

## Files

- `summary_generation_prompt.md`
  Use in ChatGPT or Claude after pasting:
  1. the YouTube link
  2. the transcript or detailed notes
- `vault_update_prompt.md`
  Use in Codex after you have a prepared summary or the generated `SOURCE_PACKET`. This updates the target vault repo.

## Placeholders to replace

Replace prompt placeholders before use:

- `<PASTE_LINK>`
- `<PASTE_TRANSCRIPT_OR_NOTES>`
- `<PASTE_SOURCE_PACKET_OR_FULL_SUMMARY>`

## Recommended workflow

1. Get the YouTube link and the transcript or detailed notes.
2. In ChatGPT or Claude, paste the link, transcript or notes, and `summary_generation_prompt.md`.
3. Save the resulting full summary or at least the `SOURCE_PACKET`.
4. Open Codex in the target knowledge vault repository.
5. Paste `vault_update_prompt.md` and include the prepared summary or `SOURCE_PACKET`.
6. Let Codex create or update the YouTube source note and any relevant related notes.

## Usage notes

- This flow is intentionally split into summary generation and repository update steps.
- The first prompt is designed to preserve nuance, caveats, examples, and implementation-relevant detail.
- The second prompt is designed to avoid duplicate notes and prefer precise updates to existing notes.
- The `SOURCE_PACKET` is the handoff format between the two steps.
