# unturned dedicated server hosting: real prices from $99 dedicated boxes vs $4 panel plans, plus the GSLT and SteamCMD setup most guides skip

Search "unturned dedicated server hosting" and you land between two very different products. Game panel hosts sell managed Unturned slots at $2.50–4.00 per month. Dedicated server providers rent you an entire physical machine, where Unturned is just one of the things it can run. Both are legitimate answers; which one fits depends on your player count, whether you run RocketMod plugins, and how many server instances you want out of one box.

This article walks through both paths with verified prices, then covers the setup details most listicles skip: the GSLT token, the two different Steam App IDs everyone mixes up, and the port math that trips people running a second instance.

> **Quick pick:** if you're hosting 20+ players, running a RocketMod or RP server, or want multiple instances from one machine, a dedicated box is the better tool. Sharktech's current promo line starts at **$99/month** for an 8-thread Xeon with 16GB RAM, free setup and built-in DDoS protection — 👉 [check Sharktech's current dedicated server deals](https://bit.ly/SharKtech)

## What "dedicated" actually means for Unturned

Unturned ships its own server tool — Unturned Dedicated Server (U3DS) — installed and updated through SteamCMD. That means any machine with a public IP, two open UDP ports and enough RAM can host the game. The real question behind "unturned dedicated server hosting" is who else shares that machine, and who's responsible when something breaks at 3 a.m.

A few ground rules from the official knowledgebase worth knowing before you spend anything:

- Every internet-facing server needs a valid **GSLT (Game Server Login Token)** to appear in the server browser. No token, no listing — players could only join by direct IP.
- The game listens on **UDP 27015** by default, and automatically uses **27016** for server list queries. Plan for both.
- Self-hosting from home requires port forwarding on your router; a rented server with a public IP skips that entirely.

Home hosting is free, and for two or three friends it's fine. The tradeoffs are upload bandwidth, your PC staying on 24/7, and a residential IP that changes. Renting exists to remove all three.

## Panel plans vs a dedicated server: the honest comparison

Panel game hosting and dedicated servers overlap on this keyword, so here's how they actually differ. Sparked Host's Unturned page (a typical panel provider) lists three tiers: Stick at **$2.50/mo** (2GB RAM, 1 vCPU, 50GB storage), Log at **$3.25/mo** (3GB RAM, 2 vCPU), and Plank at **$4.00/mo** (4GB RAM, 2 vCPU). They support RocketMod, OpenMod and uScript, offer a 24-hour free trial, and refund Unturned game hosting in full within 48 hours of purchase — though notably, their VPS and dedicated server products are excluded from refunds. Add-ons cost extra: managed game server support runs $20/mo, a dedicated IP is $3/mo.

|  | Panel game hosting | Dedicated server (Sharktech) |
| --- | --- | --- |
| Entry price | $2.50–4.00/mo | $99/mo promo, from $219/mo configurable |
| RAM | 2–4GB shared | 16–32GB+ dedicated |
| Root access | No — panel only | Full root, hardware-level |
| Extra instances | Pay per plan | Run as many as hardware allows |
| DDoS protection | Varies by provider | 60Gbps automatic, included |
| Setup effort | Point-and-click | You install U3DS yourself |
| Trials/refunds | 24h trial, 48h refund | No published refund terms — ask first |

The panel path is genuinely the right call for small friend groups. A 4GB plan runs a vanilla server comfortably, someone else handles updates, and if it doesn't work out you get your money back within two days.

The dedicated path makes sense when the math changes. If your community has outgrown 4GB, wants multiple instances (each extra panel plan is another $3–4/mo forever), or you want to tinker with plugins and configs at the OS level, one $99 box with 16GB does the work of four panel plans at a comparable monthly total — with root access the panel never gives you.

## Sharktech's dedicated server lineup and prices

Sharktech sells dedicated servers through two channels, and it helps to see them separately. The main catalog is a configurable bare-metal line: every server ships with a **10Gbps port, 300TB of monthly bandwidth and 2TB NVMe M.2 storage** standard, with CPU, memory and drive layout customized per order — listed configurations start at **$219/month before upgrades**. In-stock systems target delivery within 24 hours; fully custom builds take one to two weeks.

The second channel is a promotions page with fixed configurations at much lower prices. These are the ones most Unturned server owners actually buy:

| Configuration | CPU / RAM | Storage | Network | Price/mo | Order |
| --- | --- | --- | --- | --- | --- |
| E3-1270v5 (Chicago or LA) | 8 threads @ 3.6GHz / 16GB | 2TB HDD or 120GB SSD | 1Gbps, 30TB/mo, 5 usable IPs | **$99** (was $159, code v5LACHI) | [ Order the E3-1270v5 promo](https://bit.ly/SharKtech) |
| E3-1270v2 unmetered (LA) | 8 threads @ 3.5GHz / 16GB | 2TB HDD or 120GB SSD | 1Gbps unmetered | **$99** (code LA1G) | [ Order the LA unmetered box](https://bit.ly/SharKtech) |
| Dual E5-2637v2 (Chicago, Denver or LA) | 16 threads @ 3.5GHz / 32GB | 2TB HDD or 120GB SSD | 1Gbps, 30TB/mo | **$183.20** (code New2637v2) | [ Order the Dual E5-2637v2](https://bit.ly/SharKtech) |
| Dual E5-2670 unmetered (Amsterdam) | 32 threads @ 2.6GHz / 32GB | 2TB HDD or 120GB SSD | 1Gbps unmetered | **$159** | [ Order the Amsterdam Dual E5-2670](https://bit.ly/SharKtech) |
| Dual E5-2670 unmetered (Chicago) | 32 threads @ 2.6GHz / 32GB | 2TB HDD or 120GB SSD | 1Gbps unmetered | $169 (code E51Gchi) | [ Order the Chicago Dual E5-2670](https://bit.ly/SharKtech) |
| 10Gbps unmetered E3-1270v2 (Amsterdam) | 8 threads @ 3.5GHz / 16GB | 2TB HDD or 120GB SSD | 10Gbps unmetered | **from $269** | [ Order 10Gbps unmetered](https://bit.ly/SharKtech) |

All plans are billed monthly. Promo prices and codes come from Sharktech's own promotions hub, and they do change — treat the table as a snapshot and confirm the current rate at checkout.

A few things bundled in that matter for game servers:

- **DDoS protection up to 60Gbps comes standard on every server**, with a paid upgrade path to 100Gbps cloud protection. Public Unturned servers get attacked — someone always has a botnet and a grudge — and many budget hosts sell this separately.
- Promo servers include a **/29 IPv4 allocation (5 usable IPs)** plus free IPv6, which is generous; five IPs means room for a second game server, a website, or a voice server on separate addresses.
- **Free setup** on the promo line, plus 24/7 support and Sharktech's SECURE management platform.
- Five datacenter locations: Las Vegas, Los Angeles, Denver, Chicago and Amsterdam. Stock varies by location; sold-out configurations simply won't appear at checkout.

One caveat worth quoting directly, because it affects game server admins who care about tick rate: "Port capacity describes the connection speed; actual throughput depends on the traffic path and workload." A 10Gbps port is a ceiling, not a guarantee.

For market context, third-party pricing roundups put entry-level dedicated servers at roughly $40–80/mo and mid-range enterprise hardware at $200–500/mo — but they also warn that setup fees, bandwidth overages and DDoS protection sold as add-ons can quietly turn a "$189 server" into a $280 one. A recent Sharktech-vs-OVH comparison made the same point: OVH's Rise line starts cheaper (around $70/mo with newer CPUs), but the cheapest plans cap public bandwidth at 500Mbps and only waive the setup fee with a 12-month commitment. Whether Sharktech's bundle-everything pricing wins depends on which of those fine prints annoys you more.

👉 [Browse Sharktech's full bare-metal catalog and current promo prices](https://bit.ly/SharKtech)

## Setting up Unturned on a dedicated server: the real steps

Panel hosts automate everything below. On a dedicated box you do it once, yourself, and it takes maybe half an hour. Here's the actual sequence for a Linux server.

**1. Install U3DS via SteamCMD.** Log in anonymously — no game account needed for the server tool — and pull the dedicated server build:


steamcmd +login anonymous +app_update 1110390 validate +exit


That App ID — **1110390** — is where a lot of guides get sloppy. It's the Unturned *Dedicated Server tool*. The number **304930** is the game client itself, and it's the one you'll need later for your GSLT token. They are not interchangeable.

**2. First launch.** The files land in `steamapps/common/U3DS`. Start it once:


./ServerHelper.sh +InternetServer/MyServer


Then shut it down cleanly with the `shutdown` command once it finishes loading. That first clean shutdown generates the config files you're about to edit.

**3. Configure via Commands.dat.** Each line is one command. The essentials:


Name My Unturned Server
Port 27015
Map Russia
Perspective Both


`Map` accepts PEI (default), Washington, Russia, or any workshop map you've placed in the server's Workshop folder. If you set a `Password`, know that the game only SHA1-hashes it — don't reuse a password that matters anywhere else. Full gameplay rules live in `Config.json`, which mirrors the in-game singleplayer config menu.

**4. Get your GSLT token.** Generate one from your Steam game server account page using App ID 304930, with a memo so you remember which server it belongs to. Your Steam account needs to be verified (not a limited account) to create tokens. Set the token in your server configuration alongside `fake_IP true` — without a valid GSLT the server will run but never appear in the browser list, which is the single most common "why can't anyone find my server" problem.

**5. Load workshop maps.** Curated maps install through `WorkshopDownloadConfig.json` — add File IDs to the list, and players download the map automatically on connect. Common ones: France (1975500516), Elver (2136497468), Kuwait (2483365750), Rio de Janeiro (1821848824), Greece (1702240229).

**6. Automate updates.** SteamCMD installs don't auto-update, so a cron job rerunning `+app_update 1110390` before your scheduled restart keeps the server current without 2 a.m. manual patching.

**Running multiple instances:** change the ServerID (`+InternetServer/SecondServer`) and give each instance its own port — 27017 for the second one, since the first instance quietly occupies 27015 and 27016. Save data lives in `U3DS/Servers/ServerID`, so instances stay separated automatically. This is where a 16GB dedicated box earns its keep; two or three instances on one machine is routine.

One legal footnote: Valve's Server Monetization Policy is in effect for Unturned, so if you plan to sell VIP ranks or items, read it before building your economy around it.

👉 [Get a dedicated box with full root access and set this up your way](https://bit.ly/SharKtech)

## Who shouldn't rent a dedicated server

Some honesty before the FAQ, because a $99/mo box is wasted money on the wrong person.

If your server is a private vanilla world for under ten friends, a $2.50–4.00 panel plan is strictly better for you: cheaper, someone else handles maintenance, and the 48-hour refund means trying one costs almost nothing. If you've never touched a Linux terminal and have no interest in learning, managed panel hosting (or Sparked's $20/mo management add-on style services) will save you real frustration. And if you want a trial period before committing, panel hosts offer 24-hour trials; Sharktech doesn't publish refund or trial terms on the pages checked, so ask their support directly before paying if that's a dealbreaker.

The dedicated box is for the second stage of a server's life: a real community, plugins, multiple instances, and the desire to own the whole stack.

## FAQ

**Do I need a GSLT token to run an Unturned server?**
Yes, if you want it listed publicly. Generate one for App ID 304930 from a verified Steam account and add it to your server config; without it the server only works via direct IP connect.

**Which ports does an Unturned server use?**
UDP 27015 for game traffic and 27016 for server list queries by default. Each additional instance needs its own pair — the second instance conventionally starts at 27017. When renting, confirm the provider doesn't firewall arbitrary UDP ranges.

**Is 16GB RAM enough for Unturned?**
For the game itself, easily — Unturned is not a demanding title, and even heavily modded servers fit comfortably in a few gigabytes. The 16GB promo configurations leave room for RocketMod plugin overhead, multiple instances, and whatever else you want to run on the same machine. No provider we checked publishes exact per-player memory figures, so treat any precise "X players per GB" claim skeptically.

**Windows or Linux for the server?**
Both work; U3DS ships with helper scripts for each. Linux headless is the standard choice on rented dedicated servers since you'll be SSH-ing in anyway, and it leaves more RAM for the game.

## Before you order

A short checklist by situation:

- Private vanilla server, few friends → a $2.50–4.00 panel plan, skip the dedicated box entirely.
- One public server, 16GB headroom, want root → the $99 E3-1270v5 promo is the entry point most people should start at.
- Heavily modded RP server or multiple instances → the Dual E5-2637v2 at $183.20 gives you 16 threads and 32GB; Sharktech itself markets this one to game server operators.
- Streaming, huge communities, or unmetered bandwidth needs → the 10Gbps line from $269 (Amsterdam is the cheapest location by a wide margin).

Two things to confirm before paying: whether your chosen location has the configuration in stock (sold-out locations disappear from checkout), and what Sharktech's refund terms are — they weren't published on the product pages checked, and it's a one-line question to support. Once that's settled, 👉 [lock in Sharktech's current promo pricing on your dedicated server](https://bit.ly/SharKtech) and get the GSLT sorted while the machine provisions — in-stock systems target delivery within 24 hours, so you could be populating your map this week.
