Read `AGENTS.md`, `VAULT_INDEX.md`, and `vault_manifest.json` first.

You are working inside this Obsidian knowledge vault repository:
https://github.com/senthilnathan01/knowledge-vault

Your input is an already-prepared high-fidelity source summary from a YouTube video.

Use this input:
<PASTE_SOURCE_PACKET_OR_FULL_SUMMARY>

Your task:
Integrate this source into the vault cleanly and without duplication.

Instructions:
1. Create a detailed source note under `sources/youtube/`
2. Use the source summary to extract:
   - main thesis
   - nuanced insights
   - memorable examples
   - actionable ideas
   - important terms / frameworks
   - open questions if useful
3. Search for relevant existing notes in `concepts/` and `projects/`
4. Prefer updating existing relevant notes over creating duplicate notes
5. Create new evergreen notes only if no existing note is a good destination
6. Add Obsidian wikilinks between the source note and related notes
7. Preserve readability and stable note titles
8. Do not rewrite unrelated sections
9. Update `VAULT_INDEX.md` if any note is created, renamed, or materially changed
10. Update `vault_manifest.json` if any note is created, renamed, or materially changed
11. Keep edits high-signal, structured, and concise
12. Add a short `## Sources` section where appropriate for notes derived from this material
13. Avoid duplication across source notes, concept notes, and project notes

When creating the YouTube source note:
- Make the note detailed enough that I do not need to rewatch the video for the main ideas
- Preserve nuance and tradeoffs
- Include sections such as:
  - Summary
  - Main Thesis
  - Key Insights
  - Examples
  - Actionable Ideas
  - Related Concepts
  - Sources

When updating existing notes:
- Merge only genuinely relevant insights
- Do not force weak connections
- Prefer small, precise additions over bloated rewrites

At the end, output exactly:
- files created
- files updated
- what changed in each file
- why each change was made
- any possible duplicates or ambiguities noticed