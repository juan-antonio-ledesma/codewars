# [Find the unique number - 6 kyu](https://www.codewars.com/kata/585d7d5adb20cf33cb000235)

```javascript
const findUniq = arr => {
  const firstThreeNumbersOrdered = arr.slice(0, 3).sort((a, b) => a - b)
  const repeatedNumber =
    firstThreeNumbersOrdered[1] === firstThreeNumbersOrdered[2]
      ? firstThreeNumbersOrdered[2]
      : firstThreeNumbersOrdered[0]

  return arr.filter(number => number != repeatedNumber)[0]
}
```
