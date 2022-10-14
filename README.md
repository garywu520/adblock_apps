

By creating a Mac web application with specific User-Agent, ingeniously avoid advertising problems, such as: YouTube video ads, etc.



<br>


## Dependencies

- macOS 10.9+ / Windows / Linux
- Node.js ≥ 12.9 and npm ≥ 6.9

```bash
npm install -g nativefier

#nativefier版本更新
npm list -g --depth 0
npm update Nativefier
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
  --user-agent 'Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)'
```
<br>

## Maintain
When NativeFier's new Release is released, in order to ensure normal use, you may need to upgrade it as soon as possible.

<br>

## Tested User-Agent

Replace the following User-Agent

|      App      |                          User-Agent                          | Ad Removed | Hide Play |
| :-----------: | :----------------------------------------------------------: | :--------: | :--------: |
|    Youtube    | Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp) |    Yes     | Support |

As of now, the YouTube video ads have been removed.
For other web applications, please test it by yourself.

<br>

## License

[MIT.](https://github.com/garywu520/webapps-ads-removal/blob/main/LICENSE)
