# 10 overlooked metrics that matter more than DAU and MAU

Alternative title suggestions: 
- 10 best growth metrics you're not tracking (but should be)

## Introduction

Popular usage metrics such as DAU, MAU, and Stickiness, while valuable, may not be the most important indicators of growth for *your* app. These metrics provide a solid ground for tracking day-to-day usage, particularly in the early stages of development, but they don't tell the whole story. There are other important trends these numbers don't show.

According to [Andrew Chen](https://andrewchen.com/dau-mau-is-an-important-metric-but-heres-where-it-fails/), DAU and MAU are useful metrics only for certain types of consumer apps and can be misleading for the rest. Sometimes they make you think your app isn't doing so well when it actually is. People using your app less often can still be very valuable customers to your business. 

Here are examples of very successful apps, where DAU and MAU are not the essential metrics:
- Travel: Airbnb, Booking, Skyscanner
- Tickets: Ticketmaster, Eventbrite
- Real estate: Zillow, Redfin
- Car buying: CarGurus, Carvana
- Job search: Indeed, Glassdoor
- Taxes: TurboTax
- eLearning: Coursera, edX
- Money: Mint, Personal Capital
- Dating: Tinder, Hinge
- Freelance work: Upwork, Fiverr
- Health care: Teladoc

Notice a pattern here? People don't use these apps every day. But when they do, they use them a lot and are willing to pay. This burst usage, combined with high intent, is exactly why such apps succeed despite not needing daily engagement.

The key is *understanding the unique usage patterns that drive revenue and retention in your app*. To do that, you first need to understand your market and users deeply. Our articles on [defining the ICP](https://posthog.com/newsletter/ideal-customer-profile-framework) and [how to identify and analyze power users](https://posthog.com/tutorials/power-users) can help you with that. 

Once you have a clear picture of your users, the next step is identifying the metrics that matter most. Rather than relying solely on DAU or MAU, focus on metrics that highlight how your most valuable users interact with your app. Here are some key metrics to consider.

### Power User Curve

**What is it?** A graph which represents user engagement levels across your entire user base, typically showing the number of days where users stayed active within a given time period (e.g., 30 days).

**Is it useful?** It helps identify the size of your power user segment, the engagement gap between power users and casual users, and how engagement levels are spread out among your user base. 

**How to calculate?** Sort your users based on their number of active days in the last 30 (or 7) days, from most active to least active. Then, make a graph: 
- X-axis: all your users (from 0% to 100%)
- Y-axis: how many days they used the app

We plan to drop a deep dive into a Power User Curve and how you can create one in PostHog. [Subscribe to our newsletter](https://posthog.com/newsletter) and we'll send it straight to your inbox (we promise to send you only the good stuff!)

### DAPU

**What is it?** Daily Active Power Users: the percentage of all users who use your app every day in a week.

**Is it useful?** This metric helps you understand the size of your most engaged user segment.

**How to calculate?**

$$ \frac{\text{Number of users active every day last week}}{\text{Total number of users}} \times 100 $$

### Power User Activity Index

**What is it?** A breakdown of the most common actions performed by your power users.

**Is it useful?** This helps you understand which features or content are most valuable to your most engaged users.

**How to calculate?** Track and rank the frequency of specific events or actions taken by power users.

### Power User Retention Rate

**What is it?** The percentage of power users who remain power users over time.

**Is it useful?** It helps you understand how well you're maintaining the engagement of your most valuable users.

**How to calculate?**

$$ \frac{\text{Number of power users active in current period}}{\text{Number of power users active in previous period}} \times 100 $$

## Other often overlooked metrics

Power users are not the only users you should measure. You should also care about other segments and help them become power users. Here are some metrics that could help you with that.

### Power User Conversion Rate

**What is it?** The rate at which you're able to turn regular users into power users over time.

**Is it useful?** This metric shows how good your app is at getting people to use your app more.

**How to calculate?** 

$$ \frac{\text{New power users in a given period}}{\text{Total new users in the same period}} \times 100 $$

### Time to first key action

**What is it?** This metric measures how long it takes for a new user to engage with a significant feature of your app. 

**Is it useful?** It is important to understand your user onboarding and can indicate how quickly users get value from your app. 

**How to calculate?** Track the time (in hours or days) between when a user signs up and when they complete a specific action, such as making their first purchase or using a core feature.

### User depth

**What is it?** User depth refers to the extent of engagement a user has with the app, such as the number of features used or actions taken. 

**Is it useful?** This metric is important for assessing long-term engagement and understanding how how many features they use and to what extent.

**How to calculate?** Monitor the number of unique features or actions a user interacts with during a set period, e.g. over the course of a month.

### Feature adoption rate

**What is it?** This metric tracks how quickly users begin using new features after they are released. 

**Is it useful?** Feature adoption rate can guide the development process, set the feature priorities and ensure that the users understand how to use them.

**How to calculate?** 

$$\frac{\text{Number of users who used the new feature}}{\text{Total number of users}} \times 100 $$

### Cost per action (CPA)

**What is it?** CPA is the cost associated with a specific user action, usually, the one that makes money or has a high impact on your app, such as purchases, trials or onboarding completion.

**Is it useful?** Analysing this metric helps improve onboarding, and marketing and track the return on investment for different acquisition strategies. 

**How to calculate?** 

$$\frac{\text{Total cost of acquisition or marketing}}{\text{Number of completed actions}}$$

### User lifetime before churn

**What is it?** The duration for which a user remains active before they stop using your app (churn).

**Is this useful?** Like LTV, the user's lifetime before churn it's the key for understanding customer retention and engagement but measured in **time**. This metric can help to identify when users are most likely to stop using your app and what factors contribute to their decision.

**How to calculate?** Track the average time (in days or months) from when a user first signs up until their last activity, then calculate the average for all users who have churned during a specific period.


## Summary

There are plenty more metrics you should be considering. Make sure to understand your users and what makes sense to measure in your app. If you want to start measuring user behaviour in your app for free, get started with one of our [free dashboard templates](https://posthog.com/templates).
