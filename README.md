# Logic Test
> by Mazhar.isk


### `Question 1`
```
const soal1 = (arr = []) => {
  return arr.map(item => {
    if (item % 2 === 0) return item * 2
    return item * 3
  })
} 
```

### `Question 2`
```
const isFibo = (value = 0) => {
   const perfectSquare = (num) => {
      const square = parseInt(Math.sqrt(num))
      return (square * square == num)
   }
   return perfectSquare(5 * value * value + 4) || perfectSquare(5 * value * value - 4)
}
```

### `Question 3`
```
const soal3 = (arr = []) => {
  let result = {}

  for (let word of arr) {
    let key = word.split("").sort().join("")
    if (result[key]) {
      result[key].push(word)
     } else {
      result[key] = [word]
     }
  }
  return Object.values(result)
}
```

### `Question 4`
```
const soal4 = (arr = []) => {
   return arr.map(val => {
      const isModulus3 = (val % 3) === 0
      const isModulus7 = (val % 7) === 0
      if (isModulus3 && isModulus7) return 'Link Aja'
      if (isModulus3) return 'Link'
      if (isModulus7) return 'Aja'
      return val
   })
}
```
