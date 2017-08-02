# wordBird
**Kata page:** [https://www.codewars.com/kata/wordbird/javascript](https://www.codewars.com/kata/wordbird/javascript)

**Kata description:** The word bird is a strange animal, it only feeds on words! It likes all kind of words: long, short, in another language, even madeup ones. Its really picky when it comes to what the words entail though, and it only eats words with letters in it. It will reject even the most long delicious word for containing as little as a number or symbol in it. The one exeption is that the word bird doesn't care about air, and will eat a word that contains whitespace, as long as its at least one letter in there! It also doesnt mind upper or lowercase letters, its not case sensitive!

Your job is to help the word bird by making a function that filters out the words containing non-letters (except whitespace). You will be passed an array with strings, and should return an array containing the strings that the word bird likes.

```javascript
const wordBird = (arr) => {
  return arr.filter(item =>
    item.charCodeAt(item) > 64
    && item.charCodeAt(item) < 123
    && !item.includes(0)
    && !item.includes('-'));
}
```

**My thoughts on this kata:** It is fairly easy to solve it with regular expressions by testing for words, empty spaces and non digits inside our filter method, but since the test cases were simple, I wanted to solve it without using them. I will probably submit a new solution when the kata gets updated with more diverse test cases to pass.
