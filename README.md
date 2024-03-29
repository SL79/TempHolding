# PROJECT UPDATES

## TL; DR

 - All development work is to be raised as an issue first
 - Branches are tied to a specific issue (general maintenance tasks excluded)
 - Commits should be logical, atomic units of change that only encompass one task or fix whose purpose can be clearly described in the commit message.

## Issues Log
Issues are used to track ideas, tasks, planned updates or bugs for project work. 

Required changes must be raised as a project issue first. Issue ID numbers are used in branch names to allow reference back to a more detailed explanation of the requirement.

## Branching Strategy

The project leverages [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow) for streamlined code management and effective version control. The main branch serves as the production version, with all development work taking place in a single branch directly off the main. 

The project only supports two active branches: a main and a single development branch. The development branch is related to a specific project issue (excluding required maintenance work).

### Branch types

The following branch types are used for this project.

| Branch            | Protected | Base Branch    | Description                                                                                             |
|:------------------|:----------|:---------------|:--------------------------------------------------------------------------------------------------------|
| ```main```        | Yes       | Not Applicable | Production version.<br> A pull request is required to merge code into the main                          |
| ```feature```     | No        | main           | Used for developing new features                                                                        |
| ```bugfix```      | No        | main           | Used to fix bugs in the code                                                                            |
| ```maintenance``` | No        | main           | Used for undertaking maintenance tasks outside any specific project issue, <br> inlcuding documentation |

https://medium.com/@abhay.pixolo/naming-conventions-for-git-branches-a-cheatsheet-8549feca2534

### Branch Naming Convention
```
git branch <category>/issue-<issue id>/<short description-in-kebab-case>

                │          │              │
                │          │              │
                │          │              └─⫸ Short summary. Lowercase. Hyphens, no spaces.
                │          │ 
                │          └─⫸ no-ref to replace issue-<issue id> if the branch type is maintenance. 
                │
                └─⫸ Branch Type: feature|bugfix|maintenance.
```

## Commits
The project uses conventional commits message format. 
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```


### Commit categories

https://medium.com/front-end-weekly/how-to-write-good-git-commit-messages-like-a-pro-2c12f01569d9

| Category        | Type          | Description                                                                                   |
|:----------------|:----------|:--------------------------------------------------------------------------------------------------|
| ```feat```      | Feature   | Adding a new feature                                                                              |
| ```fix```       | Fix       | Fixing a bug or issue                                                                             |
| ```refractor``` | Refractor | Changes made for peformance or convenience purpose (e.g. readibility)                             |
| ```chore```     | Chore     | Miscellaneous (non-production) commits e.g: <br><ul><li>modifying .gitignore</li><li>changes to documentation</li><li>style changes (formatting, missing semi colons, etc;)</li> <li>adding tests</li>|

### Commit Message Format

Each commit message consists of a header, an optional body and an optional footer 

#### Header
Headers are mandatory and must conform to the Commit Message Header format: ```<type>[optional scope]: <description>```.  

The <b>type</b> value is a short prefix that represents the <b>kind</b> of change. The optional <b>scope</b> represents the <b>context</b> of the change, while the <b>subject</b> repesents a concise <b>description</b> of the actual change.

Commit Message Header
```
<type>[optional scope]: <description>

  │         │                   │
  │         │                   └─⫸ Short summary in present tense (description of actual change). Lowercase. No period at the end. Max 100 characters
  │         │
  │         └─⫸ Noun describing a section of the codebase surrounded by parenthesis (context of change)
  │
  └─⫸ Commit Type: feat|fix|refactor|chore
```

Example: 
```
git commit -m "fix(core): remove deprecated and defunct wtf* apis"
```


#### Body
The body is optional lines that introduce the motivation behind the change or just describing slightly more detailed information.
 - The header and body are to be separated by a blank line 

```
git commit -m "fix(core): remove deprecated and defunct wtf* 
apis" -m "These apis have been deprecated in v8, so they should stick around till v10, but since they are defunct we are removing them early so that they don't take up payload size."
```

#### Footer
The footer is optional lines that mention consequences which stems from the change — such as announcing a breaking change, linking closed issues, mentioning contributors and so on.

## Pull Requests








https://gist.github.com/jbenet/ee6c9ac48068889b0912 (# commit your (incremental, atomic) changes)





## Versioning


https://www.esri.com/arcgis-blog/products/js-api-arcgis/developers/rest-is-up-to-the-task/
https://community.esri.com/t5/arcgis-javascript-maps-sdk-questions/not-able-to-access-feature-layers/td-p/1227023



