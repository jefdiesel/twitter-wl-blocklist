# twitter-wl-blocklist

X (Twitter) accounts blocked from the DoorDab / Sullen Teens whitelist: bot farms and sybil accounts, caught by shared
IPs, shared wallets, X accounts made minutes apart and order bursts, then reviewed and blocked by hand.

- `blocklist.csv`: one row per blocked account (1233 accounts).
- `blocklist.txt`: just the handles, one per line.

| column | |
|---|---|
| `x_handle` | the handle when it last ordered (handles can change; `x_id` doesn't) |
| `x_id` | X's numeric user id |
| `x_signup_utc` | when the X account was made |
| `followers` | followers at its last X sign-in (blank if not recorded) |
| `wallets` | every wallet it ordered to or paid from, `;`-separated |
| `ip`, `ip_hash` | IPs it ordered from, and their hashes (same hash = same IP); raw IPs recorded from 2026-09-30 on |
| `country` | Cloudflare's country for its orders |
| `first_order_utc`, `blocked_utc` | when it first ordered, and when it was blocked |
