![functions](https://github.com/nayaba/pw-lesson-08/assets/9198401/ee7aea10-234d-46be-846c-3ab97ae97883)

# Introduction to Functions

Alrighty, let’s kick back with a cool beverage and chat about one of the most useful parts of JavaScript: functions. Think of functions like your favorite fast-food combo meal — you have a bunch of ingredients that come together to make something delicious. In coding, a function is a set of instructions that performs a task or calculates a value. You can reuse it just like how you can order that same tasty combo meal whenever you're hungry.

### 1. What's a Function and Why Should I Care?

Imagine you’ve got a bunch of party tricks that you love to show off. Each trick is a hit at parties. Wouldn't it be handy to have those tricks ready to go at a moment’s notice, instead of having to plan them out each time? That’s what functions are for in JavaScript. They’re like your pre-packaged party tricks.

### 2. Creating Your First Function

Imagine you want to greet the world. You could go with:

```javascript
console.log("Hello, world!");
```

But what if you want to greet a specific person, and you want to do it several times? It would be quite tedious to type that out over and over again. That's where a function comes in handy:

```javascript
function greet() {
  console.log("Hello, world!");
}
```

With this function named `greet`, you've created a little machine that does the greeting job for you whenever you ask it to. To activate this machine, you use the function's name followed by parentheses:

```javascript
greet();

// Output:
// Hello, world!
```

Calling `greet()` will print "Hello, world!" to the console each time you use it. 

#### Calling (or Invoking) Your Function

In programming lingo, when you use a function, you can say you're calling it, invoking it, or even executing it. They all mean you're telling JavaScript, "Hey, go run that function I wrote!"

So when you write:

```javascript
greet();

// Output:
// Hello, world!
```

You're calling or invoking the `greet` function. It's like you're saying "Hey `greet`, do your thing!" and `greet` responds with a friendly "Hello, world!".

You can call `greet` as many times as you want, and it will perform its task every time:

```javascript
greet(); // Calls the function, prints "Hello, world!"
greet(); // Calls it again, prints "Hello, world!" again
```

Each call to `greet()` is like pressing a button on a machine that says 'Hello'—push the button, get a greeting. Simple as that! This is the beauty of functions; they make repetitive tasks a breeze and keep your code tidy. Now go ahead, try calling `greet` a few times and watch your greetings multiply.

### 3. Passing Information with Parameters

Greeting the world is cool, but let's get personal. We can tweak the `greet` function to say hello to anyone by using a parameter:

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}
```

Here, `name` inside the parentheses of `function greet(name)` is a parameter. Think of a parameter as a special variable that the function uses to work with the information you give it.

Now, when you want to greet someone specific, like your friend Nina, you call the function with an argument:

```javascript
let friend = "Nina";
greet(friend);
```

In this case, `friend` is the argument. When you invoke the `greet` function with `greet(friend)`, the argument `friend` takes the place of the parameter `name`. So inside the function, `name` effectively becomes "Nina", and the output will be:

```
"Hello, Nina!"
```

So remember, a parameter is a placeholder waiting inside the function, while an argument is the actual value you pass into the function when you call it. Parameters and arguments work together to make functions flexible and powerful. Now you can greet anyone by name without rewriting your greeting code!

### 4. Getting Fancy with Multiple Parameters

You can pass more than one piece of info to a function. Let’s add a time of day:

```javascript
function greet(name, timeOfDay) {
  console.log("Good " + timeOfDay + ", " + name + "!");
}
greet('Leia', 'afternoon'); // Outputs: Good afternoon, Leia!
```

### 5. Return: Giving Something Back

Sometimes you want your function to give you something back. For that, you use `return`. If you want to calculate something and need the result, `return` is your friend.

```javascript
function addNumbers(num1, num2) {
  return num1 + num2;
}
let sum = addNumbers(7, 3); // sum will be 10
```

When you `return` something, you can use it elsewhere in your code.

### 6. Function Expressions: Another Way to Write Functions

You can also define functions using expressions. This means creating an anonymous function and assigning it to a variable.

```javascript
const sayGoodbye = function(name) {
  console.log("Goodbye, " + name + "!");
};
```

Now `sayGoodbye` is a variable containing a function, and you can call it like this: `sayGoodbye('Han Solo');`.

### 7. Arrow Functions: Short and Sweet

Arrow functions are a shorthand way to write functions in ES6 (a version of JavaScript). They're great for short, single-action functions:

```javascript
const greet = (name) => {
  console.log("Hello, " + name + "!");
};
```

And if you have a really simple function that returns a value, you can skip the curly braces and the `return` keyword:

```javascript
const add = (a, b) => a + b;
```

### Practice Time!

Let's put what you’ve learned into action. Write a function that takes a number and returns its square (the number multiplied by itself).

```javascript
function square(number) {
  return number * number;
}

let squareOfFour = square(4); // squareOfFour will be 16
```

Type it out and play with it. Try different numbers, or maybe even try writing an arrow function version.

### Recap and What's Next

Functions are the workhorses of JavaScript. They keep your code organized and reusable, which is a blessing as your code grows in complexity. You’ve learned how to declare them, how to make them do your bidding, and how to get info back from them.

From here, you might explore more about scope (where variables and functions can be seen and used), or dive into higher-order functions (functions that operate on other functions, either by taking them as arguments or by returning them).

Grab another drink, pat yourself on the back, and keep coding! 🎉

[Back to the Wiki](https://github.com/nayaba/pw-wiki)
