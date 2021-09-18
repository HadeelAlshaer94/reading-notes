# Code 301 - Intermediate Software Development
## React and Forms 

## 1 - What is a ‘Controlled Component’?

![React](https://pbs.twimg.com/media/EKzwxZ4WkAAwjlw.jpg)

- A controlled component is a component that renders form elements and controls them by keeping the form data in the component's state.

- In a controlled component, the form element's data is handled by the React component (not DOM) and kept in the component's state. A controlled component basically overrides the default behavior of the HTML form elements.

## 2- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

- In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

## How do we target what the user is entering if we have an event handler on an input field?

- Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

- With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too,

## The Conditional (Ternary) Operator Explained

## 1 - Why would we use a ternary operator?

- Shorten your if statements into one line of code with the conditional operator
- Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

## 2 - Rewrite the following statement using a ternary statement
```html
 if(x===y){
      console.log(true);
      } else {
      console.log(false);
      }
      x === y ? true: false
```

![React](https://elzero.org/wp-content/uploads/2020/10/ternary-conditional-operator.png)