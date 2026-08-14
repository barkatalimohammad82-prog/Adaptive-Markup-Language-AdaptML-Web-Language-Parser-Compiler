# AdaptML

**AdaptML (AML) — Adaptive Markup Logic**

A small experimental markup language that parses `.adaptml` files and compiles them into browser DOM elements.

## Pipeline

`.adaptml` → `AMLParser` → AST → `AMLCompiler` → DOM → `AMLRuntime`

## Quick start

This project uses native browser JavaScript and requires no build step.

1. Clone or download the repository.
2. Start a local server in the project directory, for example:
   `python -m http.server 8080`
3. Open `http://localhost:8080/`.
4. Edit `examples/hello.adaptml` and refresh.

> A browser normally does not execute `.adaptml` directly. The demo loads the file as text, parses it, and compiles it to DOM.

## Example

```xml
<adaptml version="1.0">
  <app name="Hello AdaptML">
    <screen id="home">
      <text value="Welcome to AdaptML!" />
      <button id="start" action="start">Start</button>
    </screen>
  </app>
</adaptml>
```

## API

```js
import { AMLParser } from "./src/AMLParser.js";
import { AMLCompiler } from "./src/AMLCompiler.js";
import { AMLRouter } from "./src/AMLRouter.js";
import { AMLRuntime } from "./src/AMLRuntime.js";
```

## Project status

Experimental educational language/runtime. It is not an HTML replacement or web standard.

## License

MIT
