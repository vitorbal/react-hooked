# react-hooked

♻️ Useful custom hooks for react.

## Available Hooks

### `usePrevious`

Lets you reference the previous prop or state of a component:

```jsx
function Counter() {
  const [count, setCount] = useState(0);
  const prevCount = usePrevious(count);

  return (
    <h1>
      Now: {count}, before: {prevCount}
    </h1>
  );
}
```
