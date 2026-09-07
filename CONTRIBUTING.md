# Contributing to Themecord

Thanks for helping grow the snippet collection. Contributions can add a new customisation, fix a broken snippet, or improve its documentation.

## Where changes belong

Add standalone CSS files to `snippets/`. Pride mention/reply highlight palettes belong in `snippets/pride/`. Give each file a descriptive lowercase name with underscores, such as `compact_search_field.css` or `transgender_reply_highlight.css`.

**Do not edit `quickcss.css` when contributing.** It is simply a ready-made template for users who do not wish to put their own theme together using individual snippets. It is not a generated bundle or a catalogue that needs to stay in sync with the collection. New snippets and fixes should go in their individual files.
*(`quickcss.css` is also a backup of my own quickcss build, hehe)*

Check the existing collection before adding a file. If your change fixes an existing snippet, update that snippet rather than creating a duplicate.

## Write a snippet

- Keep each snippet focused on one customisation and usable on its own. Explain any required plugin, setting, or other dependency.
- Target the relevant Discord elements as narrowly as possible so unrelated parts of the interface are unaffected.
- Add a short opening comment describing the snippet, its author, and its source and licence where applicable. Preserve existing attribution and licence notices when adapting someone else's work; do not replace their licence with your own.
- Explain unusual selectors or non-obvious CSS with concise comments. Mention known conflicts or limitations.
- Follow `.editorconfig`: UTF-8, tabs for indentation, CRLF line endings, no trailing whitespace, and a final newline.

For pride highlights, follow the existing files' selectors and gradient styling. Name the flag variant if multiple designs exist, and explain when the gradient represents only a flag's colours rather than its symbols or geometry.

## Try it in Discord

1. Back up your existing custom CSS, then apply the snippet using one of the methods in the [README](README.md).
2. Test it on its own first, with other custom styles disabled, so you can confirm what it changes.
3. Check the affected interface and relevant states, such as hover, selection, expanded panels, mentions, or replies. Check light and dark appearances where applicable, and note any unsupported appearance.
4. Re-enable your usual styles to look for obvious conflicts. Remove the snippet again to confirm its effects can be undone.

Include your patcher, Discord version or release channel, and any required plugins in your contribution notes. If you could not test a behaviour, say so. Before-and-after screenshots are useful for visual changes; remove private messages or personal details from them.

## Update the catalogue

Add your snippet to the appropriate table in [README.md](README.md), with a clear name, a short description where the table includes one, and both links:

- **View code:** `https://github.com/tobezdev/Themecord/blob/main/snippets/your_snippet.css`
- **Raw CSS:** `https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/your_snippet.css`

Use the actual path, including `pride/` for pride snippets. These links will become available on the main repository after your contribution is merged. Update existing catalogue entries if you rename a file or change its behaviour.

## Submit your contribution

1. Fork [Themecord](https://github.com/tobezdev/Themecord) into your GitHub account and create a branch for your change.
2. Add or edit the individual snippet and update the README catalogue. Leave `quickcss.css` unchanged.
3. Commit your changes, push the branch to your fork, and open a pull request against this repository's `main` branch.
4. Describe the problem or visual change, list what you tested, and include screenshots when helpful. Mention dependencies, conflicts, and any source or licence information relevant to the addition.

Keep the pull request focused on the snippet you are adding or fixing. You can also [open an issue](https://github.com/tobezdev/Themecord/issues) to suggest a snippet or report a problem without submitting code.
