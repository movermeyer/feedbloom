# Feedbloom

Inspired by that annoying news channels bottom screen stripes shwoing the latest news.
It shows your RSS and Atom feeds at a single line in your terminal.

## Installing & Running

```
pip install feedbloom

```

Create a file named `feeds.txt` in `$HOME/.config/feedbloom` with a list of RSS or Atom URLs. Example:

```
echo "https://xkcd.com/atom.xml" >> $HOME/.config/feedbloom/feeds.txt
echo "https://pypi.python.org/pypi?:action=packages_rss" >> $HOME/.config/feedbloom/feeds.txt
```

To run, simply execute:
```
feedbloom
```

Feedbloom will get the last updated feeds from the list of entries and show them one at a time in the same line.


## TODO:
- Fix: New text does not owverwrite existing text if the last is longer.
- Fix: Text that is longer than 1 line don't have the first line flushed.
- Use with [i3wm](https://i3wm.org/)
- Add command line options for format, entries limit, feedfile path, and reader and printer times.
