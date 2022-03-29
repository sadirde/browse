# browse

## Setup

After the shell script has been downloaded, it only needs to be moved to a directory where executables are located, e.g. `/usr/local/bin/`:

```sh
sudo cp browse /usr/local/bin
```

## Usage

Whenever you get a YouTube or Twitter link sent to you, you can copy it and call it in the terminal with

```sh
browse <link>
```

This will open one of many Invidious or Nitter instances in your default browser.

You can find the list of all instances in the shell file at the top. You can always remove some unwanted ones or add new ones.

## Examples

```sh
browse https://www.youtube.com/watch?v=ks_qOI0lzho
browse https://youtu.be/p_hgRLp-y_s
browse https://www.youtube.com/results?search_query=invidious

browse https://twitter.com/search?q=nitter
browse https://twitter.com/jack
```
**Disclaimer**
If there is a special character like `&` in the link, it (the whole link) should be enclosed in quotation marks.

## License

browse is free and open-sourced software licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl.html).