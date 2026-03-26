# Codewars-Weight for weight (Javascript)

```
function orderWeight(strng) {
  strng = strng.split(' ').sort();
  const weightList = strng.map(s => {
    return s.split('').reduce((acc, cur) => acc + Number(cur), 0);
  })
  strng.sort((a, b) => weightList[strng.indexOf(a)] - weightList[strng.indexOf(b)]);
  
  return strng.join(' ');
}
```

[KATA](https://www.codewars.com/kata/55c6126177c9441a570000cc/javascript)
<br>

[Medium](https://medium.com/@juneee/codewars-weight-for-weight-javascript-d09ba232ff63)
