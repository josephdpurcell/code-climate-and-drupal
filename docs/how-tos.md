# How To's

Below are examples of how to add Code Climate to a Drupal project, core, or module. These are a work in progress. For now they focus on PHPCS code style and some PHPMD checks that seem appropriate for Drupal code.

## Drupal 7 Project

To add a Code Climate config designed for a Drupal 7 project:

```
wget https://gist.githubusercontent.com/josephdpurcell/688383828f768be3aba6662d0a7736bf/raw/567617903f574ebfeb5957499a4d58e66d40a977/0001-Add-.codeclimate.yml-for-Drupal-7-project.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-7-project.patch
```

See [gist here](https://gist.github.com/josephdpurcell/688383828f768be3aba6662d0a7736bf).

@todo write notes about how if its an Acquia, composer-based, or multisite project it will be different

## Drupal 7 Core

To add a Code Climate config designed for Drupal 7 core:

```
wget https://gist.githubusercontent.com/josephdpurcell/c4c5bb42bb8f4dd75b0cdaf41e2a023e/raw/b54f27bfc11538093150a89a65120b006256337e/0001-Add-.codeclimate.yml-for-Drupal-7-core.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-7-core.patch
```

See [gist here](https://gist.github.com/josephdpurcell/c4c5bb42bb8f4dd75b0cdaf41e2a023e).

@todo confirm the ratings paths are correct

@todo add .install files

## Drupal 7 Modules

@todo write one for Drupal 7 modules

## Drupal 8 Project

@todo write one for a Drupal 8 project

## Drupal 8 Core

To add a Code Climate config designed for Drupal 8 core:

```
wget https://gist.githubusercontent.com/josephdpurcell/a57bc443b58c7c1ca547e5a7b067ff30/raw/f80049648971775fe4fe7b36a85b9c8060a47e88/0001-Add-.codeclimate.yml-for-Drupal-8-Core.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-8-Core.patch
```

See [gist here](https://gist.github.com/josephdpurcell/a57bc443b58c7c1ca547e5a7b067ff30).

## Drupal 8 Modules

To add a Code Climate config designed for Drupal 8 modules:

```
wget https://gist.githubusercontent.com/josephdpurcell/ca2572a1f2764c1fe930885c29d06382/raw/6a0904f0bf7cded8fb168f459064514ed7fa2526/0001-Add-.codeclimate.yml-for-Drupal-8-modules.patch
git am --signoff < 0001-Add-.codeclimate.yml-for-Drupal-8-modules.patch
```

See [gist here](https://gist.github.com/josephdpurcell/ca2572a1f2764c1fe930885c29d06382).

