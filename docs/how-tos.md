# How To's

Below are examples of how to add Code Climate to a Drupal project, core, or module. These are a work in progress. For now they focus on PHPCS code style and some PHPMD checks that seem appropriate for Drupal code.

## Drupal 7 Project

To add a Code Climate config designed for a Drupal 7 project:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-7-project-Code-Climate-config.patch
git am --signoff < 0001-Add-Drupal-7-project-Code-Climate-config.patch
```

See [gist here](https://gist.github.com/josephdpurcell/688383828f768be3aba6662d0a7736bf).

@todo write notes about how if its an Acquia, composer-based, or multisite project it will be different

## Drupal 7 Core

To add a Code Climate config designed for Drupal 7 core:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-7-core-Code-Climate-config.patch
git am --signoff < 0001-Add-Drupal-7-core-Code-Climate-config.patch
```

@todo confirm the ratings paths are correct

@todo add .install files

## Drupal 7 Modules

@todo write one for Drupal 7 modules

## Drupal 8 Project

@todo write one for a Drupal 8 project

## Drupal 8 Core

To add a Code Climate config designed for Drupal 8 core:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-8-core-Code-Climate-config.patch
git am --signoff < 0001-Add-Drupal-8-core-Code-Climate-config.patch
```

See [gist here](https://gist.github.com/josephdpurcell/a57bc443b58c7c1ca547e5a7b067ff30).

## Drupal 8 Modules

To add a Code Climate config designed for Drupal 8 modules:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-8-module-Code-Climate-config.patch
git am --signoff < 0001-Add-Drupal-8-module-Code-Climate-config.patch
```

See [gist here](https://gist.github.com/josephdpurcell/ca2572a1f2764c1fe930885c29d06382).

