# AdGuard DNS Filter

A small personal DNS blocklist for AdGuard DNS / AdGuard Home.

- **Blocks:** Reddit, TikTok
- **Keeps working:** Facebook Messenger (explicitly allowlisted)

## Use it

In AdGuard, add a custom filter / blocklist with this URL:

```
https://raw.githubusercontent.com/romeothethird/adguard-dns-filter/main/filter.txt
```

- **AdGuard DNS (adguard-dns.io):** Dashboard → your server → *DNS blocklists* → *Add blocklist* → paste the URL.
- **AdGuard Home:** *Filters* → *DNS blocklists* → *Add blocklist* → *Add a custom list* → paste the URL.

## Edit it

Edit `filter.txt`, commit, and push. AdGuard re-downloads the list periodically (or click *Check for updates*).

Rule syntax:

| Rule | Meaning |
|------|---------|
| `\|\|example.com^` | Block `example.com` and all subdomains |
| `@@\|\|example.com^` | Always allow `example.com` and all subdomains |
| `! text` | Comment |

## License

MIT
