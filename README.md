# github-corners

[![NPM](https://nodei.co/npm/github-corners.png)](https://nodei.co/npm/github-corners/)

[![NPM version](https://img.shields.io/npm/v/github-corners.svg)](https://www.npmjs.com/package/github-corners)

Embed script for [Tim Holman](https://github.com/tholman)'s [Github Corners](http://tholman.com/github-corners).

## Installation

Include the [embed script](https://unpkg.com/github-corners/dist/) from the [unpkg](https://unpkg.com) CDN in your page:

```html
<!-- placed preferably before the closing `<body>` tag -->
<script src="https://unpkg.com/github-corners/dist/embed.min.js"></script>
```

It's recommended that you specify a [version](https://registry.npmjs.org/github-corners) or you may experience breaking changes:

```html
<!-- replace `latest` with a version like `0.1.0` -->
<script src="https://unpkg.com/github-corners@latest/dist/embed.min.js"></script>
```

## Usage

So the GitHub Corner renders on your page. Great! But how do I specify a link?

You can set it using the `data-href` attribute:

```html
<script data-href="https://github.com/tholman/github-corners" src="https://unpkg.com/github-corners/dist/embed.min.js"></script>
```

Now what if I want the link to open in a new tab?

Set `data-target` to `_blank`:

```html
<script data-href="https://github.com/tholman/github-corners" data-target="_blank" src="https://unpkg.com/github-corners/dist/embed.min.js"></script>
```

And what if I want to change the color or position of the corner?

You can always override the default styling of the svg:

```html
<!-- placed preferably after the embed script -->
<style>
.github-corner > svg {
  fill: skyblue;
}
</style>
```

## License

[MIT](LICENSE)

See [license/acknowledgements](https://github.com/tholman/github-corners#licenseacknowledgements) from original project.
