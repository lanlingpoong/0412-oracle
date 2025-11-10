
# Since 0412 — Cyber Oracle (Demo)

This is a **zero-backend** static demo that shows a *random fortune card image* on each page load or when you tap **New Draw**.

## How it works
- `index.html` picks a random file from `/cards/` and displays it.
- You can add up to **300** images named `001.png` … `300.png`.
- Update the `cards` array in `index.html` to include all your files.

## Deploy (Easiest)

### Option C — Vercel (free)
1. Create a **new GitHub repo** (empty).
2. Upload all files in this folder to that repo (drag & drop on GitHub works).
3. Go to **vercel.com → New Project → Import from GitHub** and select your repo.
4. Hit **Deploy**. Done.
5. Your URL will look like `https://<project>.vercel.app`.
6. Make your QR code point to that URL.

### Super quick test (Netlify Drop)
- Go to **https://app.netlify.com/drop** and drop this folder (or the ZIP).
- Netlify gives you a live URL instantly.
- Use that URL for testing your QR experience.

## Add your 300 cards
1. Put your 300 PNGs into `/cards/` named `001.png` … `300.png`.
2. Open `index.html` and extend the `cards = [...]` list to include all of them.
   (Tip: keep them in order, but randomness is handled by JS)
3. Deploy again (Vercel will auto-redeploy from Git).

## Notes
- This demo is static; it randomizes on the client side.
- For “no repeats until deck is exhausted”, you’d need a lightweight backend.
