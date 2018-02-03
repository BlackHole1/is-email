# is-email

[![CircleCI](https://circleci.com/gh/segmentio/is-email.svg?style=shield&circle-token=38faad587c396e66c475415a096207d2de27e324)](https://circleci.com/gh/segmentio/is-email)
[![Codecov](https://img.shields.io/codecov/c/github/segmentio/is-email/master.svg?maxAge=2592000)](https://codecov.io/gh/segmentio/is-email)


Loosely validate an email address.

## Installation
  
```
$ npm install is-email
```

## API

### isEmail(string)

Loosely checks whether a `string` is an email address.

## Use

```javascript
isEmail('team@segment.io') // => true
isEmail('team+@segmentio.com') // => true
isEmail('te-am@segmentio.com') // => true
isEmail('team@segmen-tio.com') // => true
isEmail('t-eam+34@segme-ntio.com') // => true

isEmail('team@.org') // => false
isEmail('team+45.io') // => false
isEmail('@segmentio.com') // => false
```
