# ImageMagick Action

A GitHub action to edit your images with [ImageMagick](https://imagemagick.org/).
With [ImageMagick](https://imagemagick.org/)

> Use ImageMagick® to create, edit, compose, or convert bitmap images. It can read and write images in a variety of formats (over 200) including PNG, JPEG, GIF, HEIC, TIFF, DPX, EXR, WebP, Postscript, PDF, and SVG. ImageMagick can resize, flip, mirror, rotate, distort, shear and transform images, adjust image colors, apply various special effects, or draw text, lines, polygons, ellipses and Bézier curves.

```yml
- name: ImageMagick Action
  uses: jruipinto/ImageMagick-action@master
  with:
    # ImageMagick command to be executed
    command: mogrify -path /my-path -auto-orient -resize 800x450 *.* # default is mogrify -path /images -auto-orient -resize x500 *.*
```

This action uses `mogrify` at its core. To understand more about the tool and how to define dimensions read this [guide on mogrify](https://imagemagick.org/script/mogrify.php)

### Sample usage

[Check out a sample of how to use this action](https://github.com/jruipinto/website-bem-da-terra/blob/master/.github/workflows/scully-publish-to-gh-pages.yml)
