# Contributing

PRs to this repo are welcome!

Assuming you are wanting to change the code climate configs, to do this you'll do something like the following:

1. `cd code-climate-configs/drupal8-core`
1. Make your changes to the `.codeclimate.yml` or other files.
1. Make a commit.
1. Create a patch by running this inside the `code-climate-configs/drupal8-core` directory:

  ```
  git diff d23cd9e0d3c5b1c4a1962eb9353c7649c2d69bab..HEAD --relative > ../0001-Add-Drupal-8-core-Code-Climate-config.patch
  ```

Note: the reason for using the `d23cd9e0d3c5b1c4a1962eb9353c7649c2d69bab` commit is to create a diff of all time, which is what we want: a patch that someone can `wget` and apply to their project.

