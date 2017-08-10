# title-case

https://www.codewars.com/kata/title-case/

This is a small walkthrough of the **Title Case** Codewars kata. It is possible to complete it by using regular expressions or algorithms and methods as well. For the purpose of learning algorithms itself, I chose the second path. This walkthrough is meant to show the process of reaching a good and easy to read solution by refining and cleaning code. :mag:

```javascript
const titleCase = (title, minorWords) => {
  if (!minorWords) {
    minorWords = title;
    let minorEmpty = minorWords.toLowerCase().split(' ');

    for (let word = 1; word < minorEmpty.length; word++) {
      minorEmpty[word] = minorEmpty[word][0].toUpperCase() + minorEmpty[word].slice(1);
    }

    minorEmpty = minorEmpty.join(' ');
    return minorEmpty.substring(0, 1).toUpperCase() + minorEmpty.replace(minorWords.substring(0, 1), '');
  }

  let titleArr = title.toLowerCase().split(' ');
  let minorArr = minorWords.toLowerCase().split(' ');

  titleArr[0] = titleArr[0][0].toUpperCase() + titleArr[0].slice(1);

  for (let word = 1; word < titleArr.length; word++) {
    if (minorArr.indexOf(titleArr[word]) === -1) {
      titleArr[word] = titleArr[word][0].toUpperCase() + titleArr[word].slice(1);
    }
  }

  return titleArr.join(' ');
}
```

This is the first version of my solution. But, woah, there is a lot of ~~spaghetti~~ repeating code here!

We can make it better by evading having to uppercase the first letter only to replace it afterwards in our return statement on line 16.
Another thing we can do is to create a helper function that will help us with all of the capitalization and slicing thing happening.

Let's start with the second so we can clean our code a bit. That leaves us with:

```javascript
const titleCase = (title, minorWords) => {
  if (!minorWords) {
    minorWords = title;
    let minorEmpty = minorWords.toLowerCase().split(' ');

    for (let word = 1; word < minorEmpty.length; word++) {
      minorEmpty[word] = capitalize(minorEmpty[word]);
    }

    minorEmpty = minorEmpty.join(' ');
    return minorEmpty.substring(0, 1).toUpperCase() + minorEmpty.replace(minorWords.substring(0, 1), '');
  }

  let titleArr = title.toLowerCase().split(' ');
  let minorArr = minorWords.toLowerCase().split(' ');

  titleArr[0] = capitalize(titleArr[0]);

  for (let word = 1; word < titleArr.length; word++) {
    if (minorArr.indexOf(titleArr[word]) === -1) {
      titleArr[word] = capitalize(titleArr[word]);
    }
  }

  return titleArr.join(' ');
}

const capitalize = (str) => {
  return str[0].toUpperCase() + str.slice(1);
}
```

Ahhh! Much better. Now we can thoroughly focus on our `!minorWords` if statement. Turns out we don't even need this after all!

```javascript
const titleCase = (title, minorWords) => {
  let titleArr = title.toLowerCase().split(' ');
  let minorArr = (minorWords || '').toLowerCase().split(' ');

  titleArr[0] = capitalize(titleArr[0]);

  for (let word = 1; word < titleArr.length; word++) {
    if (minorArr.indexOf(titleArr[word]) === -1) {
      titleArr[word] = capitalize(titleArr[word]);
    }
  }

  return titleArr.join(' ');
}

const capitalize = (str) => {
  return (str[0] || '').toUpperCase() + str.slice(1);
}
```

Adding the ` || '' `s next to our `minorArr` and our capitalize helper `str` strings can mark them as optional, just as the kata description says. By doing this, we evade having to deal with undefined values. We are also left with a really clean and easily readable code. *10 points to Hufflepuff!* :satisfied:
