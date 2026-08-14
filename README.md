# AdaptML — Adaptive Markup Lgic

AdaptML is a custom web markup language that compiles `.adaptml` / `.aml` files into browser-ready HTML.

## Project

- `parser.js` — parses AdaptML into an AST
- `compiler.js` — compiles AST to HTML
- `router.js` — simple client-side route resolver
- `examples/hello.adaptml` — example source
- `docs/index.html` — documentation/landing page

## Quick start

```bash
node compiler.js examples/hello.adaptml
```

The compiler prints generated HTML to stdout.

## Example

```xml
<!DOCTYPE adaptml>
<AdaptML Version="1">
  <page title="My AdaptML Website">
    <header>
      <brand>AdaptML</brand>
    </header>
    <main>
      <h1>Hello AdaptML</h1>
      <text>यह मेरी AdaptML website है।</text>
      <button id="startButton">Start</button>
    </main>
    <footer>
      <text>Powered by AdaptML</text>
    </footer>
  </page>
</AdaptML>
```

## License

MIT
