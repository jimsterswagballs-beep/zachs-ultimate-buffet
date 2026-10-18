ZACH'S ULTIMATE BUFFET — v28

WHAT'S NEW
- Multiplayer button added to the title/lobby.
- Host can create a room and copy an invite URL. Friends opening that URL automatically join the room.
- Everyone can choose a fighter and mark themselves READY before the host starts.
- The host runs the boss-rush simulation and broadcasts game snapshots so boss health, screens, upgrades, music timing, and player positions stay synchronised.
- Additional players can move, fire, eat nearby projectiles, take damage, recover after being downed, and use three character-coloured abilities.
- Every boss has 1.75x normal health in a multiplayer run.
- Original single-player mode, Food Court, the ALL JUST A GAME sequence, the Last Stand/boss fixes, and music files are retained.
- index.html is included as a web-hosting entry point; game.html is also kept as the direct game file.

HOW TO PLAY SINGLE-PLAYER
1. Extract the ZIP.
2. Keep the music folder beside game.html / index.html.
3. Open game.html (or index.html) in a modern browser.
4. Controls: WASD / arrow keys to move; mouse aim + hold to fire; Space, Shift, or right-click to eat attacks; Esc to pause.

HOW TO PLAY MULTIPLAYER
Multiplayer needs an internet connection and the game must be opened from a public HTTPS website. A local file URL (file://), localhost, or a private computer path cannot be opened by your friends.

1. Publish the contents of this ZIP to a static HTTPS host. For example, create a GitHub repository, upload index.html, game.html, README.txt and the entire music folder, then enable GitHub Pages in the repository's Settings > Pages. Do not rename or separate the music folder.
2. Open the published website URL in your browser.
3. Choose Multiplayer in the game menu, pick your fighter, and select CREATE ROOM.
4. When the room ID appears, select COPY INVITE LINK and send the copied URL to your friends.
5. Friends open the invite URL, choose their own fighters, and press READY. The host starts CO-OP RUN after everyone is ready. Keep the host tab open for the entire run; closing it closes the room.

The multiplayer connection uses PeerJS's cloud signalling service to help browsers connect, then WebRTC data channels carry the game state between players. The project does not include a dedicated game server. Some networks/firewalls may block direct peer connections; that can require a TURN relay or a different network.

Keep the music folder and the HTML files in the same published directory. The PeerJS client is loaded from unpkg.com when the game opens, so online multiplayer also needs that library to be reachable.
