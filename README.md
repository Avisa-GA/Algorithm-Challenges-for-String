## Algorithm-Challenges-for-String

>> Input : "2 + 5 = x"
>> And Output must be less than 10
>> </br>
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
