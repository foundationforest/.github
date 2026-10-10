# Forest

The economy runs on two things: finding who to deal with, and trusting them. Hiring a tutor, renting a room, selling a bike: same two problems, finding and trusting.

We've had three ways to solve them. Forest is the fourth.

1. **Word of mouth.** Works among people who know each other. Doesn't reach strangers.
2. **Advertising.** Reaches strangers. Rewards whoever spends most.
3. **Platforms.** Reputation at scale, at last, but inside their walls: they hold your profile and your reviews, so leaving means starting over, and they set the terms.
4. **Forest.** A platform, outside the walls. You own your profiles. Your reputation is open for anyone to read. Everything else is a service you can switch.

Using it feels like a platform: a profile, a reputation, people find you, you find them, or your AI does it for you. What's different is who holds it all: you.

## How it works

1. **Own.** It starts with a [seed](https://github.com/foundationforest/standard/tree/main/keys): a long random secret made on your device and kept in its secure storage, so nobody, including us, ever sees it. From it you get one profile for each role you play: tutor, seller, landlord. Each profile is computed from the seed, not picked at random, so one seed can only ever give one profile per role. And there's no account anywhere: nobody gave you a profile, so nobody can take it away.

2. **Accountable.** A seed is only a secret; anyone can make a thousand. What makes yours count is making it unique: once, an [issuer](https://github.com/foundationforest/services/tree/main/issuer) checks that a real, single human is behind it (ours looks at your face) and won't check the same human twice. Every profile from that seed inherits it: it can show a real person stands behind it, without showing who. One person, one profile per role. That's what makes reputation stick.

3. **Publish.** Roles come from [markets](https://github.com/foundationforest/markets): shared standards that say which roles exist and how offers and reviews are written. Under that standard your profile publishes its offers, its reviews and its finished deals to a [host](https://github.com/foundationforest/services/tree/main/host) (any storage service you pick), open for anyone to read. Your profiles share nothing, so nobody can tell two are yours, or who's behind any of them, unless you choose to say.

4. **Be found.** That public data, across every verified profile, is what [indexes](https://github.com/foundationforest/services/tree/main/index) read and rank: by who stands behind a profile, the deals it has paid, the reviews it has earned. That's how people find you, and how you find them. Anyone can run an index with a different algorithm; ours is open, so no single ranking gets to rule.

5. **Act.** The [app](https://github.com/foundationforest/app) on your device makes your seed, gets you checked, and works as your control panel: who may do what on your behalf. From there, connect your AI and work in plain English: offer, agree, pay, review, under rules you set. Both sides have a profile, so reviews go both ways, and everything you write is signed, so nobody can write in your name.

6. **Switch.** What's always yours sits on your device: the seed, the profiles made from it, your money, and a copy of your data, so you can move to any host. Everything around you is a service you can switch: the issuer, the host, the indexes, the app, the AI. That's what makes the competition fair: nobody can lock you in, so a service wins only by being better.

No ads, no cut of your deals. The few things that cost money (the check, a registration, storage) are paid per use, and anyone can run a cheaper copy.

## Questions

**Who knows who I am?** Only the issuer, because it checked you, and even it learns nothing more: it can't tell which profiles are yours. Everyone else, hosts, indexes, us, sees profiles, never people. Who's behind a profile comes out only if you say so.
→ [issuer](https://github.com/foundationforest/services/tree/main/issuer)

**How do I make sure nobody links my profiles?** Inside Forest, nothing can: each profile has its own secret, its own data and its own money, and when one gets registered we pay the fee, so your own address never shows up next to it. Outside Forest, two things can, and both have fixes: your network address (a VPN or a relay) and money moved between your own profiles in the open (a privacy pool mixes it). The app will make both a setting. Linking them is only ever your move, and you can share one fact, like a rating, without sharing the rest.
→ [app](https://github.com/foundationforest/app) · [reputation](https://github.com/foundationforest/standard/tree/main/reputation)

**Can I keep things private?** Yes. What a profile publishes is public by default; anything you'd rather keep private, you encrypt with a key of yours that never leaves the device, so only you, and the people you grant access, can read it. The host keeps it without being able to read it.
→ [records](https://github.com/foundationforest/standard/tree/main/records)

**Who sets the market standards?** Anyone. A market is a proposal in an open list: we're writing the first ones to get started, and anyone can add one or improve one. Which version wins is decided the way it is everywhere, by what people, apps and indexes actually use.
→ [markets](https://github.com/foundationforest/markets)

**What stops fake profiles and fake reviews?** Nothing stops anyone from writing them; what matters is whether they count. Our index lists only profiles a real person stands behind, and weighs a review by what backs it, like a paid deal. Any index can do it its own way; the algorithm is what they'd compete on. We think today's evidence is already enough to rank well, and that more kinds will come as each market takes shape.
→ [index](https://github.com/foundationforest/services/tree/main/index)

**What if I mess up?** It stays on that profile; your others don't carry it. You earn it back the way you would anywhere: with good work, and the evidence keeps piling up.
→ [index](https://github.com/foundationforest/services/tree/main/index)

**Why crypto?** Two things need a public ledger. First, the record of who's verified: it has to be public and impossible to rewrite, us included, and a ledger is the only way we know. Second, money: it has to move between strangers, anywhere, in seconds, and digital dollars (stablecoins: dollars that live on a ledger) do that. Forest has no coin.
→ [registry](https://github.com/foundationforest/standard/tree/main/registry)

**Do I have to touch crypto?** No. The app keeps your money in digital dollars; you'd top it up the way you already pay, by card or bank transfer, and two small services (a registry payer and a fee payer) handle the ledger for you, paid in dollars.
→ [registry payer](https://github.com/foundationforest/services/tree/main/fee-payer/registry) · [fee payer](https://github.com/foundationforest/services/tree/main/fee-payer)

**How do payments work?** In digital dollars, straight to the other side. With a stranger, an escrow holds the money until both of you are done, and nothing in it lets anyone but the two sides, an arbiter you both chose or a timer move it. A finished deal becomes evidence behind the reviews.
→ [escrow](https://github.com/foundationforest/standard/tree/main/escrow)

**Do I have to handle all this myself?** No. Connect an AI to Forest through an MCP, the standard plug that gives an AI its tools (we run one), and tell it what you want in plain English: find someone, make an offer, check a review. It works with access keys you hand it, which can do only what you allow, never with your main key, the one that makes them and can take them back.
→ [mcp](https://github.com/foundationforest/services/tree/main/mcp) · [keys](https://github.com/foundationforest/standard/tree/main/keys)

**Can I be banned?** Not from Forest: nobody gave you your profile, so nobody can take it. A host can refuse to serve it and an index can leave it out; both are services you replace, and the profile and its history go with you.
→ [records](https://github.com/foundationforest/standard/tree/main/records)

**What if I lose my device?** Your seed can be rebuilt from 24 words you keep somewhere safe, like a password manager; with them, a new device gets everything back. Nobody else ever holds them, so nobody can rebuild it, us included. That's not a missing feature: any door back in for you would be a door for someone else.
→ [keys](https://github.com/foundationforest/standard/tree/main/keys)

**Why won't Forest become the next platform?** Because there's nothing to capture. You hold your seed, your profiles and a copy of your data, so everything we run has to keep earning you against any copy anyone runs. The test: can you leave every service we run and keep using your profiles and history? The day the answer is no, we've failed.

## Who's behind it

Forest is built by the Open Forest Foundation, a non-profit now being registered, with one goal: that this future arrives, with or without us. We build only the open pieces that were missing, run the first copy of each, and hope to lose every one to someone better. No investors, no ads, no coin. Some of our services charge; the app and our index are free. What we earn goes back in, and our finances will be public.

## Where it stands

Every piece except the app exists, and a test of the whole loop passes on a test network with test dollars: one person checked, profiles registered, a paid deal through escrow, a review, a rating proven. The checks in that test are stand-ins. No stranger has used it yet. Nothing is ready for real money; before that come the app, then sealing the [registry](https://github.com/foundationforest/standard/tree/main/registry) (the record of who's verified) so nobody can change it, us included, then a security review.

The standard is the only part everyone shares. Everything else can exist in copies: we built the first of each, and anyone can run another.

| Repo | What it is | State |
|---|---|---|
| [standard](https://github.com/foundationforest/standard) | the rules every piece follows, the registry, an escrow, and the libraries that implement them | built; the registry not yet sealed |
| [services](https://github.com/foundationforest/services) | what we run: an issuer, a host, an index, the two payers, the tools AIs use; open code, plus how we run each | running on the test network |
| [app](https://github.com/foundationforest/app) | holds your seed, every service swappable, ours by default; web first, then phones | not built yet |
| [markets](https://github.com/foundationforest/markets) | the open list of markets and their shapes | open to proposals |

One person built this far, with AI. What's here is the bare minimum to start: the standard, and one copy of each service, ours. What it needs now is people: the first markets, the first profiles, the first deals, and better copies of what we run, because competition is the point. If you think the economy should be open and fair: propose a market, build on the standard, run a service.

Code is Apache 2.0. The markets list is public domain.
