# AlgoCasts

## Reverse string

Given a string, return a new string with the reversed
order of characters
Examples
reverse('apple') === 'leppa'
reverse('hello') === 'olleh'
reverse('Greetings!') === '!sgniteerG'

My solution

```javascript
function reverse(str) {
  let revString = '';
  for (let i = str.length - 1; i >= 0; i--) {
    revString = revString + str[i];
  }
  return revString;
}
```

Soulution using JS buitin functions

```javascript
function reverse(str) {
  return str.split('').reverse().join('');
}
```

Another solution

```javascript
function reverse(str) {
  revString = '';
  for (let character of str) {
    revString = character + revString;
  }
  return revString;
}
```

Solution using Advanced array function -- reduce()

```javascript
function reverse(str) {
  return str.split('').reduce((reversed, character) => {
    return character + reversed;
  }, '');
}
```
