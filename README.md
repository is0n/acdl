<h1 align='center'>acdl</h1>

`acdl` is a bash script that scrapes [AlphaCoders](https://wall.alphacoders.com) for wallpapers from the command line.
Unlike conventional scraping scripts, `acdl` allows you to select wallpapers before downloading them.
Heavily inspired by [waldl](https://github.com/pystardust/waldl).

## Concepts:
- `Command line` based
- `Few` dependencies (portable)
- `Fast` in both large and small sample sizes
- `Preview` and `select` images before downloading them

## Dependencies:
- [GNU Coreutils](https://www.gnu.org/software/coreutils)
- [curl](https://curl.se/)
- [sed](https://www.gnu.org/software/sed/)
- [grep](https://www.gnu.org/software/grep/)
- [rofi](https://github.com/davatorium/rofi) or [dmenu](https://tools.suckless.org/dmenu/) (both are optional)
- An image viewer (default is [sxiv](https://github.com/muennich/sxiv))

## Demonstration:
![Demonstration](https://gitlab.com/is0n/acdl/uploads/df1c305bf26fbb3150383d8d49e3c6aa/video.mp4)

## Usage:
See `acdl --help`.

## Configuration:
The following are the default configuration values:
```shell
img_viewer="sxiv"
viewer_opts="-tpo -z 200"
pages=1
output="${HOME}/Wallpapers/alphacoders"
cachedir="${HOME}/.cache/alphacoders"
silent=false
```
Modify any of these values in `$HOME/.config/acdlrc` to configure `acdl`

## Installation
- Automatic:

```shell
$ git clone https://gitlab.com/is0n/acdl
$ cd acdl
$ sudo make install
```

- Manual:

Add `acdl` to `$PATH`

## Uninstallation:
- Automatic:

```shell
$ sudo make uninstall
```

- Manual

```shell
$ sudo rm -f "$(which acdl)"
```
