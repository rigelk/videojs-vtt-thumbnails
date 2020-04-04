# videojs-vtt-thumbnails

Video.js plugin that displays thumbnails on progress bar hover, driven by external VTT files.  Based on [this JW Player spec](https://support.jwplayer.com/customer/portal/articles/1407439-adding-preview-thumbnails).

This plugin supports both sprited and single images. If more than one image is given per second, a single image among them will be used.

## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Installation

- [Installation](#installation)
- [Usage](#usage)
  - [`<script>` Tag](#script-tag)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
## Installation

```sh
npm install --save videojs-vtt-thumbnails
```

## Usage

To include videojs-vtt-thumbnails on your website or web application, use any of the following methods.

### `<script>` Tag

This is the simplest case. Get the script in whatever way you prefer and include the plugin _after_ you include [video.js][videojs], so that the `videojs` global is available. Don't forget to include the CSS file too.

```html
<script src="//path/to/video.min.js"></script>
<script src="//path/to/videojs-vtt-thumbnails.min.js"></script>
<script>
  var player = videojs('my-video')
  player.vttThumbnails({
    src: 'example/thumbs.vtt',
    baseUrl: 'http://localhost:9000' // optional. if not, example/ will be used as baseUrl, if the .vtt sub-files are not FQ URLs.
  })
</script>
```

## License

MIT. Copyright (c) Chris Boustead &lt;chris@forgemotion.com&gt;


[videojs]: http://videojs.com/
