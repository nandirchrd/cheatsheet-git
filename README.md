# ### KESIMPULAN ###

## ( CONFIGURATION )
1. git config (--global, --local) (user.name, user.email) "Value"
2. git config (--global, --local) (auto.crlf) (true, input)
3. git config (--global, --local) (code.editor) "code --wait"
4. git config (--global, --local) (diff.tool) vscode
5. git config (--global, --local) (difftool.vscode.cmd) "code --diff --wait $LOCAL $REMOTE"
6. git config --global alias.graph "log --oneline --all --graph"

## ( GETTING STARTED )
1. git init
2. git status [-s] 
3. git add (filename, *.js, .)
4. git rm filename [--cached] 
5. git mv oldname newName 
6. git ls-files
7. git commit (-m, -am) "Commit message"
8. git restore [--staged, --source=idCommit] (filename, *.js, .)
9. git clean [-i, -n, -f]

## ( Browsing History )
1. git log [filename.js, --oneline, --all, --graph, --stat, --patch, --author="name", --before="12-12-12", --after="10-10-10", --grep="Search title", -S"Search contents", --pretty="format:'%un %Cgreen %cd blalvbal'"]
2. git diff [--staged, branchA branchB, commitA commitB, --name-only, --name-status]
3. git show (idCommit, HEAD~2) [--name-only, --name-status]