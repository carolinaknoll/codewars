# fun-with-es6-classes-2-animals-and-inheritance
https://www.codewars.com/kata/56f935002e6c0d55fa000d92/


```javascript
class Shark extends Animal {
  constructor(name, age, status) {
    super(name, age, 0, 'shark', status);
  }
}

class Cat extends Animal {
  constructor(name, age, status) {
    super(name, age, 4, 'cat', status);
  }

  introduce() {
    return `${super.introduce()}  Meow meow!`;
  }
}

class Dog extends Animal {
  constructor(name, age, status, master) {
    super(name, age, 4, 'dog', status);
    this.master = master;
  }

  greetMaster() {
    return `Hello ${this.master}`;
  }
}
```

```javascript
class Shark extends Animal {
  constructor(name, age, status) {
    super(name, age, status);
    this.name = name;
    this.age = age;
    this.status = status;
    this.legs = 0;
    this.species = 'shark';
  }
}

class Cat extends Animal {
  constructor(name, age, status) {
  super();
    this.name = name,
    this.age = age;
    this.status = status;
    this.legs = 4;
    this.species = 'cat';
  }

  introduce() {
    return `Hello, my name is ${this.name} and I am ${this.age} years old.  Meow meow!`;
  }
}

class Dog extends Animal {
  constructor(name, age, status, master) {
  super();
    this.name = name;
    this.age = age;
    this.status = status;
    this.master = master;
    this.legs = 4;
    this.species = 'dog';
  }

  greetMaster() {
    return `Hello ${this.master}`;
  }
}

```
