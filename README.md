# flow

minimalist, productivity tool. Vanilla HTML/CSS/JS.

<img width="1017" height="604" alt="image" src="https://github.com/user-attachments/assets/d5e2ef36-30a8-4a47-b442-a4aabef631b8" />
<img width="1061" height="569" alt="image" src="https://github.com/user-attachments/assets/3e464d58-3a78-4301-9e2d-338f1655d8ca" />

## Architecture
* **Zero Dependencies:** No frameworks or build steps.
* **Decoupled Logic:** "Notes" (string) and "Tasks" (JSON array) operate as independent data streams.
* **Persistence:** `localStorage` saves state on every keystroke (`input` event).

## Technical Features
* **Auto-Sorting:** Completed tasks automatically move to the bottom via boolean sort (`a.done - b.done`).
* **Native Feel:** Uses Apple System font stack (`-apple-system`) and mobile-optimized touch targets.
* **Performance:** CSS-only animations; SVG noise generation avoids external image requests.

## Data Structure
* **Tasks:** `[{ "text": "string", "done": boolean }]` stored in `flow_tasks_v2`.
* **Notes:** Raw string stored in `flow_notes_v2`.

## Usage
1.  Clone repo.
2.  Open `todo.html`.
## Customization

to modify the color scheme, edit the CSS variables in the `:root` selector:

```css
:root {
    --bg: #050505;
    --card: rgba(255, 255, 255, 0.96);
    --accent: #000000;
}
