# fun-with-es6-classes-number-1-people-people-people
https://www.codewars.com/kata/fun-with-es6-classes-number-1-people-people-people/


```javascript
class Person {
  constructor(firstName, lastName, age, gender) {
    this.firstName = firstName || 'John';
    this.lastName = lastName || 'Doe';
    this.age = age || 0;
    this.gender = gender || 'Male';
  }

  sayFullName() {
    return this.firstName + ' ' + this.lastName;
  }

  static greetExtraTerrestrials(raceName) {
    return 'Welcome to Planet Earth ' + raceName;
  }
}
```

```javascript
class Person {
  constructor( firstName, lastName, age, gender) {
    this.firstName = firstName || 'John'
    this.lastName = lastName   || 'Doe'
    this.age = age             || 0
    this.gender = gender       || "Male"

  }

  sayFullName(){
    return this.firstName + " " + this.lastName
  }

  // prefix 'class method' with the keyword 'static'
  static greetExtraTerrestrials(raceName) {
    return "Welcome to Planet Earth " + raceName
  }
}

```
