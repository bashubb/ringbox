# Ringbox website

Static site for `https://bashubb.com/ringbox/`: a coming-soon page, the privacy policy and support for App Store Connect. Publish the `docs/` folder of the GitHub repository `bashubb/ringbox` with GitHub Pages (Settings → Pages → main, /docs; leave Custom domain empty — the account's `bashubb.com` serves it under `/ringbox/`).

```sh
python3 -m http.server 8767 --bind 127.0.0.1 --directory docs
```

App source: `../../flahship bets/Ringbox/`. Facts on the pages (1:30 recording, 29 s alarm sound, three free sounds, AlarmKit, no third-party SDKs) come from the code — re-check them when those change.

Next: once the App Store listing exists, add the App Store link and `apple-itunes-app` meta, and swap the coming-soon pills for the badge.
