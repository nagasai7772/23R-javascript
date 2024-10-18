# 23R-javascript
                                                                  Questions Document
1. What will be the output?

 let x=5;
 let y=x;
 x=10;
  console.log(x); //output:10;
  console.log(y); // output:5;

Explanation: let y=x means y copies the x value which x=5||y=5
when x is updated ,the y still holds "x" old value, because y is primitive value(like numbers) are copied by value not reference.
Therefore x is updated to 10 but y reamins 5

2. What will be the output?

let obj1={name :"Alice"};
let obj2=obj1;
obj1.name="Bob";
console.log(obj1.name); //output:Bob;
console.log(obj2.name); //output:Bob;
Expalanation: obj2=obj1; means obj2 copies the obj1 reference
  Then obj1 is updated to obj1.name="Bob" 
  Then obj2 also references the same object,now both obj1.name & obj2.name will be same output "Bob"

3. let a="hello";
let b=42;
let c=true;
let d={key :"value"};
let e=null;
let f=undefined;
console.log(typeof a); // output string
console.log(typeof b); // output number
console.log(typeof c); // output Boolean
console.log(typeof d); // output object
console.log(typeof e); // output object
console.log(typeof f); // output undefined

Explanation:
1. `typeof a` is `"string"` because `a` holds a string value `"hello"`.
2. `typeof b` is `"number"` because `b` holds a numeric value `42`.
3. `typeof c` is `"boolean"` because `c` holds a boolean value `true`.
4. `typeof d` is `"object"` because `d` is an object.
5. `typeof e` is `"object"` because `null` is a special case in JavaScript where `typeof null` returns `"object"`.
6. `typeof f` is `"undefined"` because `f` is explicitly assigned as `undefined`.


4. let numbers=[10,20,30,40,50];
console.log(numbers[2]);                             //output:30;
console.log(numbers[0]);                            //output:10;
console.log(numbers[numbers.length-1]);             //output:50;


Explanation::
1. numbers[2] means index value[2], index always starts from 0 . so here 2nd value is 30
2. numbers[2] means index value[0], index always starts from 0 . so here 0 value is 10
3. numbers[numbers.length-1], here numbers.length means length of array, so numbers[numbers.length-1]
 calculates the last index of the array(here length is 5,so the last index is 4), which is last element it is 50.

5. let fruits=["apple","banana","mango"];
fruits[1]="orange";
console.log(fruits); //output :["apple","banana","mango"]

Explanation::
       The array fruits is intialized with ["apple","banana","mango"]
 Here we changing the index value fruits[1] replacing with "orange"
 Then it is updated with the new value, & the output will be displayed with updated array  

6. let matrix=[
               [1,2,3],
               [4,5,6],
               [7,8,9]
                      ];
console.log(matrix[1][2]);  //output: 6;
console.log(matrix[2][0]);  //output: 7;

Expalanation: 
  Here the matrix[1][2] means the second row (index 1) in third column (index 2) which is 6.
  Here the matrix[2][0] means the third row (index 2) in first column (index 0) which is 7.

7. let person={ name:"John", age:25, city:"New york"};
console.log(person.name);   //Output: John;
console.log(person.age);   //Output: 25;
  
  Explanation: 
  person.name access the name property of the person object which holds the value "John"
  person.age access the age property of the person object which holds the value 25         
 
 8. let car={ make:"Toyota",
                  model:"Corolla",
                   year:2021};
console.log(car["make"]); //Output:"Toyota";
console.log(car["model"]); //Output:"Corolla"

 Explanation:
         car["make"] access the name property of the car object using bracket notation which holds the value "Toyota"
         car["model"]access the model property of the car object using bracket notation which holds the value "Corolla"        
 
 9.     let book={ title:"The Great Gatsby",
             author:"F. Scott Fitzgerald"};       
             book.author="Anonymous";
              console.log(book.author);   //Output: Anonymous;

 Explanation:
            Here first we declare the object book ,property author is "F. Scott Fitzgerald"
            Then We updated the property book.author="Anonymous" with Anonymous.
            When we the run the ouput it will displays the updated value "Anonymous"

10. let student={ name:"Alice",grade:"A"};
          student.age=20;
       console.log(student); //Output: { name: 'Alice', grade: 'A', age: 20 }

       Explanation:
        First we declaring the object student with name as "Alice" and grade as "A"
        Then we adding  new property is student.age as age 20;
        When console.log(student); is called, it ouputs is the updated object and adds new object age property 
        also  { name: 'Alice', grade: 'A', age: 20 }


