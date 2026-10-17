# Gold Rush

A real-time multiplayer coin arena for 2 to 4 players. It runs in the browser, with no login and nothing to install.

**Play:** https://ajjuahmad.github.io/gold-rush/

## How to play

1. One player presses **Create room** and shares the 4-letter code (or the invite link).
2. Friends open the page on any phone or laptop, type the code and press **Join**. The host can also press **Add bot** to fill empty seats.
3. The host presses **Start game**.

Pick up coins (gold ones are worth 3) and carry them to the glowing base in your colour to bank them. The more you carry, the slower you move. **Space** (or the Dash button) lunges forward: hit a rival outside their base and you steal half of their load while the rest spills on the floor. Most banked coins after 90 seconds wins.

Controls: WASD or arrow keys to move, Space to dash. On phones, use the on-screen stick and button.

## How the multiplayer works

The host's browser runs the game and sends snapshots about 15 times a second. Everyone else sends only their input. Connections are peer to peer (WebRTC through PeerJS), so the site is static and needs no game server of its own.

Notes: the host must keep the tab open and in the foreground. Players on strict mobile-carrier networks may need Wi-Fi to connect.

## Run locally

Open `index.html` through any static server. Add `?local` to the address to test with two tabs of the same browser, without the network.

Built by Ejaz Ahemad with AI assistance.
