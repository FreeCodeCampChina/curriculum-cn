```flow
st=>start: 注册印象笔记
e=>end: 您可以使用markdown
op1=>operation: 登录印象笔记
op2=>operation: 购买并登录马克飞象
cond=>condition: 是否已经购买并登录了马克飞象?

st->op1->cond
cond(yes)->e
cond(no)->op2->e
```





![freeCodeCamp Social Banner](https://s3.amazonaws.com/freecodecamp/wide-social-banner.png)

# freeCodeCamp China Curriculum

[![Build Status](https://travis-ci.org/freeCodeCamp/curriculum.svg?branch=master)](https://travis-ci.org/freeCodeCamp/curriculum) [![npm (scoped)](https://img.shields.io/npm/v/@freecodecamp/curriculum.svg)](https://www.npmjs.com/package/@freecodecamp/curriculum)
[![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)

> 本项目包含 freeCodeCamp 中文官网的所有挑战题目。

## 安装 (未发布)

~~npm i @freecodecamp/curriculum~~
# or
~~yarn add @freecodecamp/curriculum~~

## 使用

~~import { getChallenges } from '@freecodecamp/curriculum';~~

~~// fetch an array of blocks~~
~~// i.e. basic CSS, functional programming, etc.~~
~~getChallenges()~~

### 挑战类别数据结构

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

### 挑战题目数据结构

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

## 翻译指南

### 工作流程

1. 在本项目导航栏【Issue】中选择 [**Translation request**](https://github.com/FreeCodeCampChina/curriculum/issues/new?template=translation-request.md) 模板，并填写你想要翻译的章节（以独立 JSON 文件为最小单位）。

2. 若你想翻译多节课，请用 [GFM 的 Task lists 语法](https://guides.github.com/features/mastering-markdown/)列出这些课程，并在翻译完每节课后在该条目前的复选框打勾，以此来跟踪自己的翻译进度。
 
3. 翻译完成后请提交 Pull request，并选择 [@S1ngS1ng](https://github.com/S1ngS1ng) 与 [@wudifeixue](https://github.com/wudifeixue) 两位同学进行评审。

**【注意】** 翻译文件不要在源文件上改动，请创建新文件并以 `-cn.json` 作为文件名后缀。

### 行文规范

1. 最高原则：信、达、雅（技术专业内容要用语规范，网络用语不要出现）
 
2. 专用单词：拼写正确（参考对应技术的官网、维基百科词条）、注意大小写
 
3. 标点符号
    - 中英文各自选择对应的标点符号，中英文混合句视同中文语句（如括号内中英文混用，应用中文括号）
    - 中文标点、文字间无需空格
    - 英文单标点后空一格，成对标点左标左空格、右标右空格

4. 全角与半角字符（如中文与英文，及中文与数字）间须用空格隔开（参考[盘古](https://github.com/vinta/pangu.js)）

