# Next- Forms and Conditional Rendering
React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.

React Hooks and Custom Hooks
Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

## Custom Hooks
When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks. For example, useFriendStatus

Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return. In other words, it’s just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

Things to consider when working with custom hooks
Is this code equivalent to the original examples?

Yes, it works in exactly the same way. If you look closely, you’ll notice we didn’t make any changes to the behavior. All we did was to extract some common code between two functions into a separate function. Custom Hooks are a convention that naturally follows from the design of Hooks, rather than a React feature.

 **Do I have to name my custom Hooks starting with “use”?**

Please do. This convention is very important. Without it, we wouldn’t be able to automatically check for violations of rules of Hooks because we couldn’t tell if a certain function contains calls to Hooks inside of it.

Do two components using the same Hook share state?

No. Custom Hooks are a mechanism to reuse stateful logic (such as setting up a subscription and remembering the current value), but every time you use a custom Hook, all state and effects inside of it are fully isolated.

How does a custom Hook get isolated state?

Each call to a Hook gets isolated state. Because we call useFriendStatus directly, from React’s point of view our component just calls useState and useEffect. And as we learned earlier, we can call useState and useEffect many times in one component, and they will be completely independent.

## When to use Memoization
Memoization can increase performance for some functions. But, if we use it for every component rendering, it might decrease performance since it stores results that increase memory used for the program. We should only use memoization when there is a clear benefit for doing so.

# Summary
Memoization is an optimization feature in React which, when used in the right place, increases the performance of the program. React gives us PureComponent and memo to implement memoization. PureComponent is used with the class component and memo is used with the function component. Memoization increases performance by storing results for functions when the same prop is passed, hence reducing the number of re-renderings. But, overuse of memoization in places where there are not performance issues can result in reduction of performance.
