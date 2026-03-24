This prompt set is for a simple chapter-wise book-study workflow that ends in updating a vault repo.

Reference implementation context: [book-to-vault-lite](https://github.com/senthilnathan01/book-to-vault-lite)

## Files

- `study_prompt.md`
  Use in ChatGPT or Claude after pasting:
  1. the current per-book global working memory
  2. one chapter markdown file
- `export_prompt.md`
  Use at the end of the study chat to generate the final chapter export.
- `vault_update_prompt.md`
  Use in Codex after saving the export file locally. This updates the target vault repo.

## Placeholders to replace

Replace prompt placeholders before use. Common values include:

- `<BOOK_TITLE>`
- `<BOOK_AUTHOR>`
- `<BOOK_SLUG>`
- `<CHAPTER_NUMBER>`
- `<CHAPTER_NUMBER_PADDED>`
- `<CHAPTER_TITLE>`
- `<CHAPTER_FILE_PATH>`
- `<EXPORT_FILE_PATH>`
- `<TARGET_VAULT_REPO>`
- `<BOOK_FOLDER_PATH>`
- `<GLOBAL_MEMORY_PATH>`
- `<BOOK_INDEX_PATH>`
- `<CHAPTER_NOTE_PATH>`

## Recommended workflow

1. Generate or collect chapter markdown files for the book.
2. Open the chapter you want to study.
3. In ChatGPT or Claude, paste:
   - the per-book global working memory
   - the chapter markdown
   - `study_prompt.md`
4. Continue the discussion until the chapter is clear.
5. Paste `export_prompt.md` in the same chat.
6. Save the generated markdown as a chapter export file.
7. Open Codex in the target vault repository and paste `vault_update_prompt.md`.
8. Let Codex update the chapter note, book index, and per-book working memory.

## Usage notes

- Global working memory is per book, not repo-wide.
- Keep the working memory compact and continuity-focused.
- Keep the chapter export detailed because it is the source note for the vault update step.
- The export file is the bridge between the study conversation and the vault updates.
