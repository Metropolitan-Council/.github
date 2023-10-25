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
- [ ] Branch "main" protected
- [ ] Only specifically noted users (tag users using @) have push privileges to repo on any branch
- [ ] Pull request required before merging to "main"
- [ ] At least one approval needed from maintainers (tag maintainers using @) before pull-requst merge
- [ ] Conversations and change requests must be resolved before pull-request merge
- [ ] Comprehensive README included [README.MD](README.MD)
- [ ] Repository content reviewed for typos, grammar, and other inconsistencies
- [ ] Repository git history is clean: no sensitive data commited and later removed from repository
- [ ] *Contributing or style guide included [CONTRIBUTING.MD](CONTRIBUTING.MD)
- [ ] *Pull request template included [PULL_REQUEST_TEMPLATE.MD](.github/PULL_REQUEST_TEMPLATE.MD)
- [ ] *Code of conduct included [CODE_OF_CONDUCT.MD](CODE_OF_CONDUCT.MD)
- [ ] *Automated testing (describe)

*optional 


## Repository requirements

1.	The repository must be clean
	- No absolute paths; all paths must be relative to project root directory
    - No API keys, passwords, credentials, or other “secrets” in plain text. 
    - Scan for secrets with [Talisman](https://thoughtworks.github.io/talisman/) and remove secrets
    - If secrets exist in the git history, consider using a tool like [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/) or create a new repository and copy/paste all materials (excluding .git/)
1.	The code must meet professional standards
    - All commit messages, code comments and other documentation are professional and informative. If there are substandard commit messages in the git history, consider creating a new repository and copy/pasting all materials (exlcuding .git/).
    - A .gitignore file is required, and should at a minimum contain
        ```gitignore
            .*
            !.gitignore
        ```
    - All code should be documented, at a minimum describing what the code does, and a description of parameters, returned values and side-effects.
1.	The code must have an approved OSS license, e.g., MIT, Apache-2.0, BSD-3, with the Metropolitan Council as the license holder.
	- Data or documentation repositories should have an appropriate data license, e.g., PDDL-10, CC0-1.0, CC-BY-4.0.
    - Public domain dedications (CC0, PDDL) relinquish all rights and are usual what we intend when we publish data, but you may find it appropriate in some conditions to maintain copyright and requesting minimal attribution.
    - License should have a [Blue Oak Council](https://blueoakcouncil.org/list) rating of Gold, Silver, or Bronze.
    - If a license other than MIT or Apache 2.0 is used, describe why in the request. 
1.	A README.md file describes the purpose of the project
1.	Add appropriate branch protection to the main branch

## Manager approval

If organizational risk is considered low, no further approval required. Otherwise, forward this request as an email to IS security via the ServiceDesk.

(tag manager with @), we request your review on this repository. If you approve making this repository public, please approve the pull-request.

Once approved the Metropolitan-Council GitHub organization admin or other Council employee with the appropriate GitHub role will change the repository visibility to "Public".

