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
