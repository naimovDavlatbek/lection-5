# lection-5
## What is Array in Java Script?
  Массив як тағирёбандаи махсусест, ки метавонад зиёда аз як арзиш дошта бошад:
 
 ## Why Use Arrays?
 If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:  
````Javascript
 let car1 = "Saab";
let car2 = "Volvo";
let car3 = "BMW";
````

However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars, but 300?

The solution is an array!
An array can hold many values under a single name, and you can access the values by referring to an index number.
 
____

##  CANGE ELEMENT IN ARRAY.

Дар Java Script шумо метавонед як элементро дар массив таввасути дастраси ба ба элемент бо истифода аз индекси он 
тағйир диҳед ва сипас ба он арзиши нав илова кунед.
   Мисол

```` Javascript
let array = [1, 2, 3, 4, 5];

// Changing the element at index 2 to a new value, for example, 10
array[2] = 10;

console.log(array); // Output: [1, 2, 10, 4, 5]

````
_____
## Creating an Array.
Using an array literal is the easiest way to create a JavaScript Array. 

````Javascript
   let arr = [item1,item2,...,itemn];
   ````

   ## Array methods.
  + pop();
  + shift();
  + push();
  + unshift();
  + concat();
  + slice();
  +  join();
  +  includes();
  +  indexOf();
  +  splice();
  +  toString();
  +  toReversed();
______
   + forEach();
   + map();
   + find();
   + filter();
   + reduce();
   + toSorted();
  _____
  ## Array method push().
   Дар ин метод танҳо дар охири  массив элементи нав илова мекунем.

````Javascript
let arr = [1,2,5,"Salom"];
 let add = arr.push(4,"Ali");
 console.log(add); ///6
 console.log(arr); ///[1,2,5,"Salom",4,"Ali"]
 ````
 ___


 ## Array method pop();

 Ин метод элементи охири массивро хориҷ мекунад.

 ````Javascript
  let arr = ["a","b","c","d"];
  console.log(arr.pop()); // d
  console.log(arr);  //["a","b","c"]
  ````
  ___

  ## Array method unshift()
  Ин метод дар аввали масив элементи нав дохил мекунад.

  ````Javascript
    let arr = [1,2,3];
    console.log(arr.unshift(5,6)); // 5
    console.log(arr); // [5,6,1,2,3]
    
````
____

## Array method shift();
Ин shift()усул элементи массиви якумро нест мекунад ва ҳамаи унсурҳои дигарро ба шохиси поёнтар "мегузаронад".  

````javascript
  let  arr= [1,2,3];
  let firstelement = arr,shift();
  console.log(firstelement); //1
console.log(arr); //[2,3]
````

____

## Array method toString()

Ин метод масивро ба сатр табдил медиҳад.

````Javascript
 let arr = [1,2,3];
 console.log(arr.toString()); // '1,2,3'
 ````

 ____


 ## Java Script array method indexOf();
   Дар ин метод мо индекси элементро меёбем.

   ````Javascript
   let arr = [1,2,"Naom",true];
   let index = arr.indexOf("2"); 
   console.log(index); //2
   console.log(arr.indexOf("Alo")); // -1
   ````
   _____

   ## Array method includes();
   Ин метод вазифаи  search ро мебозад. Агар элементи ворид гардидамон бошад true агар набошад   false  хориҷ мекунад.
````Javascript
   let arr = [1,2,"Naom",true];
   let is = arr.includes("2"); 
   console.log(is);//true
   ````
   ____
    
   ## Array method concat();
   Ин concat()усул массиви навро бо роҳи муттаҳид кардан (пайванд кардани) массивҳои мавҷуда эҷод мекунад:


   ````Javascript
     let arr1 = [1,2,3];
     let arr2 = [4,5,6];
     console.log(arr1.concat(arr2)); // [1,2,3,4,5,6]

````
___

   ## Array method slice();
    Ин метод ду параметр мегирад авалу охир.


    ````Javascript
    let arr= [1,2,3,4,5,6]
    ler sli = arr.slice(1,3);
    console.log(sli); //[2,3]

    ````
    ____

  ## Array method splice();
  Ин splice()усулро барои илова кардани ҷузъҳои нав ба массив истифода бурдан мумкин аст:

  ````Javascript

  let  arr = [1,2,3,true];
  let b = arr,splice(1,2, false);
  console.log(b); // deleted 2
  console.log(arr); //[1,false,3,true]
  ````

_____
 # Java Script Array methods callbacks.

## Java Script Array method map().
map() аз даъват кардани функсия барои ҳар як элементи массив массиви нав эҷод мекунад.
map() массиви аслиро тағир намедиҳад.
Усули map() массиви навро бо натиҷаи даъвати функсияи муайяншуда барои ҳар як элементи массив месозад.

````Javascript

 let arr = [1,2,2,3];
 let map1=arr.map((x)=>x*2)
   console.log(map1); ///[2,4,4,6]
   ````

   ____

   ## Java Script Array method forEach().
Усули forEach() функсияи муайяншударо барои ҳар як элемент дар ' як маротиба иҷро мекунад.
массив.   
   Методи forEach() 3 параметр қабул мекунад.
 +  Element
 +  index
 +  Array

````Javascript
 
 array.forEach(function(currentValue, index, arr), thisValue)

 ````
____
  ## Java Script Array method find().

  The find() method returns the value of the first element that passes a test.

The find() method executes a function for each array element.

The find() method returns undefined if no elements are found.

The find() method does not execute the function for empty elements.

The find() method does not change the original array.

  ````Javascript

  array.find(function(currentValue, index, arr),thisValue)

  ````
  ____

 ## Java Script Array method filter().
  Ин filter()усул массиви наверо эҷод мекунад, ки бо унсурҳое пур карда шудааст, ки аз санҷиши аз ҷониби функсия пешниҳодшуда мегузаранд.

Усул filter()функсияро барои элементҳои холӣ иҷро намекунад.

Ин filter()усул массиви аслиро тағир намедиҳад.
  

 ````Javascript
  
  let sum = 0;
const numbers = [65, 44, 12, 4];
numbers.forEach(myFunction);

function myFunction(item) {
  sum += item;
}

 ````
 ____


 ## Java Script Array method reduce().
Ин reduce()усул функсияи редукторро барои элементи массив иҷро мекунад.

Усул reduce()як арзиши ягонаро бармегардонад: натиҷаи ҷамъшудаи функсия.

Усул reduce()функсияро барои элементҳои массиви холӣ иҷро намекунад.

Ин reduce()усул массиви аслиро тағир намедиҳад.

 ### Синтаксис
 array.reduce(function(total, currentValue, currentIndex, arr), initialValue)

 Browser Support
reduce() is an ECMAScript5 (ES5) feature.

ES5 (JavaScript 2009) fully supported in all modern browsers since July 2013:
  
  ````Javascript

  const numbers = [175, 50, 25];

document.getElementById("demo").innerHTML = numbers.reduce(myFunc);

function myFunc(total, num) {
  return total - num;
}
````
____

## Java Script Array method toSorted().

ES2023 ин toSorted()усулро ҳамчун роҳи бехатари ҷудо кардани массив бидуни тағир додани массиви аслӣ илова кард.

Фарқи байни toSorted()ва sort() дар он аст, ки усули аввал массиви навро эҷод мекунад ва массиви аслиро бетағйир нигоҳ медорад, дар ҳоле ки усули охирин массиви аслиро тағир медиҳад.

  ````Javascript

const months = ["Jan", "Feb", "Mar", "Apr"];
const sorted = months.toSorted();    ////Apr,Feb,Jan,Mar
````
____

## Java Script Mechanism DESTRUCTURING.
  Destructuring  дар Java Script   барои ҷудо кардани сохторҳои массивҳо ва объектҳо мебошад, ки дар ин ҳолат
   ба осони ба арзтшҳои дохили онҳо дастраси пайдо мекунад.
   Destructuring   барои кушодани арзишҳо аз  массивзо ва объектҳо ба тағйирёбандаҳои гуногун кумвак мекунад,
   аз ин ру ба шумо лозим нест ки масивҳо ё объектҳои калонро кобед, то арзишҳои лозимара ба даст оред.

````Javascript
  let a, b, rest;
[a, b] = [10, 20];

console.log(a);
// Expected output: 10

console.log(b);
// Expected output: 20

[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
// Expected output: Array [30, 40, 50]

````
_____

   ## Java Script mechanism  Spread ...
    Оператори паҳнкунии Java Script (...) такроршавандаро (ба монанди массив) ба унсурҳои бештар васеъ мекунад.
     Ин ба мо имкон медиҳад, ки ҳама ё қисмҳои массиви мавҷударо ба массиви дигар зуд нусхабардори кунем.

     The spread (...) syntax allows an iterable, such as an array or string, 
     to be expanded in places where zero or more arguments (for function calls) or elements (for array literals)
      are expected. In an object literal, the spread 
      syntax enumerates the properties of an object and adds the key-value
       pairs to the object being created.

Spread syntax looks exactly like rest syntax. In a way, spread syntax is the opposite of rest syntax. Spread syntax "expands" an array into its elements, while rest syntax collects multiple elements and "condenses" them into a single element. See rest parameters and rest property.

  ````Javascript
  function sum(x, y, z) {
  return x + y + z;
}

const numbers = [1, 2, 3];

console.log(sum(...numbers));
// Expected output: 6

console.log(sum.apply(null, numbers));
// Expected output: 6
````

____
## Java Script mechanism  Spread (...)
Синтаксис остаточных параметров функции позволяет представлять неограниченное множество аргументов в виде массива.
## What Is the Spread Operator and How Does spread work in JavaScript?


The spread operator (...) helps you expand iterables into individual elements.
The spread syntax works within array literals, function calls, and initialized property objects to spread the values of iterable objects into separate items. So effectively, it does the opposite thing from the rest operator.


````Javascript
const myName = ["Sofela", "is", "my"];
const aboutMe = ["Oluwatobi", ...myName, "name."];

console.log(aboutMe);

// The invocation above will return:
[ "Oluwatobi", "Sofela", "is", "my", "name." ]
````