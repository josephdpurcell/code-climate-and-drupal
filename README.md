# Code Climate and Drupal

Code Climate is a free open source static analysis platform that is a great fit for Drupal core and contrib development, as well as Drupal projects. It can be used as a workflow tool to surface problems with code contributions, audit existing code for vulnerabilities or problematic code, or evaluate new or legacy projects.

Currently, I've identified in the [How To's](docs/how-tos.md) a few examples of how to use Code Climate with Drupal which focus solely on PHP Code Sniffer (PHPCS) and PHP Mess Detector (PHPMD). While PHPCS is less controversial since it is using the [Drupal Coder](https://www.drupal.org/project/coder) project. However, PHPMD is not configured out of the box to what the Drupal community would consider in alignment with best practices. As such, the examples below use a custom PHPMD configuration file according to my best guess as to what I think is a reasonable start [see config here](code-climate-configs/drupal8-core/.phpmd.xml), with a hope it can evolve into aligning with more well adopted checks. It is worth noting these examples focus solely on PHP--revising the configuration for JS and CSS standards would be a win.

# Resources

* [Persuasive Essay](persuasive-essay.md)
* [How Tos](docs/how-tos.md)
* [Example Projects](docs/example-projects.md)
* [Code Climate config examples](code-climate-configs/README.md)

# Getting Started

To get started using Code Climate on your Drupal project or contrib module:

1. Grab the right patch for the Code Climate config from [code-climate-configs/README.md].
1. Apply the patch to your repository like: `git am --signoff < 0001-THE-PATCH.patch`
1. Push the code to your GitHub repository. (Currently, Code Climate is free only for github.com)
1. Go to [codeclimate.com](https://codeclimate.com/) and add your repository.
1. Go to the repo on Code Climate, click "Integrations", click "GitHub Pull Requests" to enable the checks to show up on each pull request.

# Roadmap

Below is a rough sketch of what adoption of Code Climate might look like:

* Validate people can use these Code Climate configs to get started.
* Validate the PHPMD config is reasonable with other Drupalers.
* Identify Drupal projects and modules that can adopt Code Climate into their workflow to give feedback on the use of PHPMD and PHPCS.
* Expand the checks to include theming-related checks, e.g. JS and CSS.
* Once the Code Climate checks are affirmed by at least a portion of the community, make a recommendation to the [Drupal Technical Working Group](https://groups.drupal.org/node/510675) to provide these Code Climate configs for core, contrib, and the public to use.
* Involve the , see also [guidelines](https://www.drupal.org/project/coding_standards)

* Violations of these checks are made available per-patch in the issue queue.
* GPAs of core and contrib are published on drupal.org.

**Assumption:** Code Climate provides support for the 'drupal.org' domain.

# Wish List

* Add security sniffs to these configs we're standardizing on. (Maybe [Drupal Security Sniffs](https://www.drupal.org/sandbox/coltrane/1921926) or [issue](https://www.drupal.org/node/1844870) or [FloeDesignTechnologies/phpcs-security-audit](https://github.com/FloeDesignTechnologies/phpcs-security-audit))
* See how current issues on the TWG or infrastructure issue queues are related and perhaps make a suggestion there once this is mature, e.g. [drupal.org/node/1299710](https://www.drupal.org/node/1299710).
* Add documentation on what the PHPMD configs mean.

