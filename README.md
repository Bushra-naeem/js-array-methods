# JavaScript Array Methods

## JavaScript Array reduceRight() Method

The reduceRight() method in JavaScript is used to convert elements of
the given array from right to left to a single value.

Note − If the current array is empty or doesn't contain any initialValue, this method will
throw a 'TypeError' exception.

```sh
const array = [10, 20, 30, 40, 50];
const sum = array.reduceRight((acc, currentValue) => acc + currentValue, 0);
console.log(sum); // Output: 150
```

## JavaScript Array some() Method

The some() method performs testing and checks if atleast a single array element passes the test,
implemented by the provided function. If the test is passed, it returns true. Else, returns false.

Note: If some() method is applied on an empty array, it returns false always.

```sh
const array = [1, 2, 3, 4, 5];
const hasEven = array.some((element) => element % 2 === 0);
console.log(hasEven); // Output: true
```

## JavaScript Array filter() Method

The filter() method doesn't modify the original array, but instead returns a new array
containing only the elements that meet the specified condition.

```sh
const numbers = [1, 2, 3, 4, 5];
const evenNums = numbers.filter((num) => num % 2 === 0);
console.log(evenNums); // Output: [2, 4]
```

## JavaScript Array map() Method

The map() method in JavaScript is a higher-order function that creates a new array by applying a function to each element of the original array. Used it when you want to transform the array.

```sh
const arr = [1, 2, 3, 4];
const resultArr = arr.map((element) => element * 2);
console.log(resultArr); // Output: [2, 4, 6, 8]
```

## JavaScript Array forEach() Method

The forEach() method executes a function for each array element but doesn't return a new array.
Typically used for side effects like logging or modifying external variables.

```sh
let names = ["Bushra", "Rumaisa", "Ryle"];
names.forEach((name) => {
    console.log(name);
}); // Output: Bushra, Rumaisa, Ryle
```

## JavaScript Array slice() Method

The slice() method returns selected elements in an array as a new array. It selects from a given start, up to a (not inclusive) given end. It doesn't alter the original array but instead creates a shallow copy.

```sh
const cities = ["Tokyo", "Cairo", "Los Angeles", "Paris", "Seattle"];
const newCityArr = cities.slice(2, 4);
console.log(newCityArr); // Output: ['Los Angeles', 'Paris']
```

## JavaScript Array splice() Method

The splice() Method in JavaScript is used to change the contents of an array by removing or replacing existing elements and/or adding new elements. It modifies the original array and returns an array of the removed elements.

```sh
let skills = ["JavaScript", "Reactjs", "Nextjs"];
let tools = skills.splice(3, 0, "git", "jira");
console.log(skills); // Output: [ 'JavaScript', 'Reactjs', 'Nextjs', 'git', 'jira' ]
```

## JavaScript Array reduce() Method

The reduce() method iterates over an array, applying a reducer function to each element, accumulating a single output value. It takes an initial value and processes elements from left to right, reducing the array to a single result.

```sh
const arr = [1, 2, 3, 4, 5];
const sum = arr.reduce((acc, x) => acc + x, 0);
console.log(sum); // Output: 15
```
