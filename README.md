# Code Climate and Drupal

With the release of Drupal 8, it is apparent that improvements in speed and stability of development is needed<sup>[1](#footnote1)</sup>. However, the reality of this challenge is daunting: at over a million lines of code and with hundreds of lines in core and module code being added, removed, and modified every month by contributors all around the world, any improvements will take significant time and effort to coordinate. Thanks to developments in academia and automation tools developed by the PHP community, we have an easy win: static analysis.

To know how to improve, we need to start with understanding where we are. The speed of Drupal development is being hindered by the "noise" of bug tickets, the time to triage a bug to identify its cause, the time to resolve conflicts between patches, rework required due to close coupling, onboarding time for new contributors, and the time it takes to reach consensus on changes. Stability of development is hindered by code being hard to test, high coupling, and high complexity. Static analysis is an automated process that can surface improvements in all of these aspects.

Static analysis with Code Climate provides a free and objective way to discover error-prone and incorrect code. Initiative leads can do design reviews using coupling and complexity metrics to understand which areas of the system are most difficult to test and extend. Early contributors can quickly assist with resolving code style violations, adding missing documentation, and removing unused or duplicate code. Core and module maintainers can get warnings of code that poses a risk for bugs or security holes such as unused variables or references to superglobals. Site builders can use churn and quality metrics to compare the stability of different modules. Thus, we have an automated way to find and prevent bugs and identify and quantify improvements.

As a result the speed and stability of development is improved through fewer bugs, cleaner code that is easier to test and maintain, and greater flexibility and extensibility by better adhering to SOLID software design<sup>[2](#footnote2)</sup>. There are a predicted 1,500 bugs in Drupal 8 core<sup>[3](#footnote3)</sup>. Projects with large code bases, such as the Linux kernel and Windows server, are using static analysis tools like Code Climate to proactively resolve those bugs and improve quality, keep their teams operating at speed and their releases stable<sup>[4](#footnote4)</sup>. While other efforts in the Drupal community will arise to address these development needs, doing static analysis with Code Climate gives us clear and immediate direction we can act on.

# References

<a name="footnote1">1</a>. The need for speed and stability of development is derived from the "[Drupal 8 Retrospective Suggestions](https://docs.google.com/document/d/11ZcXSSqvAGkI4AQ9-GxQmnMR3E9bo8Z9DUA58bY7_Sk/mobilebasic)" Google Doc survey results.

<a name="footnote2">2</a>. For an explanation of SOLID software design, see the "[SOLID (object-oriented design)](https://en.wikipedia.org/wiki/SOLID_%28object-oriented_design%29)" article on WikiPedia.

<a name="footnote3">3</a>. To compute this, take the "bugs" column on the "Explore" tab of the [phpmetrics results for Drupal Core 8.0.6](phpmetrics-drupal-8.0.6.html) and multiply it by the number of files on the "Evaluation" tab. The math, then, is: 0.46 bugs * 3,373 files = 1,551.58 bugs.

<a name="footnote4">4</a>. The Linux kernel and Windows server teams found static analysis to have a 0.56 and 0.58 correlation with bug reports, see "[Linux Kernel Developer Responses to Static Analysis Bug Reports](https://www.usenix.org/legacy/event/usenix09/tech/full_papers/guo/guo_html/index.html)" by Philip J. Guo and Dawson Engler from Stanford University for details.

# Examples

Note: these GPA's are likely out of date, so verify the commit Code Climate has matches with the latest commit.

* [![Code Climate](https://codeclimate.com/github/josephdpurcell/workbench_moderation/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/workbench_moderation) [GitHub fork for drupal/workbench_moderation](https://github.com/josephdpurcell/workbench_moderation)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-multiversion/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-multiversion) [GitHub fork for drupal/multiversion](https://github.com/josephdpurcell/multiversion)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-deploy/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-deploy) [GitHub fork for drupal/drupal-deploy](https://github.com/josephdpurcell/drupal-deploy)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-replication/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-replication) [GitHub fork for drupal/drupal-replication](https://github.com/josephdpurcell/drupal-replication)
* [![Code Climate](https://codeclimate.com/github/josephdpurcell/drupal-relaxed/badges/gpa.svg)](https://codeclimate.com/github/josephdpurcell/drupal-relaxed) [GitHub fork for drupal/drupal-relaxed](https://github.com/josephdpurcell/drupal-relaxed)

# How To's

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

# TODOs

* explain why Code Climate is a better choice than other tools
* explain how Code Climate will work and give an example
* create slides for BOF
* identify a better title
