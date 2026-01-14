SHAE SITE V3 (Upload from Netlify Dashboard via CMS)

This version adds a CMS at /admin so you can upload photos/videos from a dashboard.

IMPORTANT: This only works if your Netlify site is connected to a Git repo (GitHub/GitLab/Bitbucket).
Manual drag-and-drop deploys do NOT support dashboard uploads because the CMS needs somewhere to save files.

NETLIFY SETUP (do this once):
1) Push this folder to a GitHub repo.
2) In Netlify: Add new site -> Import from Git -> select the repo.
3) Site settings -> Identity -> Enable Identity.
4) Identity -> Services -> Enable Git Gateway.
5) Deploys -> Trigger deploy.

Then go to:
https://YOUR-SITE.netlify.app/admin
Login (Netlify Identity), then edit "Galleries" -> upload images/videos.
Uploads will be saved in /uploads and the site will auto-render them on each category page.

Logo files:
Put in /images/logos/logo.png and /images/logos/logo-with-text.png (case-sensitive).

Data file:
CMS edits /data/galleries.json automatically. You shouldn't edit HTML to add media anymore.
