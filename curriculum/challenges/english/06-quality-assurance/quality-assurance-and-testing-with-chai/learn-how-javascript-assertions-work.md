---
id: 587d824a367417b2b2512c46
title: Learn How JavaScript Assertions Work
challengeType: 2
forumTopicId: 301589
---

## Description

<section id='description'>

As a reminder, this project is being built upon the following starter project on <a href="https://repl.it/github/freeCodeCamp/boilerplate-mochachai">Repl.it</a>, or cloned from <a href='https://github.com/freeCodeCamp/boilerplate-mochachai/'>GitHub</a>.

</section>

## Instructions

<section id='instructions'>

Within `tests/1_unit-tests.js` under the test labelled `#1` in the `Basic Assertions` suite, change each `assert` to either `assert.isNull` or `assert.isNotNull` to make the test pass (should evaluate to `true`). Do not alter the arguments passed to the asserts.

</section>

## Tests

<section id='tests'>

```yml
tests:
  - text: All tests should pass.
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=0').then(data => {assert.equal(data.state,'passed'); }, xhr => { throw new Error(xhr.responseText); })
  - text: You should choose the correct method for the first assertion - `isNull` vs. `isNotNull`.
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=0').then(data => {  assert.equal(data.assertions[0].method, 'isNull', 'Null is null'); }, xhr => { throw new Error(xhr.responseText); })
  - text: You should choose the correct method for the second assertion - `isNull` vs. `isNotNull`.
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=0').then(data => {  assert.equal(data.assertions[1].method, 'isNotNull', '1 is not null'); }, xhr => { throw new Error(xhr.responseText); })
```

</section>

## Challenge Seed

<section id='challengeSeed'>

</section>

## Solution

<section id='solution'>

```js
/**
  Backend challenges don't need solutions, 
  because they would need to be tested against a full working project. 
  Please check our contributing guidelines to learn more.
*/
```

</section>
