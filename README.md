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

## Contributing

We use [`commitizen`](https://github.com/commitizen/cz-cli) and [`standard-version`](https://github.com/conventional-changelog/standard-version) for automating our release and changelog process:

- Commit using `commitizen` to follow the [Conventional Commits Specification](https://conventionalcommits.org/).
- Release using `standard-version` for automatic versioning and CHANGELOG generation.

```bash
# add files to be commited
git add .
# commit using `commitizen`
yarn cz
# bump version and regenerate CHANGELOG based on commit messages
yarn release
# publish
git push --follow-tags origin master && npm publish
```
