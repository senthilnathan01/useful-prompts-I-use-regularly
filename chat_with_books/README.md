This is in reference to https://github.com/senthilnathan01/book-to-vault-lite

# Prompt Templates

These prompts are meant for a simple chapter-wise workflow.

## Files

- `study_prompt.md`  
  Use in ChatGPT or Claude when you paste:
  1. the current per-book global working memory
  2. one chapter markdown file

- `export_prompt.md`  
  Use at the end of the study chat to generate the final chapter export.

- `vault_update_prompt.md`  
  Use in Codex after you save the export file locally. This updates the target vault repo.

## What you need to change

Replace placeholders like these before use:

- `<BOOK_TITLE>`
- `<BOOK_AUTHOR>`
- `<BOOK_SLUG>`
- `<CHAPTER_NUMBER>`
- `<CHAPTER_TITLE>`
- `<CHAPTER_FILE_PATH>`
- `<EXPORT_FILE_PATH>`
- `<TARGET_VAULT_REPO>`
- `<BOOK_FOLDER_PATH>`
- `<GLOBAL_MEMORY_PATH>`
- `<BOOK_INDEX_PATH>`
- `<CHAPTER_NOTE_PATH>`

## Recommended flow

1. Run your PDF parsing script and get chapter markdown files.
2. Open one chapter file.
3. In ChatGPT/Claude, paste:
   - the per-book global working memory
   - the chapter markdown
   - `study_prompt.md`
4. Ask questions until you understand the chapter.
5. Paste `export_prompt.md`.
6. Save the result as a markdown export file.
7. Open Codex and paste `vault_update_prompt.md`.
8. Let Codex update the notes in your vault repo.

## Notes

- Global working memory is per book.
- Keep the working memory compact.
- Keep the chapter export detailed.
- The export file is the bridge between the study chat and the vault.