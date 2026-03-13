> [!NOTE]
> Since this library was written, Issuu has switched to `reader4`, a SVG renderer. The Protobuf-based `reader3` API used by this library still appears to function, but switching to a different project that uses SVG rendering will likely be more stable and give more accurate results.

# issuu-better-pdf-downloader

* Inspired by [jakeactually](https://github.com/jakeactually/issuu)'s work
* A POC downloader that creates "true" PDF files, which contain real text and vector graphics
* Implementation of the Protobuf-based `.bin` page format
* Partial reimplementation of PDF rendering - excluding the following:
  * Links (requires a rework of the dimensions scaling - open a PR if interested in implementing)
  * Blend modes
  * Line layers
  * JPG pages

## Try it

```
npm install
npm start "https://issuu.com/issuu/docs/issuu_digitaltoolkit"
```
