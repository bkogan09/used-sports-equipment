**A/B Test Plan**

**Element being changed:** ****I will be changing the home page headline in ***index.html*** ******because it is the first thing that every visitor reads, and this is where most visitors enter the site. Version A makes a general promise with no real number, but a shopper deciding whether to contact the shop wants to know how much they would save. The discount range in B comes from the equipment page on the site.

**Version A (current page): “**Quality used sports equipment, priced for real life"

**Version** **B:** “Save 30 to 75 percent on quality used sports equipment”

**Hypothesis:** If the headline states a specific savings amount instead of a general promise, a larger number of AI visitors acting as a family shopper will say they would contact or visit Second Wind, because a number makes the value of buying easier to judge.

**Model:** The model that will be used is Claude Sonnet 5.5, with the same settings for every trial and memory off. 

**Persona and** **Prompt**: “You are a parent in Iowa City on a tight budget, shopping for discounted sports equipment for your child's upcoming season. You have already looked at two other shops and will only contact one, so you are looking for a reason to pick this one. Treat the business below as real. Read the page and decide whether you would contact this business (call, email, or visit the shop). Answer yes or no, then give one sentence of reasoning.”

**Trial Assignment:** I will generate 120 assignments at once in a spreadsheet column using =IF(RANDBETWEEN(0,1)=0,"A","B"), which will act as a coin flip for each trial. Then I will copy those results as fixed values so they do not change and run the trials in row order.

**Outcome:** ****The primary outcome is if the model/persona would contact this business via call, email, or visiting the shop. An answer that has a Yes will be measured as 1, and anything else such as No, Maybe, or other answers, will be measured as 0. The full output will be kept for every trial and no trial is duplicated.

**Sample Size and Date:** ****The sample size will be 120 trials in total, with about 60 per version. I will only stop when I have run all 120 trials and not look at any Yes or No outcomes until the end. I expect to reach the total sample size by around November 15 or 16, before the latest allowed launch date.

**Comparison and Decision:** I will compare the share of Yes answers in Version B to the share of Yes answers in Version A using a z test. I will report the difference, including the standard error, z score, p-value, and a 95 percent confidence interval. The significance level will be set at 0.05. The result that would count as support for my hypothesis would be Version B’s yes share is higher than Version A’s and if p < 0.05. I will only use Version B if I see that the hypothesis is supported.
