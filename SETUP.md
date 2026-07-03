# CPAC HSA site — setup notes

This site is plain HTML pages hosted for free on GitHub Pages. The pages themselves you edit directly (ask whoever set this up, or learn basic HTML — it's just text). The **shared data** (minutes, actions, money, polls) lives in Google Sheets/Forms so all officers can update it without touching code.

## One-time setup (~15 min)

1. **Create a Google Sheet** called `CPAC HSA — Finance & Actions` with tabs: `Social`, `Finance`, `Section 3`, `Section 4`. Each tab gets the Action/Owner/Due/Status columns (Actions) or Date/Description/In/Out/Balance columns (Finance).
2. **Share it** with all officers as Editor.
3. **Embed a tab on its matching page:** open the Sheet → File → Share → Publish to web → choose the tab → Embed → copy the `<iframe>` code → paste it into the matching `.html` file where you see the dashed "Shared Google Sheet embed goes here" box.
4. **Create the first poll:** Google Forms → Blank form → title "Stray cats and dogs" → add the five options already listed on `poll.html`. Then Send → Embed (`<>`) → copy the `<iframe>` code → paste into `poll.html` in place of its dashed box.
5. **Rename Section 3 / Section 4** — open those two `.html` files, replace "Section 3" / "Section 4" with the real names, and update the links in every page's nav bar (find-and-replace across all files).

## Editing minutes / plans

The Minutes and Plans text is written straight into each page's HTML for now (easy to read, no extra tool). Whoever runs the meeting edits the relevant `.html` file after each meeting and pushes the change — or ask to have this swapped for an embedded Doc if you want it self-editable by everyone without touching code.

## Pin it in Messenger

- **Group chat:** send `https://paulhopcraft-dot.github.io/cpac-hsa/` as a message → tap and hold it → **Pin**.
- **Facebook Page:** post the link → open the post's **⋯** menu → **Pin to top of Page**.
