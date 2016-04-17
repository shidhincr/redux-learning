## From State to Store

In our last example, we used the React component's internal state to manage the view. ie,  whenever the the counter value changes, we call the `setState()` method and it triggers a re-rendering of the view.

There are couple of disadvantages for this approach. First, if you want another component to be changed based on the counter value, you cannot do it. Because the counter value is an internal state of the Counter component. Traditional and recommended way to solve this issue is to wrap the two component into a parent component and keep the counter value in the parent component's state.

But, this is will get messed up when you want to communicate any changes to the parent component. That's when you need the **Flux** pattern. Because, you need to notify the parent component to re-render -- by triggering `actions`.

**Flux** introduced the concepts of stores, actions and action dispatchers. **Redux** simplified it by having one single store to have the whole application state, and multiple reducers to modify different part of the store.

