# curl-based-services

A curated, spot-checked list of useful services you can talk to with nothing but `curl` (or `nc`/`telnet`/`ssh` where noted) — no browser, no install, no signup.

Every HTTP(S) entry below was hit with a live `curl` request on 2026-08-13 before being added. Entries that didn't respond were left out rather than listed on faith. If something in here breaks later, please open an issue or PR — that's the whole point of keeping this list honest.

- [Money & Finance](#money--finance)
- [IP & Network](#ip--network)
- [Weather](#weather)
- [Documentation & Cheatsheets](#documentation--cheatsheets)
- [Text & File Sharing](#text--file-sharing)
- [Utilities](#utilities)
- [Fun](#fun)

## Money & Finance

* `curl stockchat.sh/AAPL` — full stock research terminal over curl: price, fundamentals, chart, news, and a free-text question mode (e.g. `curl "stockchat.sh/AAPL?q=how's the balance sheet"`). No signup for basic lookups. ([stockchat.sh](https://stockchat.sh))

## IP & Network

* `curl ifconfig.me` — your public IP, plain text
* `curl icanhazip.com` — your public IP, plain text
* `curl checkip.amazonaws.com` — your public IP, from AWS
* `curl ipinfo.io/ip` — your public IP, plain text
* `curl httpbin.org/ip` — your public IP, JSON

## Weather

* `curl wttr.in` or `curl wttr.in/Berlin` — weather report as ASCII art ([chubin/wttr.in](https://github.com/chubin/wttr.in))

## Documentation & Cheatsheets

* `curl cheat.sh/tar` — cheat sheets for pretty much any UNIX/Linux command or programming language ([chubin/cheat.sh](https://github.com/chubin/cheat.sh))

## Text & File Sharing

* `echo "hello" | curl -F file=@- 0x0.st` — anonymous file/text upload, returns a share link
* `curl -F url=https://example.com https://is.gd/create.php?format=simple&url=https://example.com` — URL shortener

## Utilities

* `curl qrenco.de/some-string` — generate a QR code as ASCII art ([chubin/qrenco.de](https://github.com/chubin/qrenco.de))
* `curl foaas.com/cool/you` — Fuck Off as a Service (NSFW)

## Fun

* `curl parrot.live` — animated party parrot ([hugomd/parrot.live](https://github.com/hugomd/parrot.live))
* `curl ascii.live/nyan` — animated Nyan Cat
* `curl icanhazdadjoke.com` — random dad joke
* `curl whatthecommit.com/index.txt` — random commit message generator
* `telnet mapscii.me` — zoomable ASCII world map (telnet, not curl)

---

## Contributing

PRs welcome. Please confirm your entry actually responds to a plain `curl` request before adding it, and note the date you checked it.

## License

[MIT](LICENSE)
