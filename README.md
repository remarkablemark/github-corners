# github-corners

[![NPM](https://nodei.co/npm/github-corners.png)](https://nodei.co/npm/github-corners/)

[![NPM version](https://img.shields.io/npm/v/github-corners.svg)](https://www.npmjs.com/package/github-corners)

:octocat: [Github Corners](http://tholman.com/github-corners) embed script inspired by [Tim Holman](https://github.com/tholman).

### Examples

- [JSFiddle](https://jsfiddle.net/remarkablemark/f19eejcb/)
- [Replit](https://replit.com/@remarkablemark/Github-Corners)

## Usage

Include the [embed script](https://unpkg.com/github-corners/) on your webpage:

```html
<!-- insert before `</body>` -->
<script src="https://unpkg.com/github-corners/dist/embed.min.js"></script>
```

Specify a [version](https://registry.npmjs.org/github-corners) to prevent breaking changes:

```html
<!-- replace `latest` with a version like `0.1.0` -->
<script src="https://unpkg.com/github-corners@latest/dist/embed.min.js"></script>
```

Improve page loading with `async` or `defer` attribute:

```html
<script
  async
  defer
  src="https://unpkg.com/github-corners/dist/embed.min.js"
></script>
```

## FAQ

The GitHub Corner renders on your page. Great! But how do I specify a link?

Set it with the `data-href` attribute:

```html
<script
  data-href="https://github.com/remarkablemark/github-corners"
  src="https://unpkg.com/github-corners/dist/embed.min.js"
></script>
```

What if I want the link to open in a new tab?

Set `data-target` to `_blank`:

```html
<script
  data-href="https://github.com/remarkablemark/github-corners"
  data-target="_blank"
  src="https://unpkg.com/github-corners/dist/embed.min.js"
></script>
```

Can I change the `aria-label` of the link?

Yes, the `data-label` value will override the default value:

```html
<script
  data-label="Check out the GitHub Corners repository!"
  data-href="https://github.com/remarkablemark/github-corners"
  src="https://unpkg.com/github-corners/dist/embed.min.js"
></script>
```

What if I want to change the color or position of the corner?

You can always override the default styling of the svg:

```html
<!-- insert after embed script -->
<style>
  .github-corner > svg {
    fill: skyblue;
  }
</style>
```

## License

[MIT](LICENSE)

See [license/acknowledgements](https://github.com/tholman/github-corners#licenseacknowledgements) from original project.
