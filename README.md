# Ageless Athletes

Static site (plain HTML/CSS) for Ageless Athletes: fitness after 40. No build step.

## Structure
- `index.html`: hero + newsletter signup (Beehiiv embed placeholder)
- `about.html`, `affiliate-disclosure.html`, `privacy.html`
- `blog/`: blog index and posts
- `style.css`, `netlify.toml` (`publish = "."`)

## Add the Beehiiv form
In `index.html`, replace the `.embed-placeholder` div (see the comment above it) with the embed code from Beehiiv (Grow > Subscribe Forms > Get embed code).

## Deploy on Netlify
1. Log in at https://app.netlify.com.
2. **Add new site > Import an existing project > GitHub**, authorize Netlify, and pick the `ageless-athletes` repo.
3. Branch to deploy: `main`. Build command: leave empty. Publish directory: `.` (already set in `netlify.toml`).
4. Click **Deploy**. Netlify gives you a `*.netlify.app` URL.
5. Optional: **Domain management > Add a domain** to connect your own domain, then follow the DNS instructions. HTTPS is automatic.
6. Pull requests get Deploy Previews automatically. Merge a PR to `main` to publish it.

## Preview locally
`python3 -m http.server 8000`, then open http://localhost:8000
