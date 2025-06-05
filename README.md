# ci-data
holding test data for ldmx-sw CI

This repository should not be interacted with manually.

## Updates
The "Generate PR Gold" workflow of ldmx-sw that is run on every release
is what updates this repository.
After generating the golden histogram and log files, it copies them
into their locatins in this repository and then forcibly **amends**
the `HEAD` commit.
This means there is no history in this repository, which was done
in order to save space and easy cloning time.

If you do need to interact with this repository manually (perhaps to
run the CI tests locally or manually update the golden histograms after
a failure), you should **not** `git pull` this repository. There _will_
be confusing conflicts if you do that. Instead, just remove an old clone
and run `git clone` again.
