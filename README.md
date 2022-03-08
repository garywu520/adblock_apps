## Introduction

The older User-Agent terminals are no longer the mainstream advertising target, so you can use the "--user-agent" parameter of the nativefier open source tool to forcefully disguise User-Agent to achieve ad filtering. Of course, not most User-Agents can remove ads, you need to explore and test together.

<br>


## Dependencies

- macOS 10.9+ / Windows / Linux
- Node.js ≥ 12.9 and npm ≥ 6.9

```bash
npm install -g nativefier
```

From: https://github.com/nativefier/nativefier

<br>

## Usage

Use nativefier to generate Web as App, example:

```
/<Path>/nativefier "https://example.com" \
  --name Example \
  --tray \
  --internal-urls "(.*?)(accounts\.example\.com|example\.com)(.*?)" \
  --user-agent 'Mozilla/5.0 (xxxxxx)'
```

<br>

## Tested User-Agent

Replace the following User-Agent

|      App      |                          User-Agent                          | Ad Removed | Hide Play |
| :-----------: | :----------------------------------------------------------: | :--------: | :--------: |
|    Youtube    | Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp) |    Yes     | Support |
| Youtube-Music | Mozilla/5.0 (Macintosh; Intel Mac OS X x.y; rv:42.0) Gecko/20100101 Firefox/42.0 |    Yes     | Support |

Different User-Agent access APP interface will be different, it is automatically adjusted according to the terminal

<br>

**Other:**
- Submit suggestions to improve this project.
- If it involves infringement, please contact me to delete it in time.

<br>

## License

[MIT.](https://github.com/garywu520/webapps-ads-removal/blob/main/LICENSE)
