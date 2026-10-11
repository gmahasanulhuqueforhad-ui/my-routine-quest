MY ROUTINE QUEST — INSTALLABLE PWA (MAC + ANDROID)
1. Extract this ZIP on your Mac.
2. Open Terminal, cd into the extracted folder.
3. Start local server: python3 -m http.server 8000 --bind 127.0.0.1
4. Open a second Terminal tab/window.
5. Install Cloudflare Tunnel if Homebrew is available: brew install cloudflared
6. Start temporary HTTPS tunnel: cloudflared tunnel --url http://localhost:8000
7. Copy the https://....trycloudflare.com URL printed in Terminal and open it in Android Chrome.
8. Chrome menu (⋮) -> Install app / Add to Home screen.
9. Keep both server and tunnel running. Quick tunnel URL changes when restarted.
Files included: index.html, manifest.webmanifest, sw.js, icon.svg, icon-192.png, icon-512.png.
Caution: Quick Tunnels are for testing and the URL is public to anyone who has it. Do not put private files in the served folder.
Offline shell is cached after first successful load. Browser storage is local to this site origin. Export backups regularly.
Android may throttle timers while app is backgrounded.
