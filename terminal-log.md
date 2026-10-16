# Terminal Command Log - Week 03

## Session Overview & Command History

| Step | Command Executed | Purpose / Intent | Result / Terminal Output | Issue / Error Encountered | Correction / Resolution |
|---|---|---|---|---|---|
| **1** | `pwd` | Check current working directory | `/` | None | Initial starting directory was root |
| **2** | `cd OneDrive` | Move to OneDrive directory | `bash: cd: OneDrive: No such file or directory` | Tried to access relative path from `/` root | Ran `cd ~` to return home first |
| **3** | `cd ~` | Return to user home directory | Navigated to `~` (`C:\Users\Admin`) | None | Resolved path location |
| **4** | `cd OneDrive` | Enter OneDrive folder | Navigated to `~/OneDrive` | None | Success |
| **5** | `cd Desktop` | Enter Desktop folder | Navigated to `~/OneDrive/Desktop` | None | Success |
| **6** | `cd IYF_Wev_Dev` | Enter project parent folder | `bash: cd: IYF_Wev_Dev: No such file or directory` | Typo in folder name (`Wev` instead of `Web`) | Re-entered command with correct spelling |
| **7** | `cd IYF_Web_Dev` | Enter project parent folder | Navigated to `~/OneDrive/Desktop/IYF_Web_Dev` | None | Success |
| **8** | `cd IYF-weekend_academy` | Enter academy folder | Navigated to `IYF-weekend_academy` | None | Success |
| **9** | `cd season 12/tasks` | Move into tasks directory | `bash: cd: too many arguments` | Space in directory name (`season 12`) without quotes/hyphen | Used hyphenated path `season-12/tasks` |
| **10** | `cd season-12/tasks` | Move into tasks directory | Navigated to `season-12/tasks` | None | Success |
| **11** | `mkdir iyf-s12-wee-o3-HellenWamuciiNjue` | Create project directory | Directory created | Typo in name (`wee-o3` instead of `week-03`) | Used `mv` command to rename folder |
| **12** | `mv iyf-s12-wee-o3-HellenWamuciiNjue iyf-s12-week-03-HellenWamuciiNjue` | Rename project folder | Folder renamed to `iyf-s12-week-03-HellenWamuciiNjue` | None | Fixed typo without recreating folder |
| **13** | `cd iyf-s12-week-03-HellenWamuciiNjue` | Enter project directory | Navigated into project folder | None | Success |
| **14** | `git init` | Initialize Git repository | `Initialized empty Git repository...` | Default branch set to `master` | Used `git branch -m main` to rename |
| **15** | `git branch -m main` | Rename branch to `main` | Branch switched to `main` | None | Success |
| **16** | `git status` | Check repository status | `On branch main / No commits yet` | None | Verified clean initial state |
| **17** | `touch terminal-log.md .gitignore README.md` | Create project core files | Files created | None | Created core documentation and config files |
| **18** | `git ls` | Try listing directory contents | `git: 'ls' is not a git command.` | Used Git syntax for a standard Unix command | Used standard `ls` and `ls -a` instead |
| **19** | `ls` | List visible files | `README.md terminal-log.md` | None | Showed standard files |
| **20** | `ls -a` | List all files including hidden | `./ ../ .git/ .gitignore README.md terminal-log.md` | None | Confirmed hidden `.git` and `.gitignore` exist |
| **21** | `mkdir daily-challenges` | Create daily challenges folder | Directory created | None | Success |
| **22** | `git add .` | Stage all project files | Files staged | None | Success |
| **23** | `git commit -m "initialize project and daily-challenges directory"` | Save first commit | `[main (root-commit) acf34fb]` | None | First commit saved locally |
| **24** | `touch LICENSE` | Create LICENSE file | File created | None | Success |
| **25** | `echo "MIT License" > LICENSE` | Add license text | Text written to file | Line ending warning (LF to CRLF) | Normal cross-platform Windows warning |
| **26** | `git add LICENSE` | Stage LICENSE file | File staged | None | Success |
| **27** | `git commit -m "docs: add MIT license"` | Commit LICENSE | `[main 3f4db53] docs: add MIT license` | None | Second commit saved locally |
| **28** | `git push origin main` | Attempt early push | `fatal: 'origin' does not appear to be a git repository` | Remote origin not linked yet | Linked remote origin before pushing |
| **29** | `git remote add origin https://github.com/HellenWamuciiNjue/iyf-s12-week-03-HellenWamuciiNjue.git` | Link local repo to GitHub | Remote link established | None | Success |
| **30** | `git push -u origin main` | Push local commits to GitHub | `To https://github.com/HellenWamuciiNjue/iyf-s12-week-03-HellenWamuciiNjue.git * [new branch] main -> main` | None | Successfully pushed local repository to GitHub |
| **31** | `nano terminal-log.md` | Edit log file | Opened Nano text editor | None | Documented terminal history |
| **32** | `git checkout -b feature/daily-challenges` | Create and switch to feature branch | Switched to a new branch 'feature/daily-challenges' | None | Isolated feature development from main branch |
| **33** | `touch daily-challenges/day-01.md` | Create Day 1 challenge markdown file | File created | None | Created file inside daily-challenges folder |
| **34** | `nano daily-challenges/day-01.md` | Edit Day 1 challenge content | Documented Day 1 challenge reflection | None | Saved reflection in daily-challenges/day-01.md |
