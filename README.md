# PROJECT UPDATES

## TL; DR

Commits should be logical, atomic usnits of change that only empass one task or one fixt whose purpose can be clearly desribed in the commit message. 

## Issues Log
An issues log track bugs, improvements, feature requests and planned updates. 

Changes made to repository files myst be put into the project issues log first. Issue Log ID values are used in the Branch Name to allow reference back to a more detailed explanation of the requirement for making the commit. 



## Branching Strategy
The project maintains a single production version and focuses on small iterative updates deployed directly to the main branch. It uses the [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow) branching strategy where:

 - The main branch is always the current production version,
 - All changes are made through feature branches (pull-request + merge)
 - ```hotfixes``` and ```tests``` are treated the same as ```features```

| Branch        | Protected | Base Branch    | Description                                                                    |
|:--------------|:----------|:---------------|:-------------------------------------------------------------------------------|
| ```main```    | Yes       | Not Applicable | Production version.<br> A pull request is required to merge code into the main |
| ```feature``` | No        | main           | Used for feature development and testing                                       |
| ```hotfix```  | No        | main           | Maintenance or hotfix branches are used to quickly patch production releases   |
| ```test```    | No        | main           | Used for testing outside of any specific project issue                         |



https://gist.github.com/jbenet/ee6c9ac48068889b0912 (# commit your (incremental, atomic) changes)



## Naming Conventions

## Versioning


https://www.esri.com/arcgis-blog/products/js-api-arcgis/developers/rest-is-up-to-the-task/
https://community.esri.com/t5/arcgis-javascript-maps-sdk-questions/not-able-to-access-feature-layers/td-p/1227023

## Commit Message Format

Each commit message consists of a header, a body and a footer 

Header
Headers are mandatory and must conform to the Commit Message Header format


Commit Message Header
```
<type>[optional scope]: <short description>
  │       │             │
  │       │             └─⫸ Short summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Noun describing a section of the codebase surrounded by parenthesis, e.g., fix(parser):
  │
  └─⫸ Commit Type: feat|fix|refactor|chore
```


