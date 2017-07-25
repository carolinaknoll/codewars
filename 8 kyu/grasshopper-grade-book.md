# grasshopper-grade-book
// https://www.codewars.com/kata/grasshopper-grade-book/solutions/javascript/me/best_practice


```
const getGrade = (s1, s2, s3) => {
  let grade = (s1 + s2 + s3) / 3;
  return grade >= 90 ? "A" :
         grade >= 80 ? "B" :
         grade >= 70 ? "C" :
         grade >= 60 ? "D" : "F";
}

```

```
const getGrade = (s1, s2, s3) => {
  let gradeNumber = (s1 + s2 + s3) / 3;

  return gradeNumber < 60 ? "F" :
  gradeNumber >= 60 && gradeNumber < 70 ? "D" :
  gradeNumber >= 70 && gradeNumber < 80 ? "C" :
  gradeNumber >= 80 && gradeNumber < 90 ? "B" :
  gradeNumber >= 90 ? "A" : "No grade listed";
}

```
