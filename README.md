# Privacy-aggressive Unbound config

Features:
 - cloudflare DNS-over-TLS upstream
 - basic adblocking
 - strong DNSsec config
 - drop IPv6 records
 - minimal responses
 - no log
 - block dns rebinding attack (examples.conf)
 - whitelist by ip (examples.conf)
 - forward private tld (for example, `.local`) to authoritative server (local-zone.conf)

Notes:
 - update DNSSEC root servers key with `unbound-anchor -a /var/lib/unbound/root.key`
 - `unbound-control-setup` to generate keys
