# useCookie - React Hook

React Hook for Cookies based on [js-cookie](https://github.com/js-cookie/js-cookie)

## Instalation

```sh
npm install @use-hook/use-cookie --save
```

## Usage

```javascript
import { useCookie } from "@use-hook/use-cookie";

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

## License

[MIT](http://vjpr.mit-license.org)
