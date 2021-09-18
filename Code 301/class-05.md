# Code 301 - Intermediate Software Development

## How would you break a mock into a component heirarchy?
- a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

## What is the single responsibility principle and how does it apply to components?
- The single-responsibility principle (SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part.

## What does it mean to build a ‘static’ version of your application?
-  Static applications and websites render in the user's browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies
## Once you have a static application, what do you need to add?
- Add Your New Site. 
- Link to Your GitHub (or supported version-control tool of choice)
- Authorize Netlify. 
- Select Your Repo. 
- Configure Your Settings. 
- Build Your Site. 
- All Done.

## What are the three questions you can ask to determine if something is state?
- is it daynamic ?
- is it need to declare in the variable ?
- is it functional ?

## How can you identify where state needs to live?
- render a Todo component (as triggered by the setState ) it will first check if the state has changed (via the props or state ). Assuming the state is different (which it will be because we made an explicit setState call) React will check the shouldComponentUpdate on the Todo component.


## Things I want to know more about
- [React Bootstrap - Forms](https://react-bootstrap.github.io/components/forms/)
