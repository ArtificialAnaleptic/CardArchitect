# Card Architect v12

## Note: there appears to be an issue rendering the page in BRAVE BROWSER. Don't use brave to access the site.

<img width="800" alt="image" src="https://github.com/user-attachments/assets/44153ff7-9f96-4761-8793-a74da61a05b9" />

**Card Architect v12** is a standalone, single-file web application designed for creating, editing, and printing high-fidelity tabletop RPG unit cards. It features a dual-pane layout with a real-time editor sidebar and a live preview canvas. I have not developed this much further because there wasn't much interest and I already have the cards made that I need. But maybe others would like to adapt it to their own needs so I'm putting it up here.

## Features
* **Zero Dependencies:** Runs entirely in the browser using a single HTML file.
* **Layered Art System:** Supports separate uploads for Background, Character Art, and Icons with Z-index layering.
* **Smart Typography:** Unit names automatically resize to fit the header without breaking layout.
* **Dynamic Health Tracking:** Automatically generates health nodes or skull icons based on numeric input.
* **Behavior AI Loops:** Visualizes enemy behavior patterns with automatic loop connectors.
* **Print Ready:** Includes specific CSS to strip UI elements and print only the high-resolution card.

## How to Use

### 1. Imagery Control
* **Uploads:** Select images for the Card Background, Character Art (middle layer), and Top-left Icon.
* **Positioning:** Use the directional arrows and Zoom (+/-) buttons in the editor to perfect the placement of the Character Art within the frame.

### 2. Stats & Weapons
* Modify **Core Stats** (Move, Def, Health, Group) to see immediate updates.
* Select a **Weapon Icon** (Melee, Ranged, Magic, Beast) and define range/dice/hit/crit values.
* *Note: Setting Health to 0 displays a large Skull icon.*

### 3. Abilities Syntax
The abilities text area supports specific shortcodes to render icons and formatting:
* `[action]` : Renders a square trigger icon (■).
* `[O]` : Renders a dashed circular token slot (useful for tracking ability usage).
* `<b>Name</b>`: Wraps text in bold tags to style it as an ability header.

### 4. Behavior Loop
1.  Select a node type: **Black Die**, **Red Die**, **Action**, or **Free Text**.
2.  Click **Add**.
3.  The system automatically draws arrows between nodes and a loop bracket connecting the start and end.
4.  *Constraint:* Max limit of 6 behavior slots.

## Installation
Simply download the `.html` file and open it in any modern web browser (Chrome, Firefox, Edge). An internet connection is required to load the Google Fonts and FontAwesome icons but it will work without them.

# NOT IMPLEMENTED
* Import/Export
* Non-numbers for move characteristic (like "D6").
* Good printing (current implementation sucks but I'm yet to actually find a consistent and good one).
* Hero card generation (you can fudge it with these but it's targetting enemy card gen).
