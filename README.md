# Themecord

A collection of CSS customisations for Discord: compact controls, layout tweaks, cleaner panels, and pride-coloured mention and reply highlights.

CSS controls how Discord looks. A **snippet** is a small piece of CSS that changes a particular part of the interface. These changes appear in your own client; they do not change how other people see Discord.

[Browse the project](https://github.com/tobezdev/Themecord) · [Report an issue](https://github.com/tobezdev/Themecord/issues)

## Contents

- [Start here](#start-here)
- [Choose what to install](#choose-what-to-install)
- [Copy and paste the CSS](#option-1-copy-and-paste-the-css)
- [Add a URL to Vencord Online Themes](#option-2-add-a-url-to-vencord-online-themes)
- [Interface snippets](#interface-snippets)
- [Pride highlights](#pride-highlights)
- [Change, remove, or troubleshoot a style](#change-remove-or-troubleshoot-a-style)
- [Credits and contributions](#credits-and-contributions)

## Start here

Discord does not include a custom CSS editor by default. You first need a **client modification**, sometimes called a **patcher**, such as Vencord or BetterDiscord. It adds settings that let you apply custom styles.

1. Choose a patcher and follow its official installation instructions for your operating system:
   - **Vencord:** [Download and installation instructions](https://vencord.dev/download/) · [Help and troubleshooting](https://vencord.dev/faq/).
   - **BetterDiscord:** [Installation guide](https://docs.betterdiscord.app/users/getting-started/installation) · [Documentation](https://docs.betterdiscord.app/).
2. Restart Discord after installation, then open **User Settings** using the cog near your profile at the bottom left.
3. Look for the section added by your patcher. This is where you will find its CSS or theme settings.

These instructions are for desktop Discord. For Vencord in a desktop browser, follow its browser-extension instructions; its userscript build does not support custom themes. See the [Vencord download page](https://vencord.dev/download/) for supported options.

You do not need Git, a GitHub account, or a code editor to use these files.

## Choose what to install

| Option | What you get | Links |
| --- | --- | --- |
| Combined stylesheet | `quickcss.css`: a ready-made collection of interface tweaks, including rainbow highlights | [View code](https://github.com/tobezdev/Themecord/blob/main/quickcss.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/quickcss.css) |
| Individual snippets | Pick only the changes you want from the catalogue below | [Browse snippets](https://github.com/tobezdev/Themecord/tree/main/snippets) |
| Pride highlights | Choose a colour palette for messages that mention you and messages you are replying to | [Browse pride snippets](https://github.com/tobezdev/Themecord/tree/main/snippets/pride) |

Start with either the combined stylesheet or a selection of individual snippets. The combined file already includes many of the snippets, so you do not need to add those again. It is a separate file, not an automatic import of everything in the snippets folder.

## Option 1: Copy and paste the CSS

This works with patchers that provide a QuickCSS or Custom CSS editor.

1. Open **Raw CSS** for the file you want in the tables below. You should see plain CSS text.
2. Select and copy the entire file (`Ctrl+A`, then `Ctrl+C` on Windows/Linux; `Cmd+A`, then `Cmd+C` on macOS).
3. In Discord's **User Settings**, open your patcher's CSS editor:
   - **Vencord:** find **Open QuickCSS File** in the Vencord settings and enable **Enable Custom CSS** if it is off.
   - **BetterDiscord:** open **Custom CSS** in the BetterDiscord settings.
4. Paste the CSS into the editor. If you already have custom CSS, keep a backup and append the new code below it.
5. Save the file or use your editor's **Save/Apply** controls if shown, then return to Discord to see the change.

Copy the CSS contents, not the URL. To add another snippet, paste it below the previous one. Pasted CSS is a local copy: to receive future changes, replace it with a fresh copy from this repository.

## Option 2: Add a URL to Vencord Online Themes

Vencord can load a CSS file directly from a web address.

1. Open **User Settings → Vencord → Themes → Online Themes**.
2. Paste the raw CSS URL for your chosen file into the theme-links field, with **one URL per line**.
3. Save or apply if prompted, then return to Discord. If it does not update immediately, reload Discord.

For the combined stylesheet, copy this URL:

```text
https://raw.githubusercontent.com/tobezdev/Themecord/main/quickcss.css
```

For just the transgender highlight, for example, use:

```text
https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/transgender_reply_highlight.css
```

The [GitHub file page](https://github.com/tobezdev/Themecord/blob/main/quickcss.css) is for browsing code. Its **Raw** button opens the plain CSS address used above. In the tables, copy the destination of **Raw CSS** using your browser's **Copy link address** option.

Online links follow the version on `main` when your patcher fetches them again; updates may require a reload and can be delayed by caching. If your patcher does not have Online Themes, use the copy-and-paste method or consult its own theme guide. Menu names can differ between patchers and versions.

## Interface snippets

Choose any combination that suits you. Add one at a time so you can see what each changes.

| Snippet | Purpose | Links |
| --- | --- | --- |
| Collapse icon position | Adjusts the position of collapse icons. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/collapse_icon_position_fix.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/collapse_icon_position_fix.css) |
| Compact buttons | Reduces button spacing and sizing. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/compact_buttons.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/compact_buttons.css) |
| Compact command picker | Adjusts the size of the slash-command picker. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/compact_command_picker.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/compact_command_picker.css) |
| Compact search field | Makes the search field more compact. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/compact_search_field.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/compact_search_field.css) |
| Server list clearance | Keeps the user panel from covering the server list. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/dont_cover_server_list_with_panel.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/dont_cover_server_list_with_panel.css) |
| Expanded message timestamp | Restyles and expands edited-message timestamps. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/expanded_message_timestamp.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/expanded_message_timestamp.css) |
| Hide activity status | Hides activity-status elements. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/hide_activity_status.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/hide_activity_status.css) |
| Icon consistency | Restyles icons, including icons used by some plugins. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/icon_consistency.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/icon_consistency.css) |
| Mention/reply gradient | Adds an alternative gradient treatment for mentions and replies. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/mention_reply_gradient_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/mention_reply_gradient_highlight.css) |
| Profile button placement | Moves profile buttons to the top right. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/move_profile_buttons_top_right.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/move_profile_buttons_top_right.css) |
| Page switcher styling | Restyles page-switching controls. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/page_swapper_refresh.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/page_swapper_refresh.css) |
| Server list top gap | Removes the gap at the top of the server list. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/remove_gap_top_server_list.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/remove_gap_top_server_list.css) |
| Hide gift button | Hides the Nitro gift button. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/remove_nitro_gift_button.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/remove_nitro_gift_button.css) |
| Round server icons | Makes server icons round. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/round_server_icons.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/round_server_icons.css) |
| Settings modal | Displays settings in a modal-style layout. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/settings_modal.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/settings_modal.css) |
| User and activity panels | Restyles the user and activity panels. | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/user_activity_panels_redesign.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/user_activity_panels_redesign.css) |

## Pride highlights

Each file applies the same soft-gradient style to mentions and replies, including hover and selected states: a translucent background and an opaque coloured bar.

**Use one pride palette at a time.** These files target the same elements, so multiple palettes compete with each other. They also overlap with the separate mention/reply gradient snippet.

If you copied `quickcss.css`, paste your chosen pride snippet **after the combined CSS** to override its rainbow colours. For Online Themes, put the combined stylesheet first and the pride URL below it. If another theme or your existing QuickCSS overrides the result, remove its competing highlight rules or use individual snippets instead.

| Palette | Links |
| --- | --- |
| Abrosexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/abrosexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/abrosexual_reply_highlight.css) |
| Agender | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/agender_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/agender_reply_highlight.css) |
| Aroace (sunset) | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/aroace_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/aroace_reply_highlight.css) |
| Aromantic | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/aromantic_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/aromantic_reply_highlight.css) |
| Asexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/asexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/asexual_reply_highlight.css) |
| Bigender (pink/lavender/blue) | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/bigender_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/bigender_reply_highlight.css) |
| Bisexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/bisexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/bisexual_reply_highlight.css) |
| Demiboy | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/demiboy_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/demiboy_reply_highlight.css) |
| Demigirl | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/demigirl_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/demigirl_reply_highlight.css) |
| Demiromantic | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/demiromantic_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/demiromantic_reply_highlight.css) |
| Demisexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/demisexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/demisexual_reply_highlight.css) |
| Gay (seven-stripe) | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/gay_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/gay_reply_highlight.css) |
| Genderfluid | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/genderfluid_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/genderfluid_reply_highlight.css) |
| Genderqueer | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/genderqueer_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/genderqueer_reply_highlight.css) |
| Intersex | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/intersex_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/intersex_reply_highlight.css) |
| Lesbian (seven-stripe sunset) | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/lesbian_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/lesbian_reply_highlight.css) |
| Nonbinary | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/nonbinary_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/nonbinary_reply_highlight.css) |
| Omnisexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/omnisexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/omnisexual_reply_highlight.css) |
| Pangender | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/pangender_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/pangender_reply_highlight.css) |
| Pansexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/pansexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/pansexual_reply_highlight.css) |
| Philadelphia | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/philadelphia_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/philadelphia_reply_highlight.css) |
| Polysexual | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/polysexual_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/polysexual_reply_highlight.css) |
| Rainbow (original) | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/pride_rainbow_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/pride_rainbow_reply_highlight.css) |
| Progress | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/progress_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/progress_reply_highlight.css) |
| Transgender | [View code](https://github.com/tobezdev/Themecord/blob/main/snippets/pride/transgender_reply_highlight.css) · [Raw CSS](https://raw.githubusercontent.com/tobezdev/Themecord/main/snippets/pride/transgender_reply_highlight.css) |

This collection covers a selection of pride flags and design variants. Intersex, demisexual, demiromantic, and Progress highlights use flag colours in a linear gradient rather than reproducing their circles, triangles, or chevrons. For background on the flags, see the [UBC guide to pride flags](https://equity.ubc.ca/pride-flags/).

## Change, remove, or troubleshoot a style

- **Remove pasted CSS:** delete the snippet you added from QuickCSS/Custom CSS, then save or apply.
- **Remove an online theme:** delete its URL from Online Themes, then save or reload as needed.
- **Nothing changes:** check that custom CSS is enabled, that you copied the entire file or used a raw URL, and that the relevant interface is visible. A reply highlight only appears while you are replying to a message.
- **A raw link returns 404:** check the filename and make sure the file exists on this repository's `main` branch. Files added locally are available online only after they are pushed.
- **Styles clash:** temporarily disable other themes and snippets, then re-enable them one at a time. Some snippets change the same controls, so combinations may need adjustments.
- **A Discord update breaks a snippet:** Discord can change the class names and layout these styles depend on. Check for an updated file or [open an issue](https://github.com/tobezdev/Themecord/issues) with the snippet name, your patcher, and a description or screenshot of the problem.

For installation problems or missing patcher settings, use your patcher's help resources linked above. Compatibility can vary by Discord version, patcher, enabled plugins, and other themes.

## Credits and contributions

Themecord brings together custom styles and community snippets. Many CSS files include the original author's name, source link, and licence in their opening comments. Keep those credits when sharing or adapting the code; licence terms vary by snippet, including CC0 and GPL-2.0 notices. See [LICENSE](LICENSE) for the repository’s default terms: code without a separate applicable licence may be used freely for noncommercial purposes; commercial or money-making use is excluded. Existing snippet licences take precedence.

Suggestions, fixes, and additional palettes are welcome through [issues](https://github.com/tobezdev/Themecord/issues) or [pull requests](https://github.com/tobezdev/Themecord/pulls). Keep snippets focused, preserve attribution, and describe which part of Discord your change affects.

See the [contribution guide](CONTRIBUTING.md) for adding and testing snippets. Contributors should leave `quickcss.css` unchanged: it is a ready-made template for users who do not want to assemble their own theme from the collection.
