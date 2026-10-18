ZACH'S ULTIMATE BUFFET — v31

WHAT'S NEW IN v31
- Co-op death screen: choose WAIT FOR REVIVAL / SPECTATE or LEAVE CO-OP / RETURN TO TITLE. Waiting lets you watch the boss fight, and you return with one heart after the boss is defeated.
- Emergency team revive: if every player is down at once, the entire team is brought back with one heart and temporary invulnerability so a run cannot get stuck waiting for a boss nobody can damage.
- Clearer multiplayer usernames and lobby roster: edit your name in the room, see each player's ready status, and see names/health during the fight. Names are saved locally.
- Better connection feedback: join timeouts and disconnected hosts are explained, guests can retry a failed join, the PeerJS signalling connection attempts recovery, and busy data channels skip snapshots instead of building up a lagging queue. Game-state snapshots are sent at a gentler rate to improve stability.
- Multiplayer state now includes the host player for guests, and the lobby shows clearer player/ready chips.

FILES
- index.html: game entry point.
- game.html: game.
- music/: soundtrack used by the game. Keep this folder beside both HTML files.

HOW TO UPDATE YOUR EXISTING GITHUB PAGES SITE
1. Extract this ZIP on your computer.
2. Open your repository: https://github.com/jimsterswagballs-beep/zachs-ultimate-buffet
3. Click Add file > Upload files.
4. Drag the updated index.html, game.html, README.txt, and the whole music folder from this extracted v31 folder into the upload area. Do not drag the outer ZachsUltimateBuffet_v31 folder.
5. Commit directly to main with a message such as "Update game to v31".
6. GitHub Pages should redeploy automatically. Refresh the public website; if you still see the old version, use Ctrl+F5 or a private window.

MULTIPLAYER NOTES
- Host the game on the public HTTPS GitHub Pages URL and send the in-game invite link to friends. The host's browser tab must stay open.
- If joining times out, ask the host to create a fresh room and send a new invite link.
- The networking improvements help on common home networks, but some strict routers/firewalls still require a configured TURN relay. This package uses public STUN services only.
