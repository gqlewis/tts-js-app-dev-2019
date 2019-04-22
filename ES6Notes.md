/*//Template Literal

console.log(`Hello! I'm a string
continues on the next line`);

//Previous way
console.log("some string\n" + "string text2");
//this would move the strings to separate lines

const name = "Jimmy"
const day = "Wednesday"
const instructor = {
    name: "Chris", 
    lesson: "ES6",
    greet: function() {
        return `Hello ${this.name}, today we'll learn ${this.lesson}!`
    }
}

//ES5
console.log("Hello" + name + "I hope you have a great" + day);
//ES6
console.log(`Hello ${name} I hope ${day} goes well!`);
//interprolation
console.log(`Hello ${instructor.name}, today we'll learn ${instructor.lesson}!`);

console.log(instructor.greet());

function foo() {    
    let x = true;
    if (x) {
        var usingVar = "i'm using var";
        console.log(usingVar)
    }
}
foo();
//using let has more benefits, have more control over variables. It binds through the laxical scope. It won't be affected by closure. 

const instructors = ["Jimmy", "Chris"]
//instructors = ["Jim", "Christopher"] //would get a type error b/c instructors has already been defined
instructors.push("Jack", "Jill"); //this would add these names to the instructors array

//const also accepts uppercase or lowercase

//default parameters, lets you pass default argument to your functions
function hello(name = 'Mystery Person') {
    //name = name || 'Mystery Person';
    console.log(`Hello ${name} is it me your looking for`)
}
hello("Bobby");
hello();



// Arrow Functions
const teacher = {
    name: "Jim",
    speak: function() {
        let boundFunction = function() {
            console.log("later my name is " + this.name);
        }.bind.this;

        setTimeout(boundFunction, 10000)
    }
}
teacher.speak();
console.log(object)
*/
let students = ["boy", "girl", "alien"];
let [x,y,z] = students;
console.log(students);