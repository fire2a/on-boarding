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
