# Repository visibility change request - private/internal to public

## Request details

Please answer the questions in **bold** with sufficient detail. All sections must be filled out. 

**Describe the purpose of the code**

**Describe the need for making it public** 

**Describe security risks to the Council if malicious code were injected into the repo (worst case scenario)**

**Does the repository contain only documentation or example code?**

**Do we use the code internally?** 

**Is the code for a mission critical application?**

**Describe precautions taken to mitigate risk (pull-request review, testing, & etc.)**

Use the checklist below to track your progress on these items. Add to the checklist if you complete additional steps

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

**Describe expected level of outside interaction (popularity, issues, pull-requests)**

## Repository requirements

1.	The repository must be clean
	  - No absolute paths; all paths must be relative to project root directory
    - No API keys, passwords, credentials, or other “secrets” in plain text. 
    - Scan for secrets with [Talisman](https://thoughtworks.github.io/talisman/) and remove secrets
    - If secrets exist in the git history, consider using a tool like [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/) or create a new repository and copy/paste all materials (excluding .git/)
1.	The code must meet professional standards
    - All commit messages, code comments and other documentation are professional and informative.
    - A .gitignore file is required, and should at a minimum contain:
      - .*
      - !.gitignore
    - All code should be documented, at a minimum describing what the code does, and a description of parameters, returned values and side-effects.
1.	The code must have an approved OSS license, e.g., MIT, Apache-2.0, BSD-3, with the Metropolitan Council as the license holder.
	  - Data or documentation repositories should have an appropriate data license, e.g., PDDL-10, CC0-1.0, CC-BY-4.0.
    - Public domain dedications (CC0, PDDL) relinquish all rights and are usual what we intend when we publish data, but you may find it appropriate in some conditions to maintain copyright and requesting minimal attribution.
    - If a license other than MIT or Apache 2.0 is used, describe why in the request. 
 - Approved licenses are defined in Tech 3-4: Code and Data Licensing Policy
1.	A README.md file describes the purpose of the project
1.	Add appropriate branch protection to the main branch

## Manager approval

If organizational risk is considered low, no further approval required. Otherwise, forward this request as an email to IS security via the ServiceDesk.

(tag manager with @), we request your review on this repository. If you approve making this repository public, please approve the pull-request.

Once approved the Metropolitan-Council GitHub organization admin or other Council employee with the appropriate GitHub role will change the repository visibility to "Public".
