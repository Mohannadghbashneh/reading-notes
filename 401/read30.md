# Next- Forms and Conditional Rendering 

## Reading:
#### WHAT IS MEMOIZATION?
- Memoization is an optimization technique for accelerating computer programs by caching the results of heavy function calls and returning them when similar inputs are encountered repeatedly. Simply, React memoization is similar to caching.

As an example, consider a long-running, sophisticated function that accepts input. To speed up this function execution, you can cache the results after executing it. So that, you can take the cached value without recomputing the value whenever you execute it again with the same inputs. Consequently, we can avoid unwanted rerenders for the same resultant output with the same set of inputs. We can capture the initial render result and cache it in memory for later use. This will boost app performance.

### Why use memoization in React?
- When props within a React functional component change, the whole component rerenders by default. To put it in another way, if a value inside the component changes, the entire component will rerender, along with all the functions or components whose values or props haven’t changed.

This will result in a performance pitfall, which can be avoided with memoization.

#### HOW TO IMPLEMENT MEMOIZATION IN REACT
- Both functional and class components benefit from memoization. React offers HOCs and hooks to implement this feature. We can use React.PureComponent within class components. Memoization for functional components is also possible with React.memo() HOC and useMemo() Hook. The useCallback() Hook is also there for caching functions instead of values.

#### MEMOIZATION USING PURECOMPONENT
- React.PureComponent helps us to implement memoization in a class component. PureComponent implements React.ShouldComponentUpdate(), which performs a shallow comparison of state and props and only renders the React component if the props or state have changed.

In this case, we have to keep the props and state as simple as possible. Since PureComponent may yield incorrect results if they include any advanced data structures. As PureComponent’s shouldComponentUpdate() avoids prop updates for the entire component subtree, we should also ensure that all PureComponent’s children are also PureComponent.


#### WHEN TO USE MEMOIZATION
- Memoization can increase performance for some functions. But, if we use it for every component rendering, it might decrease performance since it stores results that increase memory used for the program. We should only use memoization when there is a clear benefit for doing so.

#### What are the advantages of using a custom React JS hook?
- Reusability
- Readability
- Testability