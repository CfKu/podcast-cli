# podcast-cli
podcast-cli - Some shell / bash scripts to search in and extract the audio links of (itunes-) podcast feeds

## Getting Started

Copy the podcast-* scripts on your local machine, maybe in your bin-folder. Maybe chmod +x is required.

### Dependencies

* [GNU grep](https://www.gnu.org/software/grep/)

On macOS via brew (is installed as ggrep):
```bash
$ brew install grep
```
On Windows you can use git bash / msys, gnuwin32 or similar shell ports.

### Minimal examples
```bash
$ podcast-itunes-id-to-url 646330750
http://feeds.feedburner.com/methodischinkorrekt

$ podcast-itunes-search methodisch inkorrekt
Methodisch inkorrekt
 >>> http://feeds.feedburner.com/methodischinkorrekt
 
$ podcast-rss-to-audio "http://feeds.feedburner.com/methodischinkorrekt"
http://feedproxy.google.com/~r/Methodischinkorrekt/~5/ [...]
[...]
```
The audio links can then be copied in your music player.

## License
This project is licensed under the terms of the MIT license - see the [LICENSE](LICENSE) file for details.
