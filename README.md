# Common Ground: Group Trips That Fit Every Budget

Scapia Product Internship Assignment

**Live prototype:** [ADD YOUR HOSTED LINK HERE]. To run it locally, open `index.html` in any browser. It needs no build step and has no dependencies.

---

## The problem and insight

**Who:** the friend with the tightest budget in a group of 5–6 planning a 3-day Goa trip. Usually a fresher on a first salary, or a friend still in college, while the others earn more.

**What happens today:** someone posts a WhatsApp poll: a ₹4,200/night private-pool villa or a ₹1,500/night homestay. The villa wins 4–1. The friend who can't afford it doesn't say so. Two days later they write "guys I might have a family thing that weekend" and drop out.

**Why it's broken:** a public poll asks people to reveal their money situation in front of the group, so nobody votes honestly about money. The loudest or richest voice sets the budget. The group loses a friend and never learns why. For a travel company, that's one seat less on every plan like this.

**Insight:** a group trip's budget should be set by its lowest *private* limit, not its loudest public vote. People will share a number in private that they will never say in the group.

## Evidence

**[TO FILL before submitting. Replace every bracket with real answers. Do not submit invented numbers or quotes.]**

**Method:** I sent an anonymous Google Form to [N] friends across [N] friend groups on [date]. It asked their real maximum for a 3-day Goa trip, and whether they had ever skipped a trip partly because of cost. I then compared the answers with what each group had actually voted for.

| What I found | Result |
| --- | --- |
| Private ceiling below the option the group picked | [X of N] people |
| Skipped a trip or made an excuse partly because of cost | [X of N] people |
| Said this in the group chat at the time | [X of N] people |

**Quotes (from follow-up DMs):**

- "[exact quote]" — [first name or initial, age, city]
- "[exact quote]" — [first name or initial, age, city]

**The key gap:** in the public poll, [X] people voted for the ₹[amount] option. Privately, [Y] of them said their limit was lower.

## Why existing tools miss it

- **WhatsApp polls are public.** Every vote shows a name next to it, so the poll measures social pressure, not budget.
- **Anonymous polls still fail the tight-budget friend.** The majority still picks the ₹4,200 villa, and they still drop out. A vote combines preferences. A private ceiling works like a veto. Nothing today lets one person rule out an option without being seen to do it.
- **DMing the organiser is awkward and doesn't scale.** It puts one friend in charge of everyone's money secrets, and the organiser still has to argue for the cheaper option in public.
- **Splitwise and shared itineraries start after the decision.** They split a cost the group already committed to. By then the friend has already dropped out.

## The idea

**Common Ground** is a group trip planner where each friend's budget is a private limit, not a public vote.

1. **The organiser starts a plan** and shares it in the existing WhatsApp group.
2. **Each friend privately sets a total trip ceiling,** flights from their own city included. As they drag the slider, they see how many trip options fit their number, so they know what it means before locking it.
3. **The group sees only who has set a budget,** never the amount.
4. **The core moment:** the group only sees stays and dates that fit *every* ceiling, then votes among those. Options that don't fit are hidden, and the app never says which ones or whose limit ruled them out. In the prototype, the ₹4,200 villa disappears, and dragging another friend's budget shows it isn't always the same person blocking it.
5. **Everyone books their own share** (flight and stay) in one flow.

Two design choices protect privacy. Ceilings are set *before* any options are shown, so nobody can work out who removed what. The ceiling covers the whole trip, because friends flying from different cities pay different amounts for the same stay.

## Who pays and why

| Who pays | How much | Why they'd pay |
| --- | --- | --- |
| Scapia (booking commission) | [X]% commission on flights and stays, booked in one flow | One saved dropout in a group of 6 is 17% more seats sold on that plan. Every booking also runs through the Scapia card. |
| Stays and resorts (sponsored listings) | ₹[X] per group shown, or a fee per booking | A sponsored stay appears only if it fits *every* person's ceiling. The advertiser reaches a group that can afford it and is about to book, without ever seeing anyone's budget. |
| Travel partners (ads during and after booking) | ₹[X] per thousand views | Group insurance while the group decides. Scooter rentals and activities after booking, matched to where the group is staying. |

**Evidence they'd pay:** [TO FILL. e.g. "[X of N] people who skipped a trip said they would have gone if the plan had fit their budget." If a homestay or resort owner told you what they pay for listings today, quote them here.]

## What I'd test next

**Riskiest assumption:** people will enter their *honest* ceiling. Someone might enter a lower number to make the trip cheaper, or a higher one to seem generous. If that happens, the "fits everyone" list is as unreliable as the public poll.

**Test (one week, no code):** run 3 real friend groups planning an actual trip through a Google Form, with me as the matcher.

1. Each friend privately submits a ceiling. I share back only the options that fit everyone.
2. After the trip is booked, I ask each person privately whether their number was their true limit, lower or higher.
3. **Pass:** at least 80% say it was honest, and no one who submitted a ceiling drops out.
4. **Fail:** lowballing is common. Then I'd test a fix, such as showing each person how many options their number removes before they lock it.

---

## About the prototype

A single-file, clickable prototype (`index.html`, plain HTML, CSS and JavaScript). It has 5 screens:

1. **The public poll:** the WhatsApp poll where the expensive villa wins.
2. **Your private budget:** a slider whose fitting-options count and cheapest-trip breakdown update live.
3. **The group sets theirs:** friends finish in real time, with no amounts shown.
4. **Trips that fit everyone:** switch dates, vote, and watch friends' votes arrive.
5. **Everyone books:** each friend pays their own share.

The side panel lets you change each friend's private budget and see the group's options update instantly. This is a demo control; in the real product nobody sees these numbers.

Ad placements shown: a budget-qualified sponsored stay (screen 4), group insurance (screen 3) and a location-matched scooter rental offer (screen 5).

All prices, names and trip options are illustrative sample data.

### Hosting

- **Netlify Drop:** drag this folder onto app.netlify.com/drop.
- **GitHub Pages:** push this repo, then go to Settings → Pages → Deploy from branch `main` / root.
