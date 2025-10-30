README - How to make this project readable by Microsoft Copilot / GitHub Copilot

1) GitHub/OneDrive
   - The easiest approach is to upload the extracted folder to a GitHub repository or to OneDrive/SharePoint.
   - GitHub Copilot can read files in repositories; uploading the extracted files (not zipped) is recommended.

2) File formats
   - Avoid uploading a single .zip. Upload the extracted directory tree so Copilot can index files.
   - If you must upload an archive, prefer a plain .tar.gz (some tools index it better), but GitHub still prefers the repo.

3) Steps (local)
   - unzip TS25_ZONE_ServerSide.zip
     Windows: right-click -> Extract All
     Linux/Mac: unzip TS25_ZONE_ServerSide.zip -d TS25_ZONE_ServerSide_extracted
   - create a Git repo:
     git init
     git add .
     git commit -m "Initial import"
     Create repo on GitHub and push:
     git remote add origin <your-github-repo-url>
     git branch -M main
     git push -u origin main

4) If you want, I created a tar.gz bundle that you can download from this chat and upload directly to GitHub or cloud storage.

5) If you want, I can:
   - list specific file types (e.g. .cpp, .h, .txt) and show the top-level tree here,
   - extract and show contents of specific files,
   - create a minimal project README or restructure repository for easier navigation by Copilot.

