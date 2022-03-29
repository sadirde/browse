# browse

browse is something like an init system for alternative frontends of various services. Its main task is to redirect links from some of the major sites on the Internet to more privacy-friendly alternatives. These are all sites that are supported at the moment:

* YouTube - Redirects to [Indivious](https://github.com/iv-org/invidious) or [Piped](https://github.com/TeamPiped/Piped)
* Twitter - Redirects to [Nitter](https://github.com/zedeus/nitter)
* Instagram - Redirects to [Bibliogram](https://sr.ht/~cadence/bibliogram/)
* TikTok - redirects to [ProxyTok](https://github.com/pablouser1/ProxiTok)
* Reddit - Redirects to [teddit](https://codeberg.org/teddit/teddit) or [libreddit](https://github.com/spikecodes/libreddit)
* Medium - Redirects to [Scribe](https://sr.ht/~edwardloveall/scribe/)

Most of the alternative services are hosted by multiple people and therefore have many instances. Which instance is chosen is determined randomly with each call.

## Setup

After the shell script has been downloaded, it only needs to be moved to a directory where executables are located, e.g. `/usr/local/bin/`:

```sh
sudo cp browse /usr/local/bin
```

## Usage

Whenever you get a link to one of the sites listed above, you can copy it and open it in the terminal with:

```sh
browse <link>
```

This will open one of the many corresponding instances in your default browser.

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