---
title: "🧭 Mortgage Side Quest: The Switching Point | homestep.ie"
layout: post
tags:
   - mortgage
   - AIP
   - help to buy
   - first home scheme
---

It's been more than 9 months since I've been in the market to buy a house in Dublin, Ireland. In this time, I've done a lot of research about property prices - both new and second-hand homes and government schemes (Help to Buy, First Home Scheme, etc.) that help with the purchase.

I needed to understand how much I could afford with or without the help of government schemes, essentially, my buying power. More importantly, I needed to understand how it changed over time as I save for the deposit and I try to put myself in a better position career-wise.

<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-charlie.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

To no one's surprise, your buying power at any point depends on the 3 factors:
1. How much you make - Gross income
2. How much you've saved
3. How much you can/wish to avail from the government schemes

### How much you make - Gross income
This is important because it's directly proportional to how much Approval in Principle (AIP) you can get. Maximum AIP/mortgage that a lender can lend is capped at 4 times your gross income and up to 90% Loan-to-Value ratio (LTV). This is *the biggest* contributor towards your buying power.

_There are other factors such as age and health, but it's something you don't have control over. I'll stick to the factors that you do have control over._

### How much you've saved
This is important because it's the amount you will use as your deposit. And in some cases, it might help you bridge the gap between the cost of the house and the sum of deposit and AIP.

### How much you can/wish to avail from the government schemes
This is important because it has the potential to drastically help you if you're a first time buyer, AND you're looking at newly built homes AND you're looking for properties under €500K. From the list of conditions I just mentioned, you might think people who opt for this would be a small portion of the population. But, that is not the case. On the contrary, it's very popular.

---
<br>

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">🎯 The Goal</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-goal.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

It's not an easy one, but my goal was to be able to buy a house that <span class="highlight">costs a certain amount</span> within a <span class="highlight">certain period of time</span>. *It still is*. I needed a plan based on all the three factors mentioned above. I needed a tool that could show me how my buying power changes over time with accurate breakup of the cost. Since I couldn't find one that helped me visualize this data over a long timeline - I built <a href="https://homestep.ie/" target="_blank" rel="noopener noreferrer">HomeStep.ie ↗</a> to do exactly that. It helped me finally get a solid plan together. If you're in the same boat, feel free to use it to map out your own future too.

I'll share the key things I learned while creating the tool and the insights I got once I started using it.

---
<br> 

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">⚖️ The Calculations</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-calculations.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

How do you know how much you can afford at any point of time? It's **always** the lesser of two amounts:
1. <span class="highlight">Amount A</span> - 10 times the deposit amount (that you've saved up till then)
2. <span class="highlight">Amount B</span> - Sum of deposit amount and AIP (or 4 times your gross income if you haven't got your AIP yet)

<span class="highlight">Amount A</span> is based on these facts:
1. The borrower has to contribute 10% of the cost of house as the deposit.
2. Lenders are allowed to give a maximum mortgage of 90% LTV.
3. There's the bit about cap of 4 times the gross income that I've already mentioned.

<span class="highlight">Amount B</span> is based on common sense. You cannot buy a house that costs more than the sum of your savings and the AIP amount.

So, why the lesser of the two amounts - Amount A and Amount B? Let me show this with an example. Consider the following example:

| Starting from      | March 2026 |
|--------------------|------------|
| Opening balance(€) | 10,000     |
| Monthly savings(€) | 1,000      |
| Gross income(€)    | 60,000     |

| Month     | Savings(€) | Max AIP(€) | Amount A(€)                            | Amount B(€) | Buying power(€)                        |
|-----------|------------|------------|----------------------------------------|-------------|----------------------------------------|
| June 2027 | 26,000     | 240,000    | <span class="highlight">260,000</span> | 266,000     | <span class="highlight">260,000</span> |

 By June 2027, it may look like your savings (which can be used as deposit) + Max AIP can get you a house that costs €266,000 (Amount B). But by this time, you do not have the 10% deposit - 10% of €266,000 - €26,600. You're short by €600. But you do have enough to get a house that costs <span class="highlight">€260,000 (Amount A)</span>.  Here's how.

<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/June-27.png" 
       alt="HomeStep screenshot" 
       style="width: 600px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

So, that's why it's always the lesser of the two.

---
<br>

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">🔀 The Switching Point</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-switching-point.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

Something interesting happens in July 2027. Let's take a look...

| Month     | Savings(€) | Max AIP(€) | Amount A(€)                            | Amount B(€)                            | Buying power(€)                        |
|-----------|------------|------------|----------------------------------------|----------------------------------------|----------------------------------------|
| June 2027 | 26,000     | 240,000    | <span class="highlight">260,000</span> | 266,000                                | <span class="highlight">260,000</span> |
| July 2027 | 27,000     | 240,000    | 270,000                                | <span class="highlight">267,000</span> | <span class="highlight">267,000</span> |

Amount B becomes lesser than Amount A. This mean the Max AIP (€240,000) is not enough to cover the difference between the cost of the house (Amount A €270,000) and the deposit (€27,000) - which is €243,000. Your AIP is short by €3,000. But you can still afford a house that costs <span class="highlight">€267,000 (Amount B)</span>. Split your savings into two - €26,700 for deposit and the remaining €300 to cover the gap. Here's how.

<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/July-27.png" 
       alt="HomeStep screenshot" 
       style="width: 600px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

So, in a timeline like this, you start off with being able to buy Amount A (10 times the deposit) and after a certain point in time, as your savings grow, the switch happens. And then your buying power becomes the sum of your savings and AIP. When does the switch happen, you ask? Well, there's a formula for that. 

<span class="highlight">
The switching point is when your savings amount becomes greater than 11.11% of your AIP.
</span>

In the above example, the moment your savings become more than 11.11% of €240,000 (€26,666.66), the switch happens. Let's zoom out a little a see what it actually means and why do I think it's soooo important.

---
<br>

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">📈 The Buying Power Trajectory</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-trajectory.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>



<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/trajectory.png" 
       alt="HomeStep screenshot" 
       style="width: 600px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

Let's take a look at the whole 5-year timeline for this example. As you can see, the rate at which your buying power increases is high until June 2027. After that it slows down. To put things in perspective, your buying power increased by €150,000 in 16 months starting from March 2026. Whereas it only increased €15,000 in the next 16 months. That's a huge drop in the rate of increase. And this isn't unique to this set of made-up numbers. You can see this pattern emerging with any combination of savings and AIP. So, what does this mean?

<span class="highlight">
It means your AIP has stopped helping you!!
</span>

Okay, maybe I got a little carried away there. It's still helping you but not much as you'd like. Once you hit the switching point, you've maxed out the help you can get from the AIP. You know how they say that every time you save €1,000, you're buying power goes by €10,000. Well, not forever. Only up till you reach the switching point. 

For instance, it's true if you've saved €20,000 and your AIP is €200,000. You **can** afford a house that costs €210,000. You AIP will help you.

<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/example-1.png" 
       alt="HomeStep screenshot" 
       style="width: 800px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

But if you've saved €80,000 and your AIP is €440,000 (assuming your gross income is €110,000), you **cannot** afford a house that costs €800,000. You can afford no more than €521,000.

<div style="text-align: center; margin: 30px 0;">
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/example-2.png" 
       alt="HomeStep screenshot" 
       style="width: 800px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

Up until the switching point, your savings have a 10x multiplier on your buying power. After the switch, that multiplier drops to 1x. From that point on, you are saving for the purchase price, not just the deposit. The rate of increase of your buying power drops by 90%.

---
<br>

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">🛡️ Changes to LTV</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-honest.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

A positive effect of being on the other side of the switching point is that your LTV ratio goes down. It's because, at this point, you've started to use your savings for paying some balance amount too. 

---
<br>

<div style="text-align: center; margin: 30px 0;">
<h2 id="the-goal">🏁 Conclusion</h2>
  <img src="{{ site.baseurl }}/assets/images/{{ page.slug }}/meme-conclusion.jpg" 
       alt="Meme" 
       style="width: 500px; max-width: 100%; height: auto; border-radius: 4px;">
</div>

I know that is a lot to take in. But it's all important things you need to know to plan for your future. I have a plan for myself and I hope to buy in the near future. <a href="https://homestep.ie/" target="_blank" rel="noopener noreferrer">HomeStep.ie ↗</a> is helping me understand where I was, where I am now, and where I want to be. I hope it helps you in your journey too.

Now I know that I haven't reached my goal yet, so I'm not in a position to give 'expert' advice. But since you're not my boss, I’m going to give you my suggestions anyway!
1. Your buying power is **heavily** dependent on two factors:
   1. How much you make - Gross income - **More important**
   2. How much you've saved
2. Try to keep your switching point as high as possible.
3. Use the <a href="https://homestep.ie/" target="_blank" rel="noopener noreferrer">HomeStep.ie ↗</a> to find out your current situation, come up with a goal, and make a plan (AND stick to it).

<style>
.highlight {
    color: #b5e853;
    font-weight: bold;
}
</style>