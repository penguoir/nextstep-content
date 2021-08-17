---
title: CI/CD
slug: ci-cd
---

Continuous integration/Continuous delivery (CI/CD) is a system that allows
developers to update code efficiently. CI/CD systems usually take the following
form:

* A Git repository to which developers upload their code.
* A server that runs tasks on this repository.

The server could, for example, run some of the following tasks:

* Run style checks (e.g. using semicolons in JavaScript files).
* Check that all tests pass.
* Send a message to the lead developer when there are changes.
* Upload new code to the server.
* Upload new code to a staging (temporary) server for further tests.

CI/CD is helpful because it prevents mistakes. For example, developers don't
accidentally upload test code to the live server. Also, it enforces best
practices such as testing.

You can use [GitHub Actions][github-actions] to run a CI/CD system. There are
other platforms which provide similar services such as GitLab, CircleCI and
Jenkins.

[github-actions]: https://github.com/features/actions

1. Go to [the ci/cd sample project][ci-cd-sample-project] and press "Fork".
2. In the new repository, set up a GitHub Action to run the test file using [the
GitHub Actions docs][github-actions-docs].
3. Run the action you created.
4. Commit a fix to the `index.js`. If you correctly fixed the code, all the
tests should pass.

[ci-cd-sample-project]: https://github.com/nextstep-sh/sample-cicd
[github-actions-docs]: https://docs.github.com/en/actions

Here's a project from start to finish:

1. Build and write tests for a React project. A good starting point is a
counter. Click a button to add one to a running total.
2. Write tests for this website using [Jest][jest].
3. Set up a CI/CD system using the [GitHub Actions
documentation][github-actions-docs] and the [GitHub pages deploy
action][github-pages-deploy-action]. This system should:

* Publish new code to GitHub pages.
* Only publish new code if all tests pass.

[jest]: https://jestjs.io/
[github-actions-doc]: https://docs.github.com/en/actions
[github-pages-deploy-action]: https://github.com/marketplace/actions/deploy-to-github-pages
