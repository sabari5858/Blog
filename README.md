# Profile site
## Deploy
1. Create a PUBLIC repo named `<username>.github.io`; upload index.html and data/site.json to `main`.
2. Settings > Pages > Deploy from a branch > main > / (root).
3. Open https://<username>.github.io/#admin > Profile > set your GitHub username and LinkedIn > Apply.
## Admin (add / edit / delete / reorder anything)
Profile, Experience, Skills, Projects and Blog posts all have Add, Edit, Delete and reorder buttons at /#admin.
Changes live in your browser until you press "Save to GitHub", which commits data/site.json.
Token: GitHub > Settings > Developer settings > Fine-grained tokens > only this repo > Repository permissions > Contents: Read and write.
Never paste the token into a file or commit it. If you skip the token, use "Download site.json" and upload it to data/ yourself.
## Local preview
`python -m http.server` in this folder, then open http://localhost:8000 (file:// will not load the JSON).
## Notes
Resume: do not upload your resume PDF as-is if it contains your phone number or email. Make a public version, put it in the repo, and set its path in Admin > Profile > Resume.
Admin sections: Profile, Experience, Technical contributions, Skills, Education, Projects, Blog posts.
