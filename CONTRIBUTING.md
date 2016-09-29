# Contributing

PRs to this repo are welcome!

Assuming you are wanting to change the code climate configs, to do this you'll do something like the following:

1. `cd code-climate-configs/drupal8-core`
1. Make your changes to the `.codeclimate.yml` or other files.
1. Make a commit.
1. Create a patch by running this inside the `code-climate-configs/drupal8-core` directory:

  ```
  git format-patch --stdout --relative HEAD~1 > ../0001-Add-Drupal-8-core-Code-Climate-config.patch
  ```

Note: the `git format-patch` command assumes the latest commit was only the files changed in the `code-climate-configs/drupal8-core` directory, or whichever directory you're making changes to.

