# How To's

Below are examples of how to add Code Climate to a Drupal project, core, or module. These are a work in progress. For now they focus on PHPCS code style and some PHPMD checks that seem appropriate for Drupal code.

## Drupal 7 Project

To add a Code Climate config designed for a Drupal 7 project:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-7-project-Code-Climate-config.patch
git apply --index < 0001-Add-Drupal-7-project-Code-Climate-config.patch
git commit -m 'Add Drupal 7 project Code Climate config'
```

@todo write notes about how if its an Acquia, composer-based, or multisite project it will be different

## Drupal 7 Core

To add a Code Climate config designed for Drupal 7 core:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-7-core-Code-Climate-config.patch
git apply --index < 0001-Add-Drupal-7-core-Code-Climate-config.patch
git commit -m 'Add Drupal 7 core Code Climate config'
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
git apply --index < 0001-Add-Drupal-8-core-Code-Climate-config.patch
git commit -m 'Add Drupal 8 core Code Climate config'
```

## Drupal 8 Modules

To add a Code Climate config designed for Drupal 8 modules:

```
wget https://raw.githubusercontent.com/josephdpurcell/code-climate-and-drupal/gh-pages/code-climate-configs/0001-Add-Drupal-8-module-Code-Climate-config.patch
git apply --index < 0001-Add-Drupal-8-module-Code-Climate-config.patch
git commit -m 'Add Drupal 8 module Code Climate config'
```

