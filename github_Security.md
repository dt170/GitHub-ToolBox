
# Keep your security 

Have you ever thought on security when upload your personal project to github ? well if you do you came in to the right place.

As a developer / computer science student you find your self uploading many projects as time passing by to github, those files may include sensitive information which can cause in some of the cases to security breach or overcharges that will cost you $$$. 
I'm going to give two easy examples as a developers we find our self's many time using API's to get the necessary information for our project which most of the time limit the free requests when uploading the project files with the API information others users may use your link and cause your bill to overcharge. 
another important case is passwords managing saving password in a file, unprotected DB and more. 

#### So what can we do ?! 

### Removing sensitive data from a repository

If you commit sensitive data, such as a password or SSH key into a Git repository, you can remove it from the history. To entirely remove unwanted files from a repository's history you can use either the `git filter-branch` command or the `BFG Repo-Cleaner` open source tool.

* [Github docs - removing sensitive data](https://docs.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository)
* [BFG github project](https://github.com/rtyley/bfg-repo-cleaner)
* [BFG main documentation](https://rtyley.github.io/bfg-repo-cleaner/)

### Prevention

Never store credentials as code/config in GitHub in the first place, furthermore using `git-secrets`,CI/CD tools like `Jenkins`, that can statically analyze your commits, via a pre-commit `Git Hook` to ensure you’re not trying to push any passwords or sensitive information into your GitHub repository.Commits will be rejected if the tool matches any configured regular expression patterns that are designed to find sensitive information. It may slow down pushes a tiny bit, but it’s well worth it.There are many ways to avoid putting credentials into your repository in the first place, and you should try to implement as many as you can, but there’s always the chance some sensitive information may sneak in. You should also consider regular auditing of your repos, making use of tools like GitRob or truffleHog, both of which scan through your codebase, searching for sensitive information via pattern matching.

* [Jenkins](https://www.jenkins.io/)
* [git-secret.io](https://git-secret.io/)
* [git-secrets repo](https://github.com/awslabs/git-secrets)
* [git-Hooks](https://githooks.com/)

### Rotate keys and Access Tokens
GitHub access is typically done using SSH keys or personal user tokens (in lieu of a password, because you enabled 2FA!). But what happens if those tokens are stolen and you didn’t know? Be sure to refresh your keys and tokens periodically, mitigating any damage caused by keys that leaked out.
another thing is when using API you get a uniqe key which in most cases you can refresh and change him after uploading the project change the key to prevent overcharge.

### Add a SECURITY.md file

when adding security.md file into your project you force your self to think on security. write in the file the breaches you found and need to be fix this may help other users that may use your code in their project/company and prevent a bigger data breach in the future. furthermore other contributors may help you solve those issues when come across your security file remember every problem you came across there is a high chance someone else already solve it.  


got the inspiration from [snyk](https://snyk.io/blog/ten-git-hub-security-best-practices/)
