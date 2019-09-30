# gitFlow

gitFlow is a set of guidelines that developers can follow when using [version control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control). It is also referred to as a branching model. gitFlow works around a Central repository. Developers in a team can clone the central repository and then work locally. 

The four branches in the gitFlow process are :

1. Master Branch

2. Develop Branch

3. Release Branch

4. Hotfix Branch

## How it works

The **Master branch** stores official release history

The **Develop branch** serves as an integration branch of features for developers to work on.

We will create a develop branch from the master branch and this develop branch, is the branch in which the team will work on.

<img src="Screenshots/gitFlow.png" width="300">

## Adding a feature

We start off by forking the develop branch and creating a separate feature branch. All changes to be done would be done on this new feature branch.
The developers will commit their work to the feature branch. Once testing is done, the feature branch is merged back into the develop branch.

## Testing the Stability

The develop branch is an unstable branch as new features are constantly added on to it. The testing takes place in the Release branch.
The Release branch is created by forking the latest copy of develop branch. The Release branch will contain a pre-determined amount of features. Testing is done on the release branch to see if it is stable.

## Merging to the Master branch

Once the testing is complete and the release branch is stable, the Release branch is merged into the develop branch and the master branch. Every time a branch is merged into master, we add a version number. This helps  tracking releases and see the history of the project.

## Hotfix Branch

Hot fixes are minor fixes such as spellings or labels that need to be changed. The master branch is forked to create a new hotfix branch. Commits are made to the hotfix branch to fix the errors. Once the issue is resolved, it is merged back into the master branch and develop branch. It is important to tag the master branch with a version number after merging.

# Learning Git

[Repository](repository.md)

[Clone](clone1.md)

[Fork](fork.md)

[Branch](branch.md)

[Commit](commit.md)

[Merge](merge.md)

[Checkout](checkout.md)

[Push](push.md)

[Pull](pull.md)

Remote Add / Remove / Show

[Status](status.md)

[Master Branch](masterbranch.md)
