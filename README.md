# vuefire-analytics brenda [![Build Status brenda](https://travis-ci.com/breadplop/test.svg?branch=master)](https://travis-ci.com/breadplop/test)

Tags: `continuous test and deployment`, `travis-ci`

> This repo demonstrates how travis-ci can be used to automatically run unit tests and coverage reports upon commits to your github repo.

---
## Situation
Current Build Status = `failing`

## Task: 
Change build status to `passing`

---

## Instructions
Notice that the current build status is `failing`

1. Fork the repo
2. Go to [Travis-ci](https://travis-ci.com/) and sign up for an account with GITHUB
  - authorize travis-pro to access your repos
  - you should be redirected to this page `https://travis-ci.com/account/repositories` that says Github Apps Integration
  - press on the green `Activate` button --> green `Approve & Install` button
3. Edit README.md
  - On the first line, replace breadplop/test with `<github_username>/vue-deployment-check` 
    _Example:_
  ```
  # vuefire-analytics brenda [![Build Status brenda](https://travis-ci.com/breadplop/test.svg?branch=master)](https://travis-ci.com/breadplop/test)
  
  # vuefire-analytics brenda [![Build Status brenda](https://travis-ci.com/thngktb/vue-deployment-check.svg?branch=master)](https://travis-ci.com/thngktb/vue-deployment-check)
  
  ```
  - Save and commit change to master (i.e. Scroll to the bottom of the page and press `commit changes`)
  - Go back to the repo's main page (e.g. https://github.com/breadplop/vue-deployment-check) and wait for about 3 minutes
  - Refresh the main page and you should see `build:failing`
  
4. Edit `main.spec.js` file to change build status to `passing`
  - Go to `main.spec.js` file and change line 6 to `expect(2).toEqual(3);` to `expect(2).toEqual(2);`
  - Save and commit change to master (i.e. Scroll to the bottom of the page and press `commit changes`)
  - Go back to the repo's main page (e.g. https://github.com/breadplop/vue-deployment-check) and wait for about 3 minutes
  - Refresh the main page and you should see `build:passing`
  
Well done!


