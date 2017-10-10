[Docs](https://github.com/coryhouse/react-slingshot) | [FAQ](https://github.com/coryhouse/react-slingshot/blob/master/docs/FAQ.md)

Do these:

1. `npm install`
2. `npm run remove-demo`
3. `npm run setup` //this will remove the .git folder so run `git init` afterwards
4. update this README


# UNIT TESTING

### Setup

1. Install mocha globally: `npm i -g mocha`
2. Make sure the project has these npm dependencies:
  - mocha
  - chai
  - enzyme
  - mochawesome
  - browser-sync
  - jsdom
  - Optional packages:
    - sinon
    - mocha-clean
    - nock
    - redux-mock-store

3. All configs, generated runner files, and mocks go into the **test/** directory.
4. Mocha finds all **\*.test.js** files in the src. directory.
5. In your test files, make sure to import whatever interface you choose (expect, should, or assert) from Chai. Importing Chai itself is optional:
```javascript
import chai, { expect } from 'chai';
```
6. import any other test tools, data, react components that you need as well for that particular test.


### Run Tests

To run testing, run `npm test`. This will watch your create a separate testing server via browser-sync, create a test runner page, run all tests, and update the tests when you make changes.
