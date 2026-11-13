# AGENTS.md
Personal repository with all kind of information on builds for the games Path Of Exile and Path Of Exile 2.The
repository is organized in [OKF - Open Knowledge Format](https://okf.md/) and uses Claude Code to organize the
information. Knowledge is stored as plain markdown, one concept per file.

## Structure
- `docs`: The Obsidian knowledge vault.
  - `poe1`: All concepts related to Path Of Exile 1. One concept per file.
    - `index.md`: The index as per the OKF specification.
    - `log.md`: Reserved OKF file. Chronological capture and changes.
  - `poe2`: All concepts related to Path Of Exile 2. One concept per file.
    - `index.md`: The index as per the OKF specification.
    - `log.md`: Reserved OKF file. Chronological capture and changes.

## Frontmatter for new concepts/notes
- Every new concept/note in `docs` starts with YAML frontmatter: Required field: type. Recommended: title, description,
  tags, timestamp. Optional: resource (a source link). You may add your own keys such as status.

## File naming for new concepts/notes
- Use descriptive kebab-case filenames for every new concept/note in `docs`, regardless of folder, for example
  `leage-start-prep.md`.

## Writing a concept/note in `docs`
- Write a short plain-language definition first, then detail
- Link related concepts/notes inline with standard markdown links, for example [[embeddings]]
- Never invent facts. If unsure, add status: draft
- Use plain punctuation, no em dashes

## Maintenance rules
- When you add a concept/note, add a link to it from any related concept/note.
- When you add, rename or remove a concept/note, update the `index.md` in the same folder. Create the `index.md` if
  it does not exist. Each entry is a bullet link with the note's frontmatter description, for example
  `* [Title](file-name.md) - Description`. Index files have no frontmatter.
- Prefer editing an existing concept/note over creating a duplicate.
- If you are unsure whether two concepts/notes are the same, ask the user.
