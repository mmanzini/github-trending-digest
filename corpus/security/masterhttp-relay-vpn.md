# MasterHttpRelayVPN

A domain-fronted HTTP/SOCKS5 proxy that tunnels traffic through Google Apps Script with MITM TLS interception, HTTP/1-2 multiplexing, and DPI evasion techniques.

- **Repo:** [masterking32/MasterHttpRelayVPN](https://github.com/masterking32/MasterHttpRelayVPN)
- **Stars:** ~921 (2026-04-24, 4 days after launch)
- **Created:** 2026-04-20
- **Language:** Python
- **Topics:** dpi, http, mitm, proxy, sni, vpn

## Why It Matters
- Domain fronting via Google Apps Script is a well-established censorship circumvention technique — routing through Google infrastructure makes blocking expensive for network operators.
- DPI evasion (SNI manipulation) targets deep-packet inspection systems used in high-censorship environments.
- Python implementation makes it accessible; SOCKS5 support means it integrates with most client software.

## Key Takeaways
- Dual-use tool: legitimate censorship circumvention in restricted regions vs. potential abuse for traffic obfuscation.
- Google Apps Script as the relay: free, globally distributed, and harder to block without blocking Google itself.
- MITM TLS interception built-in — inspect your own traffic or use in a controlled lab; risky in adversarial contexts.
- Trends alongside other DPI-evasion tools; censorship circumvention remains a consistently high-interest GitHub vertical.

## Related
- [[redsun]]
