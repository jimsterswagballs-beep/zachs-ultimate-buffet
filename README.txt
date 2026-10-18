ZACH'S ULTIMATE BUFFET — v29

WHAT'S NEW IN v29
- Multiplayer: added several STUN servers for improved peer-to-peer network discovery and a CDN fallback if PeerJS does not load from unpkg.
- Attack warnings: high-contrast dark outlines, animated yellow/white warning edges, clearer active hazard colors, and a shrinking timer ring for circular danger zones. Attack/phase callouts now sit on a dark panel with a bright border.
- Chef Chaos: Last Stand attacks are spaced out slightly more; his signature lane/ring pattern uses fewer hazards, and his Soup Splash/Rolling Pins attacks are a little less dense.
- The original single-player mode, music, and other bosses are retained.

HOW TO PLAY SINGLE-PLAYER
1. Extract this ZIP.
2. Keep the music folder beside game.html and index.html.
3. Open game.html (or index.html) in a modern browser.
4. Controls: WASD / arrow keys to move; mouse aim + hold to fire; Space, Shift, or right-click to eat nearby projectiles; Esc to pause.

HOW TO MAKE MULTIPLAYER WORK FROM OTHER COMPUTERS
The game needs to be published on a public HTTPS website first. A file:// URL, localhost URL, or private LAN address only points to a computer on that local machine/network and will not work as a shareable invite.

A simple free static-hosting option is GitHub Pages:
1. Create a GitHub repository for the game.
2. Upload index.html, game.html, README.txt and the entire music folder into the published root (do not leave them buried inside another folder, and do not rename the music folder).
3. In the repository, open Settings > Pages and enable publishing from your main branch/root folder. GitHub Pages provides HTTPS for github.io sites.
4. Open the published HTTPS site in your browser, choose Multiplayer, pick a fighter, then choose CREATE ROOM.
5. When the room appears, choose COPY INVITE LINK and send that URL to your friends. Friends should open that exact link; it automatically joins the room. They then choose their fighter and press READY.
6. Keep the host's browser tab open for the whole run. Closing it closes the room.

NETWORK LIMITATIONS / TROUBLESHOOTING
- Both players need internet access and the PeerJS client/service must be reachable. If PeerJS fails to load, reload or try another network/browser that does not block the CDN.
- v29 uses multiple public STUN servers, which can improve direct connections, but this does not guarantee every network can connect. Some strict NATs, school networks, VPNs, and firewalls block direct WebRTC connections.
- For reliable connections across restrictive networks, add a TURN relay service and its credentials to MP_PEER_OPTIONS in both HTML files. TURN credentials should not be exposed as permanent secrets in a public repository; use a provider's recommended short-lived credentials or a server you control.
- There is no dedicated authoritative server in this project: the host's browser runs the boss-rush simulation and broadcasts game snapshots to guests. If the host closes the tab or loses connection, the room ends.

Official references:
- GitHub Pages setup: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- PeerJS ICE/TURN configuration and NAT caveats: https://peerjs.com/client/faq
