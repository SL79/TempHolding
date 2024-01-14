# PROJECT UPDATES

## TL; DR

Commits should be logical, atomic usnits of change that only empass one task or one fixt whose purpose can be clearly desribed in the commit message. 

## Issues Log
An issues log track bugs, improvements, feature requests and planned updates. 

Changes made to repository files myst be put into the project issues log first. Issue Log ID values are used in the Branch Name to allow reference back to a more detailed explanation of the requirement for making the commit. 

## Branching Strategy
The project uses [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow), employing the main branch with feature branches used for development and testing, which are then merged bacn into the via pull requests. 

 - The main branch is always the current production version,
 - ```hotfixes``` and ```tests``` are treated the same as ```features```

| Branch        | Protected | Base Branch    | Description                                                                    |
|:--------------|:----------|:---------------|:-------------------------------------------------------------------------------|
| ```main```    | Yes       | Not Applicable | Production version.<br> A pull request is required to merge code into the main |
| ```feature``` | No        | main           | Used for feature development and testing                                       |
| ```hotfix```  | No        | main           | Maintenance or hotfix branches are used to quickly patch production releases   |
| ```test```    | No        | main           | Used for testing outside of any specific project issue                         |


Certainly! GitHub Flow is a lightweight, branch-based workflow that many development teams use for managing and deploying code. Here's a summary of the GitHub Flow branching strategy:

 - Create a Branch:
Start by creating a branch for a new feature or bug fix. This branch is usually based on the main or master branch.
 - Add Commits:
Make changes and commit them to your branch. Each commit represents a set of changes related to the feature or bug fix.
 - Open a Pull Request:
Once you're done with the changes, open a pull request (PR). A pull request is a request to merge your changes into the main or master branch.
 - Discuss and Review:
Team members can review your code, leave comments, and discuss the changes within the pull request. This facilitates collaboration and ensures code quality.
 - Make Changes:
If there are suggested changes or feedback, make the necessary adjustments in your branch and push the changes. The pull request will be automatically updated.
 - Merge Pull Request:
Once the changes are approved, the pull request can be merged into the main or master branch. This integrates your changes with the rest of the codebase.
 - Deploy:
After the merge, the code is ready to be deployed. The GitHub Flow encourages frequent and small releases, making it easier to manage and identify potential issues.
 - Cleanup:
After the code is merged and deployed, you can delete the branch. This keeps the repository clean and makes it easier to track active branches.

Key points of GitHub Flow include its simplicity, emphasis on small and frequent releases, and collaboration through pull requests. It's particularly well-suited for projects with continuous delivery and a need for quick iterations.







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


