# Useful Prompts I Use Regularly

Reusable prompt templates for a few repeatable knowledge-work flows.

## What is in this repo

- `chat_with_books/`
  Prompt set for studying a book chapter, exporting the chapter notes, and then updating a target Obsidian-style vault.
- `youtube_podcast_depth_extractor.md`
  Prompt for turning a YouTube video or podcast link into a detailed vault source note and related note updates.

## Repo structure

```text
.
├── chat_with_books/
│   ├── README.md
│   ├── export_prompt.md
│   ├── study_prompt.md
│   └── vault_update_prompt.md
└── youtube_podcast_depth_extractor.md
```

## How to use this repo

These files are prompt templates, not executable programs.

Typical workflow:

1. Pick the prompt that matches the task.
2. Replace the placeholder values in the template.
3. Paste the prompt into the target tool, such as ChatGPT, Claude, or Codex.
4. Review the generated output before saving or applying it to your notes repo.

## Prompt inventory

### `chat_with_books/`

This flow is for chapter-wise study and vault updates.

- `study_prompt.md`
  Use in ChatGPT or Claude after pasting the current chapter text and the per-book global working memory.
- `export_prompt.md`
  Use at the end of the study session to generate a detailed markdown chapter note.
- `vault_update_prompt.md`
  Use in Codex after saving the chapter export locally so Codex can update the target vault files.

See [chat_with_books/README.md](chat_with_books/README.md) for the detailed flow.

### `youtube_podcast_depth_extractor.md`

Use this when you want Codex to process a YouTube link inside a knowledge vault repository. The prompt tells Codex to:

- read the vault guidance files first
- create a detailed source note under `sources/youtube/`
- update related concept or project notes when useful
- update the vault index and manifest
- avoid duplicates

## Conventions

- Angle-bracket values like `<BOOK_TITLE>` are placeholders and must be replaced before use.
- Some prompts assume they are run inside another repository, such as an Obsidian vault.
- The prompts are intentionally explicit so the output is easier to audit and reuse.

## Notes

- No dependencies are required for this repo itself.
- If prompt behavior changes, update the relevant README alongside the prompt text.
