# PROJECT UPDATES

## TL; DR

Branches are tied to a specific issue


Commits should be logical, atomic units of change that only encompass one task or one fix whose purpose can be clearly described in the commit message. 

## Issues Log
An issues log track bugs, improvements, feature requests and planned updates. 

Changes made to repository files must be put into the project issues log first. Issue Log ID values are used in the Branch Name to allow reference back to a more detailed explanation of the requirement for making the commit. 

## Branching Strategy
The project maintains a single production version and focuses on small iterative updates deployed directly to the main branch. It uses the [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow) branching strategy where:

 - The main branch is always the current production version,
 - All changes are made through feature branches (pull-request + merge),
 - ```hotfixes``` and ```tests``` branches are treated the same as a ```features``` branch

### Branch types

| Branch        | Protected | Base Branch    | Description                                                                    |
|:--------------|:----------|:---------------|:-------------------------------------------------------------------------------|
| ```main```    | Yes       | Not Applicable | Production version.<br> A pull request is required to merge code into the main |
| ```feature``` | No        | main           | Used for feature development and testing                                       |
| ```hotfix```  | No        | main           | Maintenance or hotfix branches are used to quickly patch production releases   |
| ```test```    | No        | main           | Used for testing outside of any specific project issue                         |


### Branch Naming Convention
```
git branch <category>/<reference>/<short description-in-kebab-case>

                │          │              │
                │          │              │
                │          │              └─⫸ Short summary. Lowercase. Hyphens, no spaces.
                │          │ 
                │          └─⫸ Issue number prefixed with a hash (#), else no-ref.
                │
                └─⫸ Branch Type: feature|hotfix|test.
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



