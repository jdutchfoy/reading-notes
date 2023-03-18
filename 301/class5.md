# README.md

## Read Assignment 5

1.A single responsibility principle has each component do one thing. If the idea keeps growing, that component should be decomposed into smaller subcomponent

2.Building a static version is a way to implement your app once the component hierarchy has been decided 1Links to an external site.. It's the same as building components and their subcomponents passing in data using props, but without using state. The state is applied during the interactivity phase.3.

3.Once the static version that renders the app is built, the next step is adding interactivity; this is where the state comes in. The Minimal (but complete) Representation of UI Statewill be the next step 1Links to an external site.. Breaking down pieces of data and figuring out which needs state is essential.

Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

To identify what piece of data changes or needs to be updated. Input from forms, checkboxes, or text values from search bars. These data change over time and can't be computed from anything . The state needs to live inside its parent/grandparents’ components that will be able to pass down the data whenever its child components need it.

The higher-order function are functions that operate on other functions, either by taking them as arguments or by returning them 2Links to an external site.. Higher-order function allows us to either create new functions or change other functions.

The map() returns a new array by applying a function to all of its elements and building a new array from the returned values2Links to an external site.. It will have the same length as the original array, but its contents are now changed depending on the condition/code block of the function applied to it. The reduce() is mainly used to compute every single value of the array; it takes a single element from the array and combines it with the current value 2Links to an external site..
