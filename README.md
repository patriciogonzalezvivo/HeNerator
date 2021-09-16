![](.github/thumbnail.gif)

# HeNerator 
A simple script to generate HeN ipfs app exports from any frag shader created with:

- [GlslViewer](https://github.com/patriciogonzalezvivo/glslViewer)
- [GlslEditor](http://patriciogonzalezvivo.github.io/glslEditor/)
- [The Book of Shaders](https://editor.thebookofshaders.com/)
- [glslCanvas VS extension](https://marketplace.visualstudio.com/items?itemName=circledev.glsl-canvas)

## How it works?

1. If you are using [GlslEditor](http://patriciogonzalezvivo.github.io/glslEditor/) or [The Book of Shaders's](https://editor.thebookofshaders.com/) on-line editor, download the file.
2. Excecute `henerator.py` follow with the `--title NAME` of your work and (optionally) the ```--duration SECONDS``` of the thumbnail GIF. If you don't set a duration it will use the first frame as an image.

```
./henerator.py test.frag --title ball --duration 2.5
```

3. That's all! Y ou should see a `heneration.zip` file in the same folder.

### Arguments 

* `--title [TITLE_NAME]`
* `--author [AUTHOR_NAME]` 
* `--width [WIDTH]` of the thumbnail
* `--height [HEIGHT]` of the thumbnail
* `--fps [FPS] ` of the thumbnail animation
* `--start [SECONDS] ` of the thumbnail animation
* `--duration [SECONDS] ` of the thumbnail animation
* `--pixel_density [PIXEL_DENSITY] ` of the thumbnail (in MacOS usually is 2)

## Requirements and Install

* Latest version of [GlslViewer](https://github.com/patriciogonzalezvivo/glslViewer/wiki/Compiling)
* [Ffmpeg](https://ffmpeg.org/download.html) (only required to make animated GIFs for your thumbnails)
* Python3 
* ArgParse and Requests modules for Python3 
 
```bash
pip3 install argparse requests
```

or 

```
sudo easy_install -U requests argparse
```

* You can install `henerator.py` globaly on your system by just typing 
```bash
make install
```
