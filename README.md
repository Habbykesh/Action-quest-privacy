# action-quest-privacy

Hosts the public Privacy Policy page for the Action Quest Discord bot, for use
in Discord's privileged-intent application form.

## 1. Create the GitHub repo

1. Go to https://github.com/new
2. Owner: **Habbykesh**, Repository name: `action-quest-privacy`
3. Keep it **Public** (required for free GitHub Pages)
4. Don't initialize with a README (you already have one here) — click **Create repository**

## 2. Push this folder

From inside this unzipped folder:

```bash
git init
git add .
git commit -m "Add privacy policy page"
git branch -M main
git remote add origin https://github.com/Habbykesh/action-quest-privacy.git
git push -u origin main
```

If prompted for credentials, use a GitHub personal access token as the password
(GitHub no longer accepts account passwords over HTTPS git pushes) — generate
one at https://github.com/settings/tokens if you don't have one.

## 3. Turn on GitHub Pages

1. On GitHub, open the `action-quest-privacy` repo → **Settings** → **Pages**
   (left sidebar, under "Code and automation").
2. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
3. Under **Branch**, choose **main** and folder **/ (root)** → **Save**.
4. Wait ~1 minute, then refresh the Pages settings tab — it will show your live URL:

```
https://habbykesh.github.io/action-quest-privacy/
```

## 4. Use it in Discord's form

Paste that URL into the "Privacy Policy" field of the privileged intent
request form in the Discord Developer Portal.

## Updating later

Edit `index.html`, then:

```bash
git add .
git commit -m "Update privacy policy"
git push
```

GitHub Pages redeploys automatically within a minute or two.
