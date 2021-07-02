---
title: CI/CD
slug: ci-cd
---

**Knowledge Section:** You only have to read the following section. It is
intended to provide you with an overview of existing technologies, so you have
the context for when you encounter them in the real world.

Continuous integration/Continuous delivery (CI/CD) allows developers to work on
products and release the new code efficiently. CI/CD systems usually take the
following form:

* A Git repository to which developers upload code.
* A server that runs tasks on this repository.

For example, the server could run some of the following tasks:

* Run style checks (e.g. using semicolons in JavaScript files).
* Check that all tests pass.
* Send a message to the lead developer.
* Upload the new code to the server.
* Upload the new code to a staging (temporary) server for further tests.

CI/CD is helpful because it prevents mistakes. For example, developers don't
accidentally upload test code to the live server. Also, it enforces best
practices such as testing.

You can use [GitHub Actions][github-actions] to run a CI/CD system. There are
other platforms which provide similar services such as GitLab, CircleCI and
Jenkins.

[github-actions]: https://github.com/features/actions