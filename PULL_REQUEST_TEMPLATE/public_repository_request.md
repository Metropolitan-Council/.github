# Repository visibility change request - private/internal to public

## Request details

Please answer the following questions with sufficient detail. All sections must be filled out. 

### Describe the purpose of the code

### Describe the need for making it public

<!-- Is this code to be shared with external collaborators? -->

### Describe security risks to the Council if malicious code were injected into the repo (worst case scenario)

### Does the repository contain only documentation or example code?

<!-- Are all the public functions fully documented?-->

### Do we use the code internally?

<!-- Is the code used in any automated processes onsite? -->

### Is the code for a mission critical application?


### Describe precautions taken to mitigate risk

<!--Pull-request review process, automated or manual testing procedures, access and push restrictions. Use checklist.-->

### Describe expected level of outside interaction 

<!-- Popularity, issues, pull-requests from general public or potential collaborators -->

### Checklist 

Use the checklist below to track your progress on these items, particularly those that have to be done manually through GitHub. Add to the checklist if you complete additional steps

- [ ] Primary repository branch is named "main"
- [ ] Branch "main" [protected](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches).
- [ ] Only specifically noted users (tag users using @) have [push privileges](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository) on any branch
- [ ] Pull-request required before merging to "main"
- [ ] At least one approval needed from maintainers (tag maintainers using @) before pull-requst merge
- [ ] Conversations and change requests must be resolved before pull-request merge
- [ ] Comprehensive README included [README.MD](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [ ] Repository content reviewed for typos, grammar, and other inconsistencies
- [ ] Repository git history is clean: no sensitive data commited and later removed from repository
- [ ] *Contributing or style guide included [CONTRIBUTING.MD](CONTRIBUTING.MD)
- [ ] *Issue and pull-request templates included. See GitHub [documentation](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates) for more detais. 
- [ ] *Code of conduct included [CODE_OF_CONDUCT.MD](CODE_OF_CONDUCT.MD)
- [ ] *Automated testing with GitHub Actions or other CI/CD tool (describe)

*optional 


## Repository requirements

1.	The repository must be clean
	- No absolute paths; all paths must be relative to project root directory
    - No API keys, passwords, credentials, or other “secrets” in plain text. 
    - Scan for secrets with [Talisman](https://thoughtworks.github.io/talisman/) and remove secrets
    - If secrets exist in the git history, consider using a tool like [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/) or create a new repository and copy/paste all materials (excluding .git/).
1.	The code must meet professional standards
    - All commit messages, code comments and other documentation are professional and informative. If there are substandard commit messages in the git history, consider creating a new repository and copy/pasting all materials (exlcuding .git/).
    - A .gitignore file is required, and should at a minimum contain
        ```gitignore
            .*
            !.gitignore
        ```
    - All code should be documented, at a minimum describing what the code does, and a description of parameters, returned values and side-effects.
1.	The code must have an approved OSS license, e.g., [MIT](https://spdx.org/licenses/MIT.html), [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0), [BSD-3](https://spdx.org/licenses/BSD-3-Clause.html), with the Metropolitan Council as the license holder.
	- Data or documentation repositories should have an appropriate data license, e.g., [PDDL-1.0](https://opendatacommons.org/licenses/pddl/1-0/), [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/), [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).
    - Public domain dedications (CC0, PDDL) relinquish all rights and are usually what we intend when we publish data, but you may find it appropriate in some conditions to maintain copyright and requesting minimal attribution.
    - License should have a [Blue Oak Council](https://blueoakcouncil.org/list) rating of Gold, Silver, or Bronze.
    - If a license other than MIT, Apache 2.0, or BSD-3 is used, describe why in the request. 
    - If a license holder other than the Metropolitan Council is listed, explain why and reference any relevant contracts or agreements. 
1.	A README.md file describes the purpose of the project
1.	Add appropriate branch protection to the main branch

## Steps to approval

- [ ] If organizational risk is **not** considered low, forward this request as an email to IS security via the ServiceDesk.
- [ ] Your manager must approve this pull-request. If they are on GitHub, [request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review) from them. If your manager is not on GitHub, they can approve by sending an email to a repo admin, who can then add the contents of the email to the pull-request and approve on their behalf. 
- [ ] Once approved, request a GitHub admin make the repo public. 

(tag manager with @), we request your review on this repository. If you approve making this repository public, please approve the pull-request.


