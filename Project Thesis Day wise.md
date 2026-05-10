# Day 01

**Date:** 09-05-2026

## *Planning and Research*

*AI can reduce checkout abandonment by detecting behavioral friction before the user leaves.*

<br>

### **Track Selected**
**Track 2:** AI Assisted Checkout Recovery

### **Decided Project Title**
**JustBuy** — *Real-time behavioral friction detection and checkout recovery system*

<br>

# **1. Why am I building this?**

I love online shopping. There are just so many options and exploration that I cannot experience when I decide to buy stuff physically by going to a store. Yet sometimes I find myself stuck right before checkout, reconsidering my decision, whether it is because I am having second thoughts about the price, quality, or delivery time, etc.

As a shopper, this leads to confusion, regrets, and disappointments.

For the seller, this leads to incomplete sales, disappointments, and discouragement. I know this because I tried Dropshipping once with Shopify when I was in High School. I saw visitors exploring my page, adding stuff to cart, but then changing their minds at the last stage.

In technical wording, shoppers as well as sellers face *friction* leading to dismay and frustration just before checkout, or during checkout, if not anywhere else in the whole shop.

<br>

# **2. Frictions faced by Shoppers**

### **(a) Shipping Anxiety**

*“Will it get here in time?”*  
*“How long before I can flex my new sneakers?”*

#### **Signals**
- Repeatedly checking shipping
- Long pause on delivery section
- Switching shipping methods repeatedly

#### **Where AI can help**
By displaying suggestions like:

- *“Express delivery available by Tuesday.”*
- *“Free shipping eligible above ₹999.”*

<br>

### **(b) Coupon Frustration**

*“No Discounts??!!”*

#### **Signals**
- Multiple failed coupon attempts
- Repeated focus on promo field

#### **Where AI can help**
Directly applying or suggesting available and eligible coupons like:

- *“SAVE10 applied for ₹200 discount.”*

<br>

### **(c) Trust Hesitation**

*“What if the product is not according to my size?”*  
*“What if I don’t like the product?”*

#### **Signals**
- Viewing return policy
- Hovering near refund information
- Long inactivity before payment

#### **Where AI can help**
Display:

- *“7-day return and replacement available.”*

<br>

### **(d) Payment Hesitation**

*“No COD?”*  
*“UPI is down, what is the way around??”*

#### **Signals**
- Repeated payment switching
- Stalled payment page

#### **Where AI can help**
Show:

- *“UPI payment available with instant confirmation.”*
- *“Use Lazypay to pay later.”*

<br>

### **(e) Decision Fatigue**

*“Let me buy this when a different colour is in stock.”*

#### **Signals**
- Quantity changing repeatedly
- Remove/re-add cart item
- Long idle periods

#### **Where AI can help**
AI can help by displaying:

- *“This item is currently in stock and eligible for free exchange.”*

etc.

<br>

# **3. Where AI comes to play and how**

### **AI handles only**

#### **(a) Natural language generation**
Converting friction into human-friendly responses.

#### **(b) Contextual explanation**
- *“Delivery timing appears to be the concern.”*
- *“Express shipping is available.”*

#### **(c) Personalized concise messaging**
Based on cart, friction type, and checkout stage.

<br>

### **It does not handle**
- Friction detection
- Scoring
- Business logic
- State management
- Analytics

<br>

# **4. Where Logic and Deterministic Features come to play and how**

### **(a) Event Tracking**

#### **Tracks**
- Time spent
- Clicks
- Retries
- Navigation

<br>

### **(b) Friction Scoring**

#### **Example**
```txt
if shippingPageViewed > 2:
    shippingAnxiety += 30
```

<br>

### **(c) Trigger System**

#### **Example**
```txt
if shippingAnxiety > 70:
    triggerIntervention()
```

<br>

### **(d) Session State**

#### **Tracks**
- Cart
- Stage
- Interventions shown

<br>

### **(e) Recovery Metrics**

#### **Tracks**
- Recovered checkout
- Abandoned checkout
- Friction category

<br>

# **5. Planned Features**

- Real-time checkout behavior tracking
- Friction scoring engine
- AI-assisted recovery prompts
- Shipping hesitation detection
- Coupon frustration detection
- Payment hesitation detection
- Recovery analytics dashboard
- Fallback handling for AI/API failures

<br>

# **6. Planned Tech Stack**

### **(a) Frontend**
- Next.js
- Tailwind CSS

### **(b) Backend**
- Node.js
- Express

### **(c) AI**
- OpenAI API

### **(d) Deployment**
- Vercel
- Railway/Render
