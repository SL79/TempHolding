# PROJECT UPDATES

## TL; DR

Branches are tied to a specific issue

Commits should be logical, atomic units of change that only encompass one task or one fix whose purpose can be clearly described in the commit message. 

## Issues Log
An issues log track bugs, improvements, feature requests and planned updates. 

Changes made to repository files must be put into the project issues log first. Issue Log ID values are used in the Branch Name to allow reference back to a more detailed explanation of the requirement for making the commit. 

## Branching Strategy

The project leverages [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow) for streamlined code management and effective version control. The main branch serves as the production version, with all development work taking place in a single branch directly off the main. 

The project only supports two active branches: a main and a single development branch. The development branch is related to a specific project issue (excluding required maintenance work).

### Branch types

The following branch types are used for this project.

| Branch            | Protected | Base Branch    | Description                                                                    |
|:------------------|:----------|:---------------|:-------------------------------------------------------------------------------|
| ```main```        | Yes       | Not Applicable | Production version.<br> A pull request is required to merge code into the main |
| ```feature```     | No        | main           | Used for feature development and testing                                       |
| ```hotfix```      | No        | main           | Used to quickly patch production releases                                      |
| ```test```        | No        | main           | Used for testing a specific project issue                                      |
| ```maintenance``` | No        | main           | Used for undertaking maintenance tasks outside any specific project issue      |


### Branch Naming Convention
```
git branch <category>/issue-<issue id>/<short description-in-kebab-case>

                │          │              │
                │          │              │
                │          │              └─⫸ Short summary. Lowercase. Hyphens, no spaces.
                │          │ 
                │          └─⫸ no-ref to replace issue-<issue id> if the the branch type is maintenance. 
                │
                └─⫸ Branch Type: feature|hotfix|test|maintenance.
```

## Commits


## Commit Message Format

Each commit message consists of a header, a body and a footer 

Header
Headers are mandatory and must conform to the Commit Message Header format


Commit Message Header
```
<type>[optional scope]: <short description>

  │         │                   │
  │         │                   └─⫸ Short summary in present tense. Lowercase. No period at the end.
  │         │
  │         └─⫸ Noun describing a section of the codebase surrounded by parenthesis, e.g., fix(parser):
  │
  └─⫸ Commit Type: feat|fix|refactor|chore
```




## Pull Requests








https://gist.github.com/jbenet/ee6c9ac48068889b0912 (# commit your (incremental, atomic) changes)





## Versioning


https://www.esri.com/arcgis-blog/products/js-api-arcgis/developers/rest-is-up-to-the-task/
https://community.esri.com/t5/arcgis-javascript-maps-sdk-questions/not-able-to-access-feature-layers/td-p/1227023



