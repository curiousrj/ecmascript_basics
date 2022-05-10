# ecmascript_basics
variables - var, let, const</br>
</br>
declairing function in object</br>
walk: function() {},</br>
walk() {},</br>
</br>
geting value from objects</br>
objectname.variable</br>
objectname.function()</br>
objectname['variable']</br>
</br>
in object method this refers the object</br>
in html element this refers the element</br>
alone/in function this refers to the global object</br>
js module by default is in strict mode</br>
in a function, in strict mode this is undefined</br>
methods like call(), apply(), and bind() can refer this to any object</br>
with bind() method one object can borrow a method from another object</br>
</br>
arrow function -</br>
functionName = parameter => body;</br>
functionName = () => body;</br>
in arrow function this inherits parent this</br>
const person = {</br>
    talk() {</br>
        let self = this;</br>
        setTimeout(() => {</br>
            console.log("this", this);</br>
        }, 1000);</br>
    }</br>
};</br>
person.talk();</br>
</br>
map() method -</br>
creates a new array from calling a function for every array element</br>
const names  = [ "Rohit", "Rahul" ];</br>
const copiedNames = names.map((name)=> name);</br>
console.log(copiedNames);</br>
</br>
back-ticks -</br>
defines string with more easy and useful way</br>
const id = {name: "Rijaul Sk", age: 22};</br>
console.log(`Hi I'm "${id.name}" and I'm "${id.age}"`);</br>
</br>
destructuring -</br>
const person = {</br>
    name: "Steve Roger",</br>
    age: 35,</br>
};</br>
const {name: personName, age: personAge} = person;</br>
console.log(personName,personAge);</br>
</br>
spread operator -</br>
const places1 = ["Kolkata", "Bengaluru"];</br></br>
const places2 = ["Chennai", "Delhi"];</br>
const places = [...places1, ...places2];</br>
console.log(places);</br>
</br>
const personName = {name: "John"};</br>
const personAge = {age: 35};</br>
const person = {...personName, ...personAge};</br>
console.log(person);</br>
</br>
class & constructor</br>
class Person {</br>
    constructor(name) {</br>
        this.name = name;</br>
        function run() {</br>
            console.log(`${name} is Running`);</br>
        }</br>
        run();</br>
    }</br>
}</br>
const person = new Person("Rijaul");</br>
</br>
modules -</br>
named export -</br>
export const name = "Joe";</br>
at bottom</br>
export {name, age};</br>
</br>
derfault export -</br>
export default function running() {</br>
console.log("Running");</br>
};</br>
at bottom</br>
export default running;</br>
