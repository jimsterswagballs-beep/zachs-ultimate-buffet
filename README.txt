ZACH'S ULTIMATE BUFFET — v33

WHAT'S NEW IN v33
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
- PATCH_NOTES_v33.txt: concise update summary.

HOW TO UPDATE YOUR EXISTING GITHUB PAGES SITE
1. Extract this ZIP on your computer.
2. Open your repository: https://github.com/jimsterswagballs-beep/zachs-ultimate-buffet
3. Click Add file > Upload files.
4. Drag index.html, game.html, README.txt, cartman.png, and the whole music folder into the upload area. Do not drag the outer ZachsUltimateBuffet_v33 folder.
5. Commit directly to main, for example with the message "Update game to v33".
6. GitHub Pages redeploys automatically. Refresh the public website; if needed, use Ctrl+F5 or a private window.

CO-OP NOTES
- Host the public HTTPS GitHub Pages URL and send the in-game invite link to your friends. The host's tab must remain open.
- The six room settings are host-controlled once a room exists and become locked when the run starts.
- Triple T's normal fire cooldown remains 0.5 seconds; Night Flight adds extra side-bats without changing that cooldown.
- Direct player-to-player WebRTC connections may still fail on restrictive networks; some networks require a configured TURN relay.
