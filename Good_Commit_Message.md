# How to write a good commit message 
inspired from [chrissiemhrk](https://dev.to/chrissiemhrk/git-commit-message-5e21)

<b>What is a commit?</b> 

A commit message is a short description of the changes you've made to a file added before committing the changes.

<b>What is a good commit?</b>

Good commit messages are important not only for others who you may be collaborating on the project but also for you, 
to keep track of all your commits and knowing exactly what changes where maybe during that particular commit.


## Template:

| Subject | feat: Create new navigation bar  | 
| ------- | ------- |
| <b>Description</b> | explain what changes you made and why you made them |

<b>Note:</b> Not all commits are complex enough that they need a Description, 
especially if you are working on a personal project alone, and as such writing a body is optional.

### Subject options
You may use Text or emojis, An easy way to put the emoji is using shortcuts:
* For WINDOWS user Press `WIN + ;` 
* For MAC user Press `Command + Control + Space`

# Option 1

| Text | Use them |
| ---- | ---- |
| feat|a new feature|
|fix|a bug fix|
|docs|changes in documentation|
|style|everything related to styling|
|refactor|code changes that neither fixes a bug or adds a feature|
|test|everything related to testing|
|chore|updating build tasks, package manager configs, etc|

# Option 2

| Code | Emoji | Use them |
| ---- | ----- | ---- |
| `:heavy_plus_sign:`|➕|when adding a file or implementing a feature|
|`:hammer:`|🔨|when fixing a bug or issue|
|`:green_heart`|💚|when improving code or comments|
|`:zap:`|⚡|when improving performance|
|`:scroll:`|📜|when updating docs or readme|
|`:key:`|🔑|when dealing with security|
|`:repeat:`|🔁|when updating dependencies or data|
|`:white_check_mark:`|✅|when a new release was built|
|`:shirt:`|👕|when refactoring or removing linter warnings|
|`:x:`|❌|when removing code or files|

# Option 3

| Code | Emoji | Use them |
| ---- | ----- | ---- |
| `:tada:`|🎉|when doing initial commit|
|`:rocket:`|🚀|when implementing a new feature|
|`:hammer:`|🔨|when fixing a bug or issue|
|`:art:`|🎨|when refactor/improving code|
|`:scroll:`|📜|when updating docs or readme|
|`:pencil:`|📝|when doing some small updates|



You may use other emoji or text to mark your commits but try to make them as clear as you can for other to view and understand.

