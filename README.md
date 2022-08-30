# ### KESIMPULAN ###
## ( CONFIGURATION )
1. git config (--global, --local) (user.name, user.email) "Value"
2. git config (--global, --local) (auto.crlf) (true, input)
3. git config (--global, --local) (code.editor) "code --wait"
4. git config (--global, --local) diff.tool vscode
5. git config (--global, --local) difftool.vscode.cmd "code --diff --wait $LOCAL $REMOTE"
6. git config (--global, --local) merge.tool p4merge
7. git config (--global, --local) mergetool.p4merge.path "C://yourpath"
8. git config (--global, --local) mergetool.keepBackup false
9. git config (--global, --local) alias.graph "log --oneline --all --graph"
10. git config (--global, --local) ff no || no fast-forward merge

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
1. git log [filename.js, --oneline, --all, --graph, --stat, --patch, --author="name", --before="12-12-12", --after="10-10-10", --grep="Search title", -S"Search contents", --pretty="format:'%un %Cgreen %cd testing'"]
2. git diff [--staged, --name-only, --name-status] (branchA branchB, commitA commitB)
3. git show (idCommit, HEAD~2) [--name-only, --name-status]
4. git bisect start -> git bisect good idCommit -> git bisect bad idCommit -> git bisect reset
5. git shortlog [-n, -s, -e, --before="", --after=""]
6. git checkout idCommit fileName || Restore deleted file
7. git blame [-e, -L 1,4] filename.js
8. git tag [-n, -d] -a v.1.0.0 -m "Description" or git tag v.1.0.0 idCommit

## ( Branches )
1. git branch [-d, -D, --merged. --no-merged] newBranch
2. git stash push [-a, -m, -am] "Message Description" -> git stash list -> git stash show 1 -> git stash apply 1 -> git stash drop 1 or git stash clear
3. git merge [--abort, --continue, --squash] {fast-forward, 3-way}
4. git reset [--soft, --mixed, --hard] (idCommit, HEAD~1)
5. git revert -m 1 HEAD
6. git rebase [--continue, --skip, --abort] branchA
7. git cherry-pick idCommit