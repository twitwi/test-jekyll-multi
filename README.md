# Experimenting with technical aspects of lesson release

This repo is an experiment for lesson release.
It actually aggregates a set of lessons.

There would be one such repository per release.



## Using git submodules

Git submodules have been often discussed.
I think they can be used for the release process as we are not asking all instructors to know how to do a release.

Git submodules are leveraged to achieve multiple goals:
- aggregating lessons in a single place (single repository),
- for each lesson, selecting and freezing the version to release (git commit),
- having Jekyll (github pages) hosts each lesson with this specific version.


## Viewing the example site

[http://twitwi.github.io/test-jekyll-multi-swc-4.3-fake/](view the site)

For this example, an index is added, but the swc website could act as such index too.

In this example:
- the last version of the shell lesson has been taken,
- version v5.3 of the git lesson is used, one can see the (subtle) differences between the two versions:
    - http://twitwi.github.io/test-jekyll-multi-swc-4.3-fake/git-novice/01-basics.html
    - http://swcarpentry.github.io/git-novice/01-basics.html



## Discussion

### In a broader context of lesson releases

This one-aggregating-repo-per-release approach puts no constraint on the lesson repositories.
More precisely, it would fit well in a workflow where the lessons have a single branch (gh-pages).
This way we avoid PR made on the wrong branch.

### Backward compatibility issue?
While doing this experiment, I realized a potential long-term issue (or a reason to actually rather generate the HTML files and host them): if Jekyll gets updated, in a non backward-compatible manner, 

