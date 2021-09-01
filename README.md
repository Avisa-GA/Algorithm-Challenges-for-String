## Algorithm-Challenges-for-String

>> Input : "2 + 5 = x"
>> Output : "7"

```ruby
function missingDigit(str) {
   for(let i = 0; i<10; i++) {
    const newStr = str.replace(/x/, i.toString()).replace(/=/, '===');
    if (eval(newStr)) {
      return i;
    }
  }
  return 'failed';
}

```
