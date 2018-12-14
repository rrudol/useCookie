# useCookie - React Hook

React Hook for Cookies based on [js-cookie](https://github.com/js-cookie/js-cookie)

## Instalation

```sh
npm install useCookie --save
```

## Usage

```javascript
import { useCookie } from "useCookie";

function App() {
  const [name, setName] = useCookie("name", "Stefan");

  return (
    <div>
      <input
        type="text"
        placeholder="Provide your name"
        value={name}
        onChange={e => setName(e.target.value, { expires: 1 })}
      />
    </div>
  );
}
```

## Example

- [codesandbox.io](https://codesandbox.io/s/5v8x67nw8l)

## License

[MIT](http://vjpr.mit-license.org)
