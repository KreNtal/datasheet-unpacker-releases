# DataSheet Unpacker

A **Windows** app for unpacking spritesheets: give it a spritesheet image and its
data file, get back every individual sprite as a separate image.

DataSheet Unpacker reads the **data file** exported alongside the image
(JSON, XML, or `.atlas`) to know exactly where each sprite is, so every cut
is pixel-precise — including rotated sprites and multi-image atlases.

## Download

Grab the latest `DataSheetUnpacker.exe` from the
[Releases](https://github.com/KreNtal/datasheet-unpacker-releases/releases)
page. No installation needed — just run it.

The app checks for updates on startup and can download and apply them for
you.

## Supported formats

**Currently supporting**:
- Spine2D spritesheets (via *.atlas*)
- TexturePacker spritesheets  (via *.json*)
- Pixi.js fonts (via *.xml*)

**Spritesheet image**: `.png`, `.webp`, `.jpg`/`.jpeg`, `.bmp`, `.tga`, `.tiff`

You can also load multiple data files and images at once — DataSheet
Unpacker matches each data file to its image automatically (using the
`meta.image` field for TexturePacker JSON exports, or by filename otherwise)
and extracts them all in one go.

## How to use

1. Drop your spritesheet image(s) and data file(s) onto the window (or
   browse for them).
2. Choose an output folder.
3. Click **Extract Sprites**.

## License

See [LICENSE.md](LICENSE.md). The app is free to download and use; the
compiled binary may not be redistributed, modified, or reverse engineered.

## Issues

Found a bug or have a feature request? Open an issue on this repository.
