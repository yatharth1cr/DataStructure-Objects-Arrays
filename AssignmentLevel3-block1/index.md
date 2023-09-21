1. What will be the output and explain the reason.

```js
let obj = { name: 'Arya' };
obj = { surname: 'Stark' };
let newObj = { name: 'Arya' };
let user = obj;
let arr = ['Hi'];
let arr2 = arr;
```

Answer the following with reason after going through the above code:

`[10] === [10]` <!-- false//boubt reason?? -->
`obj == newObj` //false
`obj === newObj` //false
`user === newObj` //false
`user == newObj` //false
`user == obj` //true
`arr == arr2` //true
`arr === arr2` //true

2. What's will be the value of `person1` and `person2` ? Explain with reason. Draw the memory representation diagram.
<!-- To add this image here use ![name](./hello.jpg) -->

```js
function personDetails(person) {
  person.age = 25;
  person = { name: 'John', age: 50 };
  return person;
}
let person1 = { name: 'Alex', age: 30 };
let person2 = personDetails(person1);
console.log(person1);
console.log(person2); 
```

3. What will be the output of the below code:

```js
let brothers = ['Bran', 'John'];
let user = {
  name: 'Sansa',
};
user.brothers = brothers;
brothers.push('Robb');
console.log(user.brothers === brothers);
console.log(user.brothers.length === brothers.length);