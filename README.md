# Code Climate and Drupal

Code Climate is a free open source static analysis platform that is a great fit for Drupal core and contrib development, as well as Drupal projects. It can be used as a workflow tool to surface problems with code contributions, audit existing code for vulnerabilities or problematic code, or evaluate different projects.

For more information on why Code Climate is a good fit for Drupal, read the [persuasive essay](persuasive-essay.md).

# Examples

The following examples use the PHPCS sniffs supported by their respective communities, and the same phpmd file. The result should be a somewhat objective comparison of how each code base meets its own code style, as well as the checks from PHPMD, such as complexity or unused variables.

Note: these GPA's are likely out of date, so verify the commit Code Climate has matches with the latest commit.

## Drupal

* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-7.x/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-7.x) [GitHub fork for drupal/drupal:7.x](https://github.com/josephdpurcell/drupal-7.x)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal) [GitHub fork for drupal/drupal:8.1.x](https://github.com/josephdpurcell/drupal)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-8.2.x/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-8.2.x) [GitHub fork for drupal/drupal:8.2.x](https://github.com/josephdpurcell/drupal-8.2.x)

## Drupal Modules

* [![Code Climate](https://codeclimate.com/github/josephdpurcell/workbench_moderation/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/workbench_moderation) [GitHub fork for drupal/workbench_moderation:8.x-1.x](https://github.com/josephdpurcell/workbench_moderation)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-multiversion/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-multiversion) [GitHub fork for drupal/multiversion:8.x-1.x](https://github.com/josephdpurcell/drupal-multiversion)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-deploy/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-deploy) [GitHub fork for drupal/drupal-deploy:8.x-1.x](https://github.com/josephdpurcell/drupal-deploy)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-replication/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-replication) [GitHub fork for drupal/drupal-replication:8.x-1.x](https://github.com/josephdpurcell/drupal-replication)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-relaxed/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-relaxed) [GitHub fork for drupal/drupal-relaxed:8.x-1.x](https://github.com/josephdpurcell/drupal-relaxed)

## Other

* [![Code Climate](https://codeclimate.com/github/josephdpurcell/symfony/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/symfony) [GitHub fork for symfony/symfony:master](https://github.com/josephdpurcell/symfony)
* [![Code Climate](https://codeclimate.com/repos/5730fdf0d132d84858004be5/badges/9503049144363360d9c2/gpa.svg)](https://codeclimate.com/repos/5730fdf0d132d84858004be5/feed) [GitHub fork for wordpress/wordpress:master](https://github.com/josephdpurcell/wordpress) ...is this number right???

# How To's

## Add Code Climate Config to Drupal 7 Core

```
wget https://gist.githubusercontent.com/josephdpurcell/c4c5bb42bb8f4dd75b0cdaf41e2a023e/raw/9205838037a2ee6f62a69962a0252f6b8ec3f7c7/0001-Add-.codeclimate.yml-for-Drupal-7-core.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-7-core.patch
```

See [gist here](https://gist.github.com/josephdpurcell/c4c5bb42bb8f4dd75b0cdaf41e2a023e).

## Add Code Climate Config to Drupal 8 Core

```
wget https://gist.githubusercontent.com/josephdpurcell/a57bc443b58c7c1ca547e5a7b067ff30/raw/2d05db503001af1a90d2d40a9270e0c5fb8c50a2/0001-Add-.codeclimate.yml-for-Drupal-8-Core.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-8-Core.patch
```

See [gist here](https://gist.github.com/josephdpurcell/a57bc443b58c7c1ca547e5a7b067ff30).

## Add Code Climate Config to a Drupal 8 Module

```
wget https://gist.githubusercontent.com/josephdpurcell/ca2572a1f2764c1fe930885c29d06382/raw/cc3437d7e93c5b9184561a5e09d34921bb6336b6/0001-Add-.codeclimate.yml-for-Drupal-8-modules.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-8-modules.patch
```

See [gist here](https://gist.github.com/josephdpurcell/ca2572a1f2764c1fe930885c29d06382).

# Improvements

* Check Symfony using https://github.com/djoos/Symfony2-coding-standard
* Use AST like [Phan](https://github.com/etsy/phan) or [pharborist](https://github.com/grom358/pharborist)
* Involve the [Drupal Technical Working Group](https://groups.drupal.org/node/510675), see also [guidelines](https://www.drupal.org/project/coding_standards)
* Have PHPCS include Drupal code sniffs (just like it does for PRS2)
* Include security sniffs:
    * [Drupal Security Sniffs](https://www.drupal.org/sandbox/coltrane/1921926), see also [issue](https://www.drupal.org/node/1844870)
    * [FloeDesignTechnologies/phpcs-security-audit](https://github.com/FloeDesignTechnologies/phpcs-security-audit)
* Add checks for CSS and JS
* Compare Scruitinizer and phpmetrics.org with Code Climate
* Check [laravel](https://github.com/laravel/laravel) and [laravel framework](https://github.com/laravel/framework)
* How does this compare with [https://www.drupal.org/node/1299710](https://www.drupal.org/node/1299710)?
