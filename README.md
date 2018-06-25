![freeCodeCamp Social Banner](https://s3.amazonaws.com/freecodecamp/wide-social-banner.png)

# freeCodeCamp Curriculum

[![Build Status](https://travis-ci.org/freeCodeCamp/curriculum.svg?branch=master)](https://travis-ci.org/freeCodeCamp/curriculum) [![npm (scoped)](https://img.shields.io/npm/v/@freecodecamp/curriculum.svg)](https://www.npmjs.com/package/@freecodecamp/curriculum)
[![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)

> This package contains the "challenge" files used in the freeCodeCamp Curriculum.

## Installation

```sh
npm i @freecodecamp/curriculum
# or
yarn add @freecodecamp/curriculum
```

## Usage

```js
import { getChallenges } from '@freecodecamp/curriculum';

// fetch an array of blocks
// i.e. basic CSS, functional programming, etc.
getChallenges()
```

### `block` Structure

```js
{
  "name": "ES6",
  "order": 2,
  "time": "5 hours",
  "helpRoom": "Help",
  "challenges": [/*<challenge>*/],
  "fileName": "02-javascript-algorithms-and-data-structures/es6.json",
  "superBlock": "javascript-algorithms-and-data-structures",
  "superOrder": 2
}
```

### `challenge` Structure

```js
{
  "id": "ObjectId()",
  "title": "Declare a Read-Only Variable with the const Keyword",
  "description": [
    "A Description of the challenge and what is required to pass"
  ],
  "tests": [
    {
      "text": "should return \"foo\"",
      "testString": "a stringified function using Chai asserts"
    }
  ],
  "challengeType": 1,
  "translations": {},
  "files": {
    "indexjs": {
      "key": "indexjs",
      "ext": "js",
      "name": "index",
      "contents": [
        "Initial editor seed"
      ],
      "head": [
        "A place for test set up",
        "Can be thought of as mocha's beforeEach()"
      ],
      "tail": [
        "A place for test tear down",
        "Can be thought of as mocha's afterEach()"
        ]
    }
  }
},
```

## 翻译流程

 1. 在本项目导航栏【Issue】中选择 [**Translation request**](https://github.com/FreeCodeCampChina/curriculum/issues/new?template=translation-request.md) 模板，并填写你想要翻译的章节（以独立 JSON 文件为最小单位）。

 2. 若你想翻译多节课，请用 [GFM 的 Task lists 语法](https://guides.github.com/features/mastering-markdown/)列出这些课程，并在翻译完每节课后在该条目前的复选框打勾，以此来跟踪自己的翻译进度。
 
 3. 翻译完成后请提交 Pull request，并选择 [@S1ngS1ng](https://github.com/S1ngS1ng) 与 [@wudifeixue](https://github.com/wudifeixue) 两位同学进行评审。

**【注意】**翻译文件不要在源文件上改动，请创建新文件并以 `-cn` 作为文件名后缀。

