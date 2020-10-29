# git-commands

A small collection of user friendly git commands.

- `git last-tag` displays the latest tag.
- `git next-tag` increments SemVer style tags. Args `major|minor|patch(default)`.
- `git purge` clean up task deleting all branches merged into master.
- `git info` display branches colour coded by merged status.
- `git main` checks for master or main branch, exits with error if none or both are found.
- `git migrate-branch` built to support the switch to `main` branch. A move from the technology industry to abolish slavery references. Also supports migrating arbitary branches from one name space to another. `git migrate` assumes `git mirgrate master main`. Steps involeda are. 
  1. Check your current branch status
  2. Checkout deprecated branch
  3. Branch to new namespace
  4. Push to origin
  5. Delete deprecated branch locally
  6. Finally delete from remote.
- `git prettylog` oneline summary log output.
- `git mv-branch` script to move/migrate branch names locally & on remote. By default it migrates master branch to main for a more inclusive tech industry.

### Why Git Commands

Git or bash aliases are usful, but hard to share and maintain across machines ie.
Personal and Work machines. Let alone keeping a team in sync.

This allows version controlled commands standardised by ShellCheck.

### Set up

Git recognises commands in your $PATH with a prefix of `git-`. You can clone this directory and incude the `/bin` folder in your path. Or copy the contents to another location already in your path.

```
git clone git@github.com:bambii7/git-commands.git
cd git-commands
printf 'export PATH="%s:$PATH"' "$PWD/bin" >> ~/.bash_profile
source ~/.bash_profile
### you may want to restart your terminal, .bash_profile is only read once on start.
```

The benifits of keeping this repo in your PATH is to be able to pull updates when they occur.
Moving the scripts to a seperate folder keeps you responsible to sync script updates or renames.

### Licence

[MIT Licence](LICENSE.md)