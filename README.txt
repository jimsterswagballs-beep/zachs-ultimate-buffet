ZACH'S ULTIMATE BUFFET — v34

WHAT'S NEW IN v34
- Cartman uses the supplied picture as an in-game sprite. Keep cartman.png in the same repository folder as index.html and game.html.
- Triple T's primary fire cooldown is fixed at 0.5 seconds in solo play and co-op.
- Triple T receives three new abilities: Shadow Slip, Bat Echo Cage, and Night Flight.
- Cartman receives three new abilities: Cheese Meteor, Lunchroom Lockdown, and Lunch Money Rain.
- Co-op settings expanded to six options: boss health, player limit, revival health, revival protection, boss attack pace, and starting health.
- Host settings synchronize to guests and lock after the run starts. Player count remains 2–4 including the host.

FILES
- index.html: game entry point.
- game.html: game.
- cartman.png: transparent Cartman image based on the supplied picture.
- music/: game soundtrack. Keep the folder beside both HTML files.
- PATCH_NOTES_v33.txt and PATCH_NOTES_v34.txt: update summaries.

HOW TO UPDATE YOUR EXISTING GITHUB PAGES SITE
1. Extract this ZIP on your computer.
2. Open your repository: https://github.com/jimsterswagballs-beep/zachs-ultimate-buffet
3. Click Add file > Upload files.
4. Drag index.html, game.html, README.txt, cartman.png, PATCH_NOTES_v34.txt, and the whole music folder into the upload area. Do not drag the outer ZachsUltimateBuffet_v34 folder.
5. Commit directly to main, for example with the message "Update game to v34".
6. GitHub Pages redeploys automatically. Refresh the public website; if needed, use Ctrl+F5 or a private window.

CO-OP NOTES
- Host the public HTTPS GitHub Pages URL and send the in-game invite link to your friends. The host's tab must remain open.
- The six room settings are host-controlled once a room exists and become locked when the run starts.
- Triple T's normal fire cooldown remains 0.5 seconds; Night Flight adds extra side-bats without changing that cooldown.
- Direct player-to-player WebRTC connections may still fail on restrictive networks; some networks require a configured TURN relay.


V34 CHANGES
- Boss base health +45%; multiplayer scales automatically by active room size: 1 player 1.00x, 2 players 1.75x, 3 players 2.50x, 4 players 3.25x. Boss HP bonus setting scales this further.
- The Hollow King is slower and has longer attack cooldowns.
- Added unique attacks for the first six bosses and clear pre-attack warnings.
- Settings now include Attack Warnings and Show Hitboxes.
- Admin cheat panel: open Settings, click ADMIN CODE, enter BUFFET-OVERDRIVE-777. It supports random upgrades, three random upgrades, full heal, +1 max heart, and skipping a boss. The code is visible in the downloadable client and is not secure against other players inspecting source.
