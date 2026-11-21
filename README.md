# Alipay VPS: Can You Pay Without a Credit Card, What Does the Fee Add, and Which Plans Survive China Peak Hours? (Full AkkoCloud Plan Table)

AkkoCloud pairs an Alipay checkout with CN2 GIA routing, a combination most Alipay-friendly hosts don't offer. Its cheapest listed plan is ¥49/month or ¥449/year for 1 vCPU, 512 MB RAM, 10 GB SSD and 500 GB of monthly traffic on a 500 Mbps port; the 1 GB plan at ¥699/year is where most buyers land. Below you'll find every plan it currently lists, what Alipay actually costs you at confirmation, how the China routing compares with hosts that take Alipay but route the long way around, and which terms (refund, renewal) you need to confirm before money leaves your account.

> **Most readers should start with KVM-CN2-B1 mini**: 1 vCPU, 1 GB RAM, 20 GB SSD, 1.2 TB of traffic at 500 Mbps, ¥59/month or ¥699/year. It's the smallest plan with enough memory for a control panel plus a WordPress site or a proxy, and the annual price works out to about ¥58 a month.
> 👉 [See AkkoCloud's current plans and pay with Alipay](https://bit.ly/akkocloud)

## AkkoCloud's full plan line, in yuan

AkkoCloud runs a Chinese-language storefront with no English pricing page, so the figures below come from the named SKUs on its order pages as recorded in current plan listings. Everything is priced in CNY (¥), billed monthly or annually. Stock and pricing differ by data centre, so the order form is the number that counts.

| Plan | vCPU / RAM / SSD | Traffic & port | Price (CNY) | Order |
| --- | --- | --- | --- | --- |
| KVM-CN2-A2 mini | 1 / 512 MB / 10 GB | 500 GB · 500 Mbps | ¥49/mo · ¥449/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-B1 mini | 1 / 1 GB / 20 GB | 1.2 TB · 500 Mbps | ¥59/mo · ¥699/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-B1 standard | 1 / 1.5 GB / 20 GB | 1.5 TB · 1 Gbps | ¥75/mo · ¥899/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-B2 | 1 / 2 GB / 30 GB | 3 TB · 1 Gbps | ¥99/mo · ¥1,099/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-C1 | 1 / 2 GB / 30 GB | 4 TB · 1 Gbps | ¥129/mo · ¥1,299/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-D1 | 2 / 4 GB / 40 GB | 6 TB · 1 Gbps | ¥199/mo · ¥1,999/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-E1 | 4 / 8 GB / 60 GB | 9 TB · 1 Gbps | ¥299/mo · ¥2,999/yr | [Order](https://bit.ly/akkocloud) |
| KVM-CN2-U2 (unmetered) | 4 / 8 GB / 50 GB | Unmetered · 50 Mbps | ¥59/mo · ≈¥590/yr | [Order](https://bit.ly/akkocloud) |

Two notes on reading that table. B2 and C1 share the same CPU, memory and disk, so the ¥30/month difference buys traffic (3 TB to 4 TB), not speed. The unmetered U2 is the odd one out: 4 cores and 8 GB for less than the 2 GB C1, because the port drops to 50 Mbps. It suits seeding, backups and low-concurrency services; it will not suit a site with concurrent visitors.

Other configurations (768 MB with 15 GB, 1.5 GB with 20 GB on different traffic allowances) appear in older listings at different prices. Treat the eight named plans above as the current retail line and check the order page for what's in stock in your preferred city.

**Locations and platform**, from the same listings: San Jose (USA), Frankfurt (Germany) and London (UK), KVM virtualisation, full root access, 500 Mbps to 1 Gbps ports depending on plan, and CN2 GIA routing on the China-bound path. IPv6 availability, backup policy and the exact OS template list aren't published in the material I could check, so confirm those on the order form if they matter to you.

## What Alipay adds to the final bill

The amount that leaves your account isn't always the amount on the plan page, and the gap varies by host.

Infrawire states plainly that Alipay is the only payment method it surcharges, at **3% of the invoice, added to the bill and visible before you confirm**, while card, PayPal, crypto and bank transfer stay fee-free. Cloudzy takes the opposite line: no surcharge, same price as card, but "whatever Alipay itself charges (network fees, FX spread, processor fees) is between you and Alipay," and it invoices in USD so the conversion happens on the payment side. LightNode says only that the amount is set by the exchange rate and is "all transparent." rdp.monster prices in USD and points to the Alipay payment page as the place where the exact figure appears.

So there's no industry-standard Alipay fee to budget for. Two of those four add nothing on their side, one adds 3%, and all four push the currency conversion to Alipay. AkkoCloud quotes in yuan, which removes one conversion step for a mainland buyer, but the surcharge question isn't published and has to be settled on the confirmation screen. The number shown there, before you tap confirm, is the only number worth comparing.

👉 [Open the AkkoCloud order form and check the yuan total before confirming](https://bit.ly/akkocloud)

## No international card needed, but the payment knows your name

Paying by Alipay removes the card requirement entirely: the transaction is confirmed in the app from your balance or whatever funding source is linked to the account, and no Visa or Mastercard is involved. That's the whole reason this category exists.

The part buyers tend to discover afterwards is identity. rdp.monster spells it out: "Alipay accounts are verified under their owner's real name: rdp.monster never asks for ID, but the payment itself is linked to your Alipay account." The host may never see your documents, yet the payment record ties the purchase to a verified identity. If a server tied to your legal name is a problem, some hosts accept USDT or Monero for exactly that reason. Cloudzy takes the middle route, storing no card data and collecting only a billing email.

For most people this is a non-issue. For anyone buying a server they'd rather not have associated with their real name, it's the deciding factor, and it's worth deciding before checkout rather than after.

## Alipay accepted doesn't mean the route is fast

This is where a lot of Alipay VPS roundups quietly mislead. Payment method and network path are unrelated, and some hosts say so themselves. rdp.monster answers the China question with "No, and we prefer to say it upfront. Our datacenters are in Europe and the USA, without China-optimized routes such as CN2 GIA," then tells readers whose users are in mainland China to buy a China-optimized line instead. That's a host being straight about a limitation most competitors leave out.

CN2 GIA is China Telecom's premium backbone, with dedicated bandwidth and prioritised routing. In practice it means lower latency and stable evening speeds, which is exactly when budget routes degrade. AkkoCloud's entire product line is built on it, including the Frankfurt and London nodes, which is unusual: most China-optimised providers only bother with the US west coast and Hong Kong.

How the alternatives stack up on location: LightNode lists 40+ data centres including Hong Kong, Singapore, Japan, Korea and Taiwan; Cloudzy has 13 regions including ap-sgp-1; Infrawire's Asian point is Hong Kong (Equinix HK1) and it publishes a looking glass so you can measure latency before ordering. None of those three advertises CN2 GIA on its Alipay page.

If your visitors are in mainland China, pick the city first and the plan second. San Jose with CN2 GIA is the usual choice for a China-facing site; Frankfurt and London make sense when your traffic is European and you want the China route as a bonus. Test latency from your own connection before you commit to a city, and don't assume an Asian data centre automatically beats a US one with better routing.

👉 [Pick a city and plan on AkkoCloud's order page](https://bit.ly/akkocloud)

## Refunds, billing granularity and what renewal costs

Refund terms vary enough between hosts that "money-back guarantee" tells you nothing on its own. Cloudzy offers 14 days, no questions asked, refunded to the original payment method, which for an Alipay buyer means the money returns through Alipay. Infrawire offers 7 days. LightNode and rdp.monster don't publish a refund window on their Alipay pages; LightNode leans on hourly billing instead, so a wrong purchase can be destroyed and rebuilt within the hour.

Billing granularity matters as much. LightNode and Cloudzy both bill hourly, which turns a mis-sized plan into a small loss rather than a month's worth. Infrawire bills monthly with no commitment and issues the renewal invoice before expiry, and Cloudzy lets you pay the first invoice with Alipay and switch to a card later, or the reverse.

AkkoCloud's refund policy isn't published in anything I could verify, and its plans are sold monthly or annually with no hourly option in the listing. Ask support about cancellation and refunds before you buy an annual plan; ¥699 is a small amount to lose, but a year is a long time to be stuck with the wrong city. On renewal, third-party write-ups of AkkoCloud report that renewal is billed at the same rate as the first term, with no jump after year one. That's a claim worth confirming on the renewal terms, because it's the opposite of how most of this industry works.

## How the Alipay-friendly hosts compare

Pure information, no links: every provider below accepts Alipay, and the differences that matter are currency, routing and refund terms.

| Provider | Entry price | Billing | China-optimised routing | Refund |
| --- | --- | --- | --- | --- |
| AkkoCloud | ¥49/mo or ¥449/yr (1 vCPU, 512 MB, 10 GB) | CNY, monthly or annual | CN2 GIA, San Jose / Frankfurt / London | Not published; ask support |
| LightNode | $7.71/mo (1 vCPU, 2 GB, 50 GB NVMe, 1 TB) | USD, hourly | Not stated; 40+ locations incl. HK, SG, JP | Not stated |
| Cloudzy | $2.48/mo at 50% off (512 MB, 20 GB NVMe, 1 TB) | USD, hourly/monthly/yearly | Not stated; 13 regions incl. ap-sgp-1 | 14 days, original method |
| Infrawire | €8.30/mo (2 cores, 4 GB, 40 GB NVMe) | EUR, monthly | Not stated; Hong Kong Equinix HK1 | 7 days |
| rdp.monster | $8.99/mo (2 cores, 6 GB, 40 GB NVMe) | USD | Explicitly none (no CN2 GIA) | Not stated |

Cloudzy's 50% discount has no stated end date and no stated renewal price, so don't budget on $2.48 continuing. Infrawire's euro pricing moves with the exchange rate against the yuan. Neither point is a criticism; they're the reasons a straight price comparison across currencies is misleading.

## FAQ

**Do I need an international credit card to buy a VPS with Alipay?**
No. You confirm the payment in the Alipay app from your balance or a linked funding source, and the server is provisioned automatically once the payment clears.

**Who charges the Alipay fee, the host or Alipay?**
Both can. Infrawire adds a disclosed 3% on its own invoice; Cloudzy adds nothing but leaves Alipay's network and FX charges to the payment side. Check the confirmation screen.

**How fast is setup after paying?**
rdp.monster quotes about 10 seconds after confirmation, Cloudzy 60 seconds with the full click-to-SSH flow under 5 minutes, LightNode under 2 minutes, Infrawire about 5 minutes. AkkoCloud doesn't publish a figure; Alipay settlement is normally instant, and credentials arrive by email and in the client area.

**Can I change payment method on renewal?**
Cloudzy and Infrawire both allow it invoice by invoice. AkkoCloud's panel behaviour isn't documented publicly, so ask before you rely on it.

**What if Alipay isn't available in my country?**
Eligibility is set by Alipay, not the host. If you can't complete the payment, hosts that also take cards, PayPal or crypto are the fallback; AkkoCloud's yuan-only storefront is the least flexible option there.

## Which plan to pick

Match the plan to the job, not to the price list. A personal blog or a small Node app runs fine on **A2 mini** at ¥449/year; 512 MB is tight but workable with a swap file. Anything running a control panel, a database and a WordPress install wants **B1 mini** at ¥699/year, which is the value sweet spot in this line. Two or three sites with real traffic, or a proxy serving several people, justify **D1** at ¥1,999/year. **E1** is for workloads that would otherwise be split across servers. **U2** only makes sense if you're moving terabytes and can live with 50 Mbps.

Before paying, check two things: the yuan amount on the Alipay confirmation screen, which is the figure that actually leaves your account once any surcharge and conversion are applied; and the city your plan ships from, tested against your own latency rather than assumed.

👉 [Start with the B1 mini plan on AkkoCloud and confirm the Alipay total](https://bit.ly/akkocloud)
