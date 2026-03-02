# Album Review Widgets

Interactive vinyl record widgets for Substack album reviews.


## SETUP (one time)

### 1. Create a GitHub repo
- Go to github.com → click **+** → **New repository**
- Name it **album-reviews**
- Set to **Public**
- Check **"Add a README file"** (this creates the repo for you)
- Click **Create repository**

### 2. Upload files to the repo
- In your new repo, click **Add file** → **Upload files**
- Drag in: `TEMPLATE.html` and `042-rumours.html`
- Click **Commit changes**

### 3. Deploy on Vercel
- Go to vercel.com/new
- Select your **album-reviews** repo
- **Framework Preset**: Other
- **Root Directory**: leave blank
- **Build Command**: leave blank
- **Output Directory**: leave blank
- Click **Deploy**
- After it finishes, Vercel shows your URL (something like `album-reviews.vercel.app`)

### 4. Test it
- Visit: `https://YOUR-VERCEL-URL/042-rumours.html`
- You should see the interactive vinyl widget


## ADDING NEW ALBUMS

1. Download `TEMPLATE.html` from the repo
2. Open it in any text editor
3. Edit the album data section at the top (rank, title, artist, year, tracks)
4. Save As with the format: `000-album-name.html` (example: `039-blue.html`)
5. Go to GitHub repo → **Add file** → **Upload files** → drag the new file in → Commit
6. Vercel auto-deploys in ~30 seconds
7. Your new widget lives at: `https://YOUR-VERCEL-URL/039-blue.html`


## EMBEDDING IN SUBSTACK

In the Substack editor:
1. Click **+** to add a block
2. Choose **Embed**
3. Paste the URL: `https://YOUR-VERCEL-URL/042-rumours.html`

If the embed looks cropped, use a **Custom HTML** block instead:
```html
<iframe src="https://YOUR-VERCEL-URL/042-rumours.html" width="100%" height="900" frameborder="0"></iframe>
```
