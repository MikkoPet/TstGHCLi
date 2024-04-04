# GhCLI common commands  

## SETUP
#### git auth login
setup link with ghub accnt  

#### gh config set editor
+editors name  
sets up the editor for CLI  

#### gh alias set
sets frequent use aliases  

## REPO MANAGEMENT

#### gh repo create [name] 
creates repo of [name]  
- **-p**, **--template [repolnk]**, uses a repo as template
- **-t**, **--team [name]**, grants access to org of [name]
- **-c**, **--clone**, clones the repo locally

#### gh repo fork [repolnk]
forks repo  

#### gh repo clone [repolnk][dir]
clones a repo  

#### gh repo view [repolnk] 
views dist repo
- **-b** **--branch [string]** view specific branch
- **-w**, **--web**, opens repo in browser  

## ISSUES

#### gh issue create
creates an issue
- **-t**, **--title [string]**, specifies title
- **-l**, **--label [name]**, adds a label
- **-a**, **--assignee [login]** assigns people to the issue. 
    - @me self assigns the task

#### gh issue list
lists issues  
- **-a**, filters by assignee
- **-A**, filters by author
- **-s [open|closed|all]**, filters by state
    - on default, is "open"
- **-l** filters by label

#### gh issues status
shows status of issues  

#### gh issues view (number | url)
view specified issue
- **-c** displays comments

#### gh issue close (number | url)  
closes issue
- **-c** adds a closing comment
- **-r** specifies reason for closing

## PR

#### gh pr create
creates pull request
- **-a**, which branch to merge into
- **-f**, uses last commit info as PR title and body
- **-l**, adds label  

#### gh pr list
lists pull request
- **-a**, filters by assignee
- **-A**, filters by author
- **-s [open|closed|all]**, filters by state
    - on default, is "open"
- **-l** filters by label  

#### gh pr status
shows status of PRs  

#### gh pr view (number | url | branch)  
view specific pr
- **-c** displays comments  

#### gh pr checkout (number | url | branch)  
checkout pull request  

#### gh pr merge (number | url | branch) 
merges pull request  

#### gh pr diff (number | url | branch) 
display changes in pr  

#### gh pr close (number | url | branch)  
closes pr  
- **c** leaves closing comment
- **d** deletes branch upon closing

#### gh pr reopen (number | url | branch)
reopens closed pr
- **-c** leaves closing comment  
