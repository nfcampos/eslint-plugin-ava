# Allow only use of the asserts that have no power-assert alternative.

Translations: [Français](https://github.com/sindresorhus/ava-docs/blob/master/fr_FR/related/eslint-plugin-ava/docs/rules/prefer-power-assert.md)

- [`t.truthy()`](https://github.com/sindresorhus/ava#truthyvalue-message) __(You can do [most things](https://github.com/sindresorhus/ava#enhanced-assertion-messages) with this one)__
- [`t.deepEqual()`](https://github.com/sindresorhus/ava#deepequalvalue-expected-message)
- [`t.notDeepEqual()`](https://github.com/sindresorhus/ava#notdeepequalvalue-expected-message)
- [`t.throws()`](https://github.com/sindresorhus/ava#throwsfunctionpromise-error-message)
- [`t.notThrows()`](https://github.com/sindresorhus/ava#notthrowsfunctionpromise-message)
- [`t.pass()`](https://github.com/sindresorhus/ava#passmessage)
- [`t.fail()`](https://github.com/sindresorhus/ava#failmessage)

Useful for people wanting to fully embrace the power of [power-assert](https://github.com/power-assert-js/power-assert).


## Fail

```js
import test from 'ava';

test(t => {
	t.is(foo, bar);
});
```


## Pass

```js
import test from 'ava';

test(t => {
	t.truthy(foo === bar);
});
```
