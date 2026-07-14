EYE Q&A GAME SHOW — HOSTED WEB PACKAGE
=======================================

Source
------
Converted from EYE_Game_Show_Practice_v3_17b.html.
The game interface and behavior have not been intentionally redesigned.

Main file
---------
index.html

Folder structure
----------------
css/app.css                  App styling
js/app.js                    App data and behavior
images/category-sheets/      15 category/level display sheets
images/items/                Item artwork, logos, and other interface images
audio/                       Game sounds
asset-manifest.json          Extracted asset inventory with hashes

Local testing
-------------
Do not rely only on double-clicking index.html because browser security rules can differ from a real website.
From this folder, run a simple local web server, for example:

    python3 -m http.server 8080

Then open:

    http://localhost:8080

Deployment
----------
Upload the CONTENTS of this folder to the root of a static host such as Cloudflare Pages or Netlify.
The host must serve index.html as the site homepage.

Updating a category sheet
-------------------------
Replace the matching JPG in images/category-sheets/ while keeping the same filename and 16:9 canvas dimensions.
The filenames are organized by category and level.

Important testing checklist
---------------------------
- Splash screen and external links
- Classroom Mode timer: start, pause, resume, and custom durations
- MC Mode timer and custom durations
- Scoring and reset controls
- Category and level sheets
- Audience display / second-window synchronization
- Sounds after the first user interaction
- Fullscreen behavior
- Chrome and Safari

Offline backup
--------------
Keep EYE_Game_Show_Practice_v3_17b.html and its ZIP as the standalone offline version.
