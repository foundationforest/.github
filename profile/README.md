# Forest

In a small town, everyone knows each other. You know who to call when something breaks and whether they do good work, so everyone is held accountable by their reputation. That doesn't work among millions of strangers, who need another way to find and trust each other. Platforms like Uber, Airbnb and Amazon do that job for us, at scale. It's why you can get into a stranger's car or rent their home without thinking about it.

The catch is that we depend on these platforms. Your profile, with all its reviews, lives inside their app and only counts there. Leave, and you start from zero. So nobody leaves, and they use it to their advantage: bigger cuts every year, more ads in your search results, rules that can change or shut you out overnight.

It doesn't have to be this way. Modern technology lets strangers find and trust each other the way neighbours do in a small town, without depending on anyone in the middle, and with a much better experience. We built Forest's first version to prove it's possible.

## How it works

The core idea: if you own your profiles, you can switch, and if you can switch, there is no dependency. Everything a platform does, from checking who's real to settling disputes, unbundles into services that compete to serve you, not to capture you. Let's start from the bottom:

**Profiles.** Platforms make sure there's a real, unique person behind every profile, so you can't simply start over. Here, you hold one secret, your seed, in the password manager you choose, and from it you create one profile per role you play (seller, renter, patient), and nothing public links them unless you do. To make yourself accountable, verifiers check that you're a real, unique person and sign off on your seed, without ever seeing it. Every profile made from it becomes accountable too.

**Posting.** A platform keeps your listings and reviews inside its app. Now each market (rides, rentals, freelance work, anything) has an open standard for what a listing (an offer or a request) and a review look like. Your profiles post them publicly, on a host: a service anyone can run that keeps them online for anyone to read. Each is signed by whoever wrote it, so nobody can fake one, and the reviews you receive stick to you and belong to whoever wrote them.

**Finding.** A platform decides who you see, with its own private algorithm. Now everything is public, so anyone can look without an account, and anyone can build an index: read every listing and review in a market, check who verified each profile, and rank them with their own algorithm. An index can rank the way a small town judges, where praise counts for more from someone with a good name of their own. You choose the index you trust, so indexes compete on how good their rankings are.

**Using it.** Today each platform has its own app. But the way we use software is moving to plain English, with AI apps that can even draw the screen you need on the spot. Connect your profiles to the AI app you already use, and it can find, post, review and message for you, only within what you allow, and you can take that back any time. One app, with all your context, in plain English.

Every piece follows an open standard, so anyone can build a verifier, a host, an index or an app, and you can switch between them any time.

## What this changes

**Fair competition.** Rankings are built by indexes from public ratings and reviews. So the way up is a better reputation, earned through quality and price, not a bigger ad budget.

**Any market can exist.** A new market is just an open standard away. Anyone can propose one, for anything, and nobody has to build a new platform for it. Joining one is a single step, with no new app or sign-up: you're verified once, so every new profile starts verified.

**One open network.** Everyone in a market meets in the same open network instead of being split across rival apps. You get the reach of a monopoly, without anyone in the middle.

**Agency.** Many companies exist mainly to put several markets together for you: a delivery app joins restaurants and couriers, a travel site joins flights, hotels and cars. Big deals already work without one: buying a house brings an inspector, a lender, an insurer and an escrow agent together, none of them the same company. Small deals got bundled mostly because arranging all that by hand cost more than the deal. When every listing and review is open and your AI can act for you, it can put them together itself, and still hire an expert, like a planner or an architect, when you want one.

## Where we are

The Forest Foundation is a non-profit with one goal: a fairer, more open future.

The first version works. You can get verified, make profiles, post listings, message and connect your AI today. We started with simple markets: deals between two people, like tutoring, home cleaning or selling a used phone, where a listing, a message and a review are enough, and you pay each other however you already do.

It's early, everything is open source, and nothing is perfect yet. We need people to help polish the standards, improve the first markets and create new ones, and we hope others will run services that compete with ours.

What we need most is people using it: an open network gets better with every person on it. [Starting](https://app.forest.foundation) is free and takes two minutes, and [looking around](https://index.forest.foundation) takes nothing.

- **[Standard](https://github.com/foundationforest/standard):** the shared formats everything is built on: keys made from your seed, proofs that a profile is verified, folders where a profile's listings and reviews live, and escrows that hold a deal's money.
- **[Markets](https://github.com/foundationforest/markets):** what a listing and a review hold in each market. Anyone can propose a new one.
- **[Services](https://github.com/foundationforest/services):** the first verifier, host, index and AI connector, which we run.
- **[App](https://github.com/foundationforest/app):** your control panel: create your profiles, get verified, post, message and connect your AI.

Some of our services will charge a little, like verifying with your ID, to sustain the foundation. Everything we earn goes back into the project, and our finances will be public, on chain.

## What's next

- **Payments.** Your profiles already have their own addresses for digital dollars. Next, a deal's money can be held by the terms both sides agreed to, you'll have simple ways to move dollars in and out, and your AI will be able to pay for you, within limits you set. Real money moves only after the code has had an outside review.
- **Markets with more parts.** With payments in place, deals that need more than two people can follow, like a rental with a deposit and someone to settle disputes, each part a service anyone can offer.
- **Your reputation, everywhere.** A good record in one market will help your new profile in another, without linking the two.
- **Screens in your chat.** Listings and messages you can see and tap right in your AI app, not only as text.
- **A phone app.** With notifications, so new messages and reviews reach you right away.
- **An AI on your own device.** For even more privacy: one that runs on your phone, so not even your AI's company sees what you do.

## FAQ

**Why now? Haven't people tried this before?** Yes, and open marketplaces never caught on, mostly for two reasons. There was no accountability: anyone could make a hundred profiles, so reviews meant little. And they were hard to use, often asking you to run your own software or buy crypto just to take part. Both changed only recently: verifiers make every profile accountable without saying who you are, and you can use it all through the AI app you already have.

**What if nobody's on it yet?** It's useful from day one. Your listings show on [our index](https://index.forest.foundation) right away, for free: anyone can find you there on the web, or through an AI connected to Forest, and contact you. And you can bring the clients you already have: share your profile with them, they join for free and review you, and the reputation you build is yours to keep, wherever you find your next client.

**What stops friends from faking reviews for each other?** Each of them is one real person, verified once, so nobody can invent a crowd of fake reviewers. And an index can weigh each review by the reviewer's own reputation, so a group of friends can lift each other only so far. Once payments arrive, a review can also point to a real, paid deal.

**If anyone can run a verifier, can't one person get verified twice?** By two different verifiers, yes. So each index decides which verifiers it counts and how much, and a profile verified by several counts as more surely one person. Verifiers compete on how hard they are to fool, and some could even check something only one person has, like the chip in a passport, and agree on who's who without sharing anyone's data.

**How can a verifier check me without knowing my profiles?** It never sees your seed. Your device shows it a number made from your seed, and it signs that. Each profile then proves, with a [zero-knowledge proof](https://github.com/foundationforest/standard/blob/main/proofs/README.md), that it comes from a verified seed, without showing which one. So nothing public traces your profiles to each other or to you, and no profile ever shows your name. You decide what to link.

**What if I lose my phone?** Your seed lives in a passkey, kept by your password manager (Apple's, Google's or another) the same way it keeps your passwords. Sign in on a new device and everything comes back. You can also add a second passkey, in another password manager or on a security key, so losing one loses nothing. And the app can show your seed as 24 words: write them down, and they open your profiles in any app. Lose every passkey and your words, and nobody can recover them for you: that's the price of no one holding your seed but you.
