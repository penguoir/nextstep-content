---
title: Testing
slug: testing
---

Tests are code which makes sure that other code works as expected.

Writing code which tests other code might seem like a waste of time, but it's a
valuable practice. Writing tests means you know that even if you change your
code, it will still work as expected.

There are different kinds of tests. The main tests developers write are:

* System tests
* Unit tests

**System tests** test multiple parts of the application together. For example,
a request to your web server.

**Unit tests** test singluar parts of the application. For example, a function.

1. Write a test for the following function

    ```javascript
    function add(a, b) {
      return a + b
    }
    ```

    Here is what to test for:

    * It should add two numbers
    * It should not coerce arguments to numbers

    Use the Node.js `assert` module. Here's [the `assert` module
    documentation](https://nodejs.org/api/assert.html) and here's [the `ok`
    method](https://nodejs.org/api/assert.html#assert_assert_ok_value_message),
    which you should try out first.

    Here's how Lodash writes this test for reference: [Lodash
    add.test.js](https://github.com/lodash/lodash/blob/master/test/add.test.js)

    Lodash uses some custom functions (`describe()` and `it()`). These functions
    simply run the tests inside. See [the Mocha
    documentation](https://mochajs.org/) for more details.

2. Write tests for 5 Lodash functions of your choice. Try to figure out edge
   cases of the functions, and test those too.

3. Most repositories use a more complicated test suite. This is not necessary,
   but will help when testing more complex frameworks such as React. Read [the
   Jest documentation](https://jestjs.io/docs/getting-started), and complete the
   Getting Started page.

4. Write tests for a React project you've done previously.

   You can test React projects using Jest. A good library that simplifies this
   process is
   [react-testing-library](https://github.com/testing-library/react-testing-library).
   For examples of React component tests, see the [Chakra UI on
   GitHub](https://github.com/chakra-ui/chakra-ui/tree/326813ea261ddb6c9f0106e7e63f49f51e111fa2/packages).

OPTIONAL: Read [Testing
Rails](https://books.thoughtbot.com/assets/testing-rails.pdf). This guide is
intended for Ruby on Rails, but the principles can be brought over to any
programming language.
