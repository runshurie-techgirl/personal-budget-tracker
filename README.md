# My Budget Tracker (Week 2)

A budget tracker web page built with HTML and CSS. This is the Week 2 upgrade of my Week 1 project. I continued building on the same `index.html` and `style.css` files instead of starting a new project.

## What I Built

This week I added four new layers to the tracker: an expense table, an upgraded form, multimedia content and interactive elements. I then styled everything with advanced CSS selectors.

## Files in This Project

| File | Purpose |
|------|---------|
| `index.html` | The structure and content of the page |
| `style.css` | All colors, layout, hover effects and selectors |
| `logo.svg` | The logo image shown beside the main heading |
| `README.md` | This explanation of the project |

## What Each Part Does

### 1. Expense Table
- Built with `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>` and `<td>`.
- The header row has four column headings: Name, Amount (KES), Category and Date.
- The body has 5 hardcoded sample expenses with dates from 21 to 25 September 2026.
- In CSS: `border-collapse: collapse`, cell padding, a green header row and alternating row colors using `tbody tr:nth-child(even)`.

### 2. Upgraded Add Expense Form
- All inputs are wrapped inside a proper `<form>` element.
- The category field is a `<select>` dropdown with Food, Transport, Rent, Entertainment and Other.
- Every input has a clear ID that will be used by JavaScript later: `expense-name`, `expense-amount` and `expense-category`.
- The "Add Expense" button uses `type="button"`. It does nothing yet, because the functionality comes in Week 7.

### 3. Multimedia
- **Image:** `logo.svg` sits beside the main heading, with `src`, `alt` and `width` attributes.
- **Video:** a YouTube budgeting video is embedded with an `<iframe>` that has `width`, `height`, `title` and `frameborder` attributes.

### 4. Interactive Elements
- A collapsible "How to use this tracker" section using `<details>` and `<summary>`.
- Table rows change color on hover with `tbody tr:hover`.
- The button shows the hand cursor with `cursor: pointer`.

### 5. Advanced CSS Selectors

| Selector | What it does |
|----------|--------------|
| `.expenses-section td` (descendant) | Styles every table cell inside the expenses section |
| `.input-group > input` (direct child) | Gives inputs directly inside each group a light green background |
| `tbody tr:last-child td` (position) | Makes the last table row bold |
| `input:not([type="number"])` (negation) | Thickens the border of every input except the number input |
| `input:focus, select:focus` (focus) | Adds a green glow to the field being typed in |

## How to Run It

1. Download or clone this repository.
2. Keep all four files in the same folder.
3. Open `index.html` in a browser, or right-click it in VS Code and choose **Open with Live Server**.

## Challenges I Faced

- **Leftover text in my HTML:** when I first added the table, some placeholder text got pasted into my `<p>` tag and the table did not show. I fixed it by replacing the section with clean code and checking the file line by line.
- **YouTube error:** my first video showed a playback error because the iframe still contained a placeholder video ID. I learned that the link must use `/embed/` and must be a real video that allows embedding.
- **Missing logo:** the image did not show until I created `logo.svg` in the same folder as `index.html`. The file name in `src` must match exactly.

## Reflection

This assignment taught me how much structure matters in HTML. Before this, I thought a table was just rows of text, but using `<thead>`, `<tbody>`, `<th>` and `<td>` correctly makes the data easier for browsers and screen readers to understand. It also made the CSS easier, because I could target the header and the data rows separately.

The hardest part was debugging. Small mistakes, like a misplaced tag, a placeholder video ID or a wrong file name, stopped parts of the page from working. These taught me to check my files carefully, test often in Live Server and read errors instead of panicking.

I also learned that CSS selectors give precise control over a page. Using `:nth-child`, `:hover`, `:not()` and `:focus` let me change how the page looks and reacts without adding extra classes everywhere. The `:focus` glow in particular made the form feel more professional and easier to use.

In the coming weeks I want to make the tracker actually work: the "Add Expense" button should add new rows to the table, which needs JavaScript. The IDs I added this week will help with that. I also want to make the layout work better on phones, since many people in Kenya use their phones to manage money.

## Author

Run Hajir Shurie