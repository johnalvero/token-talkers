# Token Talkers — The Hidden Layer

A static, single-page landing site for the **Token Talkers** Viber group — an invite-only,
speakeasy-themed community for AI enthusiasts.

## Add your Viber invite link

Open `index.html` and find this line near the bottom (inside the `<script>` tag):

```js
const VIBER_INVITE_LINK = "#REPLACE_WITH_YOUR_VIBER_LINK";
```

Replace it with your real Viber group invite, e.g.:

```js
const VIBER_INVITE_LINK = "https://invite.viber.com/?g2=xxxxxxxx";
```

Both "Join" buttons update automatically. Until you set it, clicking a button shows a
friendly "door isn't open yet" message instead.

## Host on GitHub Pages

1. Create a new GitHub repository and push these files (`index.html` must be at the repo root).
   ```bash
   git init
   git add .
   git commit -m "Token Talkers landing page"
   git branch -M main
   git remote add origin https://github.com/<you>/<repo>.git
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages → Build and deployment**.
3. Set **Source** to *Deploy from a branch*, branch **main**, folder **/ (root)**, then **Save**.
4. Your site goes live at `https://<you>.github.io/<repo>/` within a minute or two.

> Tip: for a custom domain, add it under Settings → Pages and create a `CNAME` file.

## Files

- `index.html` — the entire site (HTML + CSS + JS in one file, no build step, no dependencies).
- `README.md` — this file.
