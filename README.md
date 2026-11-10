# My Budget Tracker

A simple budget tracker page built with plain HTML and CSS. This week's update focuses entirely on visual design: the HTML structure is unchanged, and CSS turns the page into a clean, card-based interface.

## Files

- `index.html`: the page structure (heading with logo, how-to details, Add Expense form, expense table, YouTube video).
- `style.css`: all styling.
- `logo.svg`: the logo shown in the page heading.
- `README.md`: this file.

## What Each Part Does

### 1. Color Palette
An emerald green palette, defined once as CSS variables in `:root` and reused everywhere.

| Color | Hex | Used for |
|---|---|---|
| Emerald | `#047857` | Headings, labels, buttons, table header |
| Dark emerald | `#065f46` | Button hover |
| Bright green | `#10b981` | Heading underlines, focus glow |
| Mint | `#ecfdf5` | Page background, alternating table rows |
| Light green | `#6ee7b7` | Borders |
| White | `#ffffff` | Card backgrounds |

### 2. Typography
Fonts are loaded from Google Fonts with `@import` at the top of `style.css`.

- **Poppins**: page heading, section headings, the details summary and table headers.
- **Inter**: body text, labels, form inputs, buttons and table content.

### 3. Form and Table Styling
- Inputs and the dropdown have padding, rounded borders and a green focus glow.
- The button has one consistent style with a darker hover color.
- The table has an emerald header, bordered cells with padding, alternating row colors, a hover highlight and right-aligned amounts.

### 4. CSS Box Model
- **Margin** separates each card from the next.
- **Padding** creates space inside cards, cells and inputs.
- **Border** defines each card, the table and its cells.
- **Border-radius** softens cards, inputs, buttons and the video.
- The page heading, Add Expense form and Expense table each appear as a distinct card. The details box and video use the same card style.

### 5. Advanced Selectors (from Week 2)
Descendant, direct child, `:last-child`, `:not()` and `:focus` selectors are kept and now use the palette.

## How to Run
Open `index.html` in a browser, or use Live Server in VS Code.