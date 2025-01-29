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
git switch [-c] branch-name-is-at-least-a-half-sentence-explaining-the-feature/issue [main]

git add new_or_changed_text_file
git commit -m "sentence that explains the purpose of the change"

git push [--set-upstream origin my-feature-branch]

# B pull request
firefox https://github.com/fire2a/C2F-W/compare/main...my-feature-branch
```

### A learning path

1. (what is git again?) watch any video introduction
2. (novice) [Get started with GitHub documentation](https://docs.github.com/en/get-started/)
3. _(do once)_ [SSH Authentication](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
4. __(essential, must be understood)__ [Contributing to a project](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)
5. [official docs](https://git-scm.com/doc): really good cheat sheets and official manual

### [optional] follow the rabbit hole
- [recommended] diff files between branches, commits, etc.
- merge: branches, 2-3 way
- cherry pick

## coding practices 0
- the best code/document is not the smartest one, but the most legible
- write/name everything as for your future self, when you'd forgotten about it & context
- avoid typing errors by typing as little as possible vs copy/paste
- avoid using unclear variable names, acronyms are usually unclear
  
## our github organization
1. Every team member has write as default privileges. Be respectful of other people branches
2. When creating a new public repo (can't be done with private), create a protection rule for the main branch:
   - requiring pull requests
   - disallowing push
   <img src="https://github.com/user-attachments/assets/573f21f8-b666-4164-9baa-9bc511051c0b"  alt='cannot load image' width="400px" >
3. When opening a pull request, link it to the corresponding issue and explain your code's expected result
