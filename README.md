# git-commands

A small collection of user friendly git commands.

- `git last-tag` displays the latest tag.
- `git next-tag` increments SemVer style tags. Args `major|minor|patch(default)`
- `git purge-merged` clean up task deleting all branches merged into master.

### Set up

Git recognises commands in your $PATH with a prefix of `git-`. You can clone this directory and incude the `/bin` folder in your path. Or copy the contents to another location already in your path.

```
git clone git@github.com:bambii7/git-commands.git
cd git-commands
printf 'export PATH="%s:$PATH"' $(pwd)/bin >> ~/.bash_profile
```

The benifits of keeping this repo in your PATH is to be able to pull updates when they occur.
Moving the scripts to a seperate folder keeps you responsible to sync script updates or renames.

### Licence
