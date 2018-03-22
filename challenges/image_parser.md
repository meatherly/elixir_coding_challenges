# Image Parser

In this challenge you'll take an PNG image and print out the height and width of the image. You can start with just hard coding the path to the image file to get you up and running.

## Example output
```
iex> ImageParser.parse("my_image.png")
iex> Name: my_image
ImageFormat: PNG
Height: 200px
Width: 200px
```

## Helpful links
 * [PNG specs](http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html)
 * [Elixir Binary Guide](https://elixir-lang.org/getting-started/binaries-strings-and-char-lists.html)
 * [Elixr Binary Docs](https://hexdocs.pm/elixir/Kernel.SpecialForms.html#%3C%3C%3E%3E/1)

## Extra challenges

* Create a cli app that takes that path of the image
* Return height and width for other image formats. JPEG, GIF, BPM, etc.

Credit to [@zabirauf](https://github.com/zabirauf) for writing an awesome [blog post](http://www.zohaib.me/binary-pattern-matching-in-elixir/) about parsing PNG images in Elixir!