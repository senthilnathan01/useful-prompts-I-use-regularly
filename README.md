# Useful Prompts I Use Regularly

Reusable prompt templates for a few repeatable knowledge-work flows.

## What is in this repo

- `chat_with_books/`
  Prompt set for studying a book chapter, exporting the chapter notes, and then updating a target Obsidian-style vault.
- `deep_summarizer_for_youtube_vids/`
  Prompt set for creating a high-fidelity YouTube summary first, then integrating it into a knowledge vault without duplicating notes.

## Repo structure

```text
.
├── README.md
├── chat_with_books/
│   ├── README.md
│   ├── export_prompt.md
│   ├── study_prompt.md
│   └── vault_update_prompt.md
└── deep_summarizer_for_youtube_vids/
    ├── README.md
    ├── summary_generation_prompt.md
    └── vault_update_prompt.md
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

### `deep_summarizer_for_youtube_vids/`

This flow splits YouTube capture into two steps so the summary quality and the vault update step stay separate.

- `summary_generation_prompt.md`
  Use in ChatGPT or Claude after pasting the YouTube link and a transcript or detailed notes. It generates a dense summary plus a reusable `SOURCE_PACKET`.
- `vault_update_prompt.md`
  Use in Codex inside the target vault repository after pasting the prepared summary or `SOURCE_PACKET`. It updates source notes, related concept or project notes, and the vault index/manifest.

See [deep_summarizer_for_youtube_vids/README.md](deep_summarizer_for_youtube_vids/README.md) for the detailed flow.

## Conventions

- Angle-bracket values like `<BOOK_TITLE>` are placeholders and must be replaced before use.
- Some prompts assume they are run inside another repository, such as an Obsidian vault.
- The prompts are intentionally explicit so the output is easier to audit and reuse.

## Notes

- No dependencies are required for this repo itself.
- If prompt behavior changes, update the relevant README alongside the prompt text.
