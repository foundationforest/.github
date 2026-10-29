# Forest

Every deal between strangers needs two things: finding each other, and trusting each other. Platforms like Uber, Airbnb and Amazon solve both at scale. It's why you can get into a stranger's car or rent their home without thinking about it.

The catch is that we depend on these platforms. Your profile, with all its reviews, lives inside their app and only counts there. Leave, and you start from zero. So nobody leaves, and they use it to their advantage: bigger cuts every year, more ads in your search results, rules that can change or shut you out overnight.

It doesn't have to be this way. Modern technology lets us rethink how finding and trusting work, without dependencies, and with a much better experience. We built Forest's first version to prove it's possible.

## How it works

The core idea: if you own your profiles, you can switch, and if you can switch, there is no dependency. Everything a platform does (verification, hosting, algorithms, UI) unbundles into services that compete to serve you, not to capture you. Let's start from the bottom:

**Profiles.** Platforms make sure there's a real, unique person behind every profile, so you can't simply start over. Here, you hold one secret on your device, and from it you create one profile per role you play (seller, renter, patient), and nobody can link them. To make yourself accountable, verifiers check that you're a real, unique person and sign off on your secret, without ever seeing it. Every profile made from it becomes accountable too.

**Posting.** A platform keeps your posts inside its app. Now each market (rides, rentals, freelance work, anything) has an open standard for what an offer and a review look like, and your profiles post them publicly, on any host you choose. Each is signed by whoever wrote it, so nobody can fake one, and the reviews you receive stick to you and belong to whoever wrote them.

**Finding.** A platform decides who you see, with its own private algorithm. Now everything is public, so anyone can build an index: read every offer and review in a market, check who verified each profile, and rank them with their own algorithm. You choose the index you trust, so indexes compete on how good their rankings are.

**Using it.** Today each platform has its own app. But the way we use software is moving to plain English. Connect your profiles to the AI app you already use, and it can find, post, review and message for you, only within what you allow, and you can take that back any time. It can even build the screen you need on the spot. One app, with all your context, in plain English.

Every piece follows an open standard, so anyone can build a verifier, a host, an index or an app, and you can switch between them any time.

## What this changes

**Fair competition.** Rankings are built by indexes from public ratings and reviews. So the way up is a better reputation, earned through quality and price, not a bigger ad budget.

**Any market can exist.** A new market is just an open standard away. Anyone can propose one, for anything, and it works the day someone posts the first offer.

**One open network.** Everyone in a market meets in the same open network instead of being split across rival apps. You get the reach of a monopoly, without anyone in the middle.

**Agency.** Many companies exist mainly to put several markets together for you: a delivery app joins restaurants and couriers, a travel site joins flights, hotels and cars. When every offer and review is open and your AI can act for you, it can put them together itself, and still hire an expert, like a planner or an architect, when you want one.

## Where we are

The Forest Foundation is a non-profit with one goal: a fairer, more open future.

We wrote the first standards and services so Forest works, all open source for anyone to review. They aren't perfect. We need help polishing the standards and creating new markets, and we hope for competitors to our services.

What we need most right now is people. The first version works, and the network gets better with every person on it. It's free, and you can start in two minutes.

- **[Standard](https://github.com/foundationforest/standard):** the shared formats everything is built on: keys, profiles, folders and proofs.
- **[Markets](https://github.com/foundationforest/markets):** what an offer and a review hold in each market. Anyone can propose a new one.
- **[Services](https://github.com/foundationforest/services):** the first verifier, host, index and AI connector, which we run.
- **[App](https://github.com/foundationforest/app):** your control panel: create your profiles, get verified, connect your AI.

Some of our services will make money to sustain the foundation. Everything we earn goes back into the project, and our finances will be 100% public, on chain.

## FAQ

**How can a verifier vouch for me without knowing my profiles?** It never sees your secret. Your device shows it a number made from your secret, and it signs that. Each profile then proves, with a zero-knowledge proof, that it comes from a verified secret, without showing which one. So your profiles can't be traced to each other or to you, and you never have to show your name. You decide what to link.

**What if I lose my phone?** Your secret lives in a passkey, kept by your password manager (Apple's, Google's or another) the same way it keeps your passwords. Sign in on a new device and everything comes back. If you lose the passkey itself, nobody can recover it for you: that's the price of no one holding it but you.

**What's next?** Payments first. Your profiles already have their own addresses for digital dollars. Next, the app will hold a deal's money until both sides are happy, and your AI will be able to pay for you, within limits you set. Later, an AI that runs on your own device, so not even your AI's company sees what you do.
