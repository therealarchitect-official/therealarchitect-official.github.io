# Project Overview: TheRealArchitect Retro Terminal Portfolio
"3 portfolios. One terminal."
This project is an interactive, 8-bit CRT retro terminal web portfolio for **TheRealArchitect**. It unifies three distinct creator identities into a single command-line interface with clickable mobile-friendly shortcuts and dynamic theme switching.

## Core Aesthetics & UI Rules
- **Font:** Use a crisp 8-bit monospace/pixel font (such as `'Press Start 2P'` or `'VT323'` from Google Fonts).
- **Default Theme:** Glowing red text (`#ff2a2a`) on a pure black background (`#050505`) with subtle CRT scanlines, phosphor text-shadow glow, and a blinking block cursor.
- **Mobile Accessibility:** Every command printed in the boot guide or help text MUST also be rendered as a clickable `<span>` or `<button>` that automatically populates the input and executes the command when clicked/tapped.
- **Transitions:** Switching between portfolio modes (`default`, `gd`, `md`) should trigger a brief CRT channel-switch flicker animation and shift the terminal's accent color palette to match the selected mode.

## Required Terminal Commands & Behavior
Implement a clean, modular command parser in JavaScript supporting the following commands:

1. **`help`** (and initial boot screen):
   - Displays the ASCII banner: `3 PORTFOLIOS. ONE TERMINAL.`
   - Lists available commands with clickable triggers: `default`, `gd`, `md`, `lore`, `credits`, `clear`, and a hint for hidden commands.

2. **`default`**:
   - Resets the terminal to the signature red-on-black 8-bit aesthetic.
   - Displays **TheRealArchitect**'s main developer/creator portfolio, skills, and featured web projects.

3. **`gd`**:
   - Shifts the terminal accent theme (e.g., neon cyan/gold Geometry Dash vibe).
   - Displays the **RealArchitectGD** portfolio: Geometry Dash levels, level IDs, collabs, creator stats, and a `launch gd` sub-command/link to preview the Geometry Dash Web portfolio.

4. **`md`**:
   - Shifts the terminal accent theme to match **Munet Dash**.
   - Displays the **ArchitectMunet** portfolio: fan-made Munet Dash web project details, custom assets, and a `launch md` sub-command/link to play/preview Munet Dash Web.

5. **`lore`** (alias: `story`):
   - Prints the creator origin story: How **GDColon's** fan-made Geometry Dash in a browser inspired the creation of the Geometry Dash portfolio, which led to building **Munet Dash Web** by **TheRealArchitect**, with full credit to **Munetios**.

6. **`credits`**:
   - Cleanly formats and displays attributions:
     - `Munet Dash Web` — By **TheRealArchitect**
     - `Geometry Dash Web` — By **GDColon**
     - `Original Munet Dash` — Credits to **Munetios**

7. **`clear`**:
   - Clears the terminal output history while keeping the input prompt active.

8. **Secret Easter Egg (`vault` or `unsolvable`)**:
   - Hidden command that unlocks a classified directory teasing unreleased GD/Munet Dash layouts or an "unsolvable" mini-riddle.

## Coding Guidelines
- Keep the architecture lightweight and dependency-free (semantic HTML5, modern CSS3 with CSS variables for instant theme switching, and vanilla ES6+ JavaScript) unless a framework is already present in the repo.
- Store all command outputs, portfolio items, and theme configurations in a clean data object/config file so new levels, links, or commands can be added easily without rewriting DOM logic.
- Ensure keyboard navigation works seamlessly (auto-focus input, `Enter` to submit, `Up/Down` arrows for command history).
