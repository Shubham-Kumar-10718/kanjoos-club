# Kanjoos Club: Group Trips That Fit Every Budget

**Shubham Kumar** · Scapia Product Internship Assignment

**Prototype:** https://shubham-kumar-10718.github.io/common-ground/

## The problem and insight

**Who:** the friend with the tightest budget in a group of 5–6 planning a 3-day Goa trip. Usually a fresher on a first salary, or a friend still in college, while the others earn more.

**What happens today:** someone posts a WhatsApp poll: a ₹4,200/night private-pool villa or a ₹1,500/night homestay. The villa wins 4–1. The friend who can't afford it doesn't say so. Two days later they write "guys I might have a family thing that weekend" and drop out.

**Why it's broken:** a public poll asks people to reveal their money situation in front of the group, so nobody votes honestly about money. The richest voice sets the budget, and the group loses a friend without knowing why. For a travel company, that is one seat less on every plan like this.

**Insight:** a group trip's budget should be set by its lowest *private* limit, not its loudest public vote. People will share a number in private that they will never say in the group.

## Evidence

**Status: a hypothesis from my own friend groups. Structured interviews have not been run yet,** so this document contains no numbers or quotes I haven't collected.

**What I have seen myself:** in our WhatsApp trip planning, price is decided by a public poll, and anyone who drops out gives a reason that isn't money ("family thing", "work came up"). Nobody asks whether cost was the real reason.

**How I'm validating it:** an anonymous form to 3 friend groups that recently planned a trip, asking (1) "What's the most you could comfortably spend on a 3-day Goa trip, all-in?" and (2) "Have you ever skipped a trip, or made an excuse, partly because of cost?" I compare each private answer with the option that group voted for. The signal: private ceilings below the option the group picked, from people who voted for it in public.

## Why existing tools miss it

- **WhatsApp polls are public.** Every vote has a name next to it, so the poll measures social pressure, not budget.
- **Anonymous polls still fail this friend.** The majority still picks the villa. A vote combines preferences; a private ceiling works like a veto. No tool lets one person rule out an option without being seen to do it.
- **DMing the organiser is awkward.** It makes one friend the keeper of everyone's money secrets, and they still have to argue for the cheaper option in public.
- **Splitwise and shared itineraries start after the decision.** By then, the friend has already dropped out.

## The idea

**Kanjoos Club** ("kanjoos" is Hindi for miser) is a group trip planner where each friend's budget is a private limit, not a public vote.

1. **The organiser starts a plan** and shares it in the existing WhatsApp group.
2. **Each friend privately sets a total trip ceiling,** flights from their own city included. The slider shows how many trips fit their number before they lock it.
3. **The group sees only who has set a budget,** never the amount.
4. **Core moment:** the group sees only stays and dates that fit *every* ceiling, and votes among those. Options that don't fit are hidden, and the app never says which ones or whose limit removed them. In the prototype, the ₹4,200 villa simply isn't there.
5. **Everyone books their own share** of flight and stay in one flow.

Ceilings are set *before* any options are shown, so nobody can work out who removed what. The ceiling covers the whole trip, because friends flying from different cities pay different amounts for the same stay.

## Who pays and why

| Who pays | How much (estimates) | Why |
| --- | --- | --- |
| Scapia (booking commission) | 2–3% on flights, 12–15% on stays | One saved dropout in a group of 6 is 17% more seats sold on that plan, and every booking runs through the Scapia card. |
| Stays and resorts (sponsored listings) | ₹40–60 per group shown, or 5% extra per booking | A sponsored stay appears only if it fits *every* ceiling, so owners reach groups that can afford them and are about to book, without seeing anyone's budget. |
| Travel partners (ads) | ₹200–300 per thousand views | Group insurance while the group decides; scooters and activities near the booked stay after booking. |

**Evidence they'd pay:** these prices are not validated yet. Scapia's case is the strongest: every saved dropout is extra booking revenue at no extra acquisition cost. Next, I'd ask 3–5 Goa homestay owners what they pay online travel agencies per booking today.

## What I'd test next

**Riskiest assumption:** people will enter their *honest* ceiling. Someone might enter a lower number to make the trip cheaper, or a higher one to seem generous. Then "fits everyone" is as unreliable as the public poll.

**Test (one week, no code):** 3 real friend groups plan an actual trip through a Google Form, with me matching ceilings to options by hand. After booking, I ask each person privately whether their number was their true limit. **Pass:** at least 80% say it was honest, and nobody who submitted a ceiling drops out. **Fail:** lowballing is common, so I'd test showing each person how many options their number removes before they lock it.
