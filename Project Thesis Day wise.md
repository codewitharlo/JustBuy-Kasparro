#Day 01
Date: 09-05-2026

**Planning and Research**

AI can reduce checkout abandonment by detecting behavioral friction before the user leaves

Track Selected- **Track 2**: AI Assisted Checout Recovery
Decided Project Title- **JustBuy**: Real-time behavioral friction detection and checkout recovery system

1. **Why am I building this?**

I love online shopping, there are just so many options and exploration that I cannot exprerience when I decide to by stuff physically, by going to a store. Yet sometimes I find myself stuck right before checkout, reconsidering my decision, may it be because I am having second thoughts about the price, about quality or delivery time etc. As a shopper, This leads to confusion, regrets and disappointments. 

For the seller, this leads to incomplete sales, disappointments and discourage. I know this because I tried Dropshipping once with Shopify when I was in High School. I saw visitors exploring my page, adding stuff to cart, but then changing their minds at the last stage.

In techincal wording, Shoppers as well as Sellers face *Friction* leading to Dismay, Frustration, just before checkout, or during checkout, if not anywhere else in the whole shop.

2. **Frictions faced by Shoppers-**

(a) Shipping Anxiety-
"WIll it get here in time?", "how long before I can flex my new sneakers?"
Signals: Repeatedly checking shipping, Long pause on delivery section, switching shipping methods repeatedly
Where AI can help: By displaying stuff like "Express delivery available by Tuesday." or "Free shipping eligible above ₹999."

(b) Coupon Frustration-
"No Discounts??!!"
Signals: multiple failed coupon attempts, Repeated focus on promo field
Where AI can help: Directly applying or suggesting available and eligible coupon like "SAVE10 applied for ₹200 discount."

(c) Trust Hesitation- 
"What if product is not according to my size?" "WHat if I dont like the product?"
Signals: viewing return policy, hovering near refund info, long inactivity before payment
Where Ai can help: Display "7-day return and replacement available."

(d) Payment Hesitation-
"No COD?" "UPI is down, what is the way around??"
Signals: repeated payment switching, stalled payment page
Where AI can help: Show "UPI payment available with instant confirmation." or "Use Lazypay to pay later"

(e) Decision Fatigue-
"Let me buy this when a different colour is in stock"
Signals: quantity changing repeatedly, remove/re-add cart item, long idle periods
Where AI can help: Ai can help by displaying "This item is currently in stock and eligible for free exchange." etc

3. **Where AI comes to play and how**

AI handles only-
(a) Natural language generation: Converting friction into human-friendly response.
(b) Contextual explanation: "Delivery timing appears to be the concern." or "Express shipping is available."
(c) Personalized concise messaging: Based on cart, friction type, checkout stage

It does not handle- friction detection, scoring, business logic, state management, analytics

4. **Where Logic and Deteministic Features come to play and how**

(a) Event Tracking-
Tracks: time spent, clicks, retries, navigation

(b) Friction Scoring-
Example: if shippingPageViewed > 2:
         shippingAnxiety += 30

(c) Trigger System-
Example: if shippingAnxiety > 70:
         triggerIntervention()

(d) Session State-
Tracks: cart, stage, interventions shown

(e) Recovery Metrics-
Tracks: recovered checkout, abandoned checkout, friction category

5. **Planned Features**

- Real-time checkout behavior tracking
- Friction scoring engine
- AI-assisted recovery prompts
- Shipping hesitation detection
- Coupon frustration detection
- Payment hesitation detection
- Recovery analytics dashboard
- Fallback handling for AI/API failures

6. **Planned Techstack**

(a) Frontend: Next.js, Tailwind CSS

(b) Backend: Node.js, Express

(c) AI: OpenAI API

(d) Deployment: Vercel, Railway/Render