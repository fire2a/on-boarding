# fire2a-on-boarding

## git
### there are 10 commandments

<img src="https://imgs.xkcd.com/comics/git_2x.png"  alt='cannot load image' width="500px" >

```bash
git clone git@github.com:fire2a/C2F-W.git
cd C2F-W

# alternative A
git pull
# B
git fetch 
git switch [-c] my-feature-branch [main]

git add new_or_changed_text_file
git commit -m "sentence that explains the purpose of the changes"

git push [--set-upstream origin my-feature-branch]

# B pull request
firefox https://github.com/fire2a/C2F-W/compare/main...my-feature-branch
```

### [optional] follow the rabbit hole
- [recommended] diff files between branches, commits, etc.
- merge: branches, 2-3 way
- cherry pick

## github organization
1. Every team member has write as default privileges. Be respectful of other people branches
2. When creating a new public repo (can't be done with private), create a protection rule for the main branch:
   - requiring pull requests
   - disallowing push
   <img src="https://github.com/user-attachments/assets/573f21f8-b666-4164-9baa-9bc511051c0b"  alt='cannot load image' width="400px" >
