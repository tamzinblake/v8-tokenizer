## v8-tokenizer

Beginning of an attempt to tokenize v8 without parsing in emacs lisp.

Not safe for public consumption.

The attempt was doomed to failure from the beginning, because the
following cases are not distinguishable without parsing:

```javascript
if (foo) /bar/

;(foo) /bar/
```
