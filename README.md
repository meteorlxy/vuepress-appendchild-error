
### Install dependencies

```sh
yarn
```

### Reproduce the bug

```sh
yarn bug
```

Open the browser dev-tool to check the console:

```
DOMException: Failed to execute 'appendChild' on 'Node': This node type does not support this method.
```

The pre-rendered `dist_bug/index.html` includes:

```html
<div class="theme-default-content content__default"><!----></div>
```

### Try out the workaround

```sh
yarn workaround
```

Open the browser dev-tool to check the console, and the error disappears.

The pre-rendered `dist_workaround/index.html` includes:

```html
<div class="theme-default-content content__default"></div>
```

If we manually delete the `<!---->` in the `dist_bug/index.html`, the error will disappear, too.
