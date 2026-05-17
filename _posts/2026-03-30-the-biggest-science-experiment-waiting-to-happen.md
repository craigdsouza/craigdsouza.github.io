---
layout: post
title: "The Biggest Science Experiment Waiting to Happen"
date: 2026-03-30
tags: [AI, agriculture, food, polyhouse, precision-agriculture]
---

> **TLDR** : For anyone curious about what AI and controlled-environment agriculture could mean for food production and farmer incomes, especially in India. This post describes a real experiment where Claude was given full control of a tomato plant's growing environment, explains the plant science behind what it managed, and asks: what if we ran this experiment at scale across hundreds of plants simultaneously? The implications for agricultural productivity and farmer livelihoods could be significant.

# The AI that grew a tomato
On the 30th of December, 2025, a U.S. resident Martin DeVido based in Boise, Idaho sowed a tomato seed. Not outdoors, the frigid winter weather doesn't allow tomatoes to grow outdoors in Idaho. He sowed this seed in an indoor environment. He then gave Claude, Anthropic's AI model, full control over the physical environment that the plant could grow in. Claude could control via physical actuators the plant's exposure to light, its soil temperature, water availability, humidity and airflow. Claude also had inputs, via a camera that photographed the plant, CO2 sensors, RH sensors, air and leaf temperature sensors, soil moisture sensors. 

![Claude grows a plant LIVE](/img/posts/2026-03-30-the-biggest-science-experiment/live.png)
<p style="text-align: center; font-size: 0.85em; color: #888;">A Live view of Claude growing tomatoes in Idaho</p>

Claude has a rich in-built knowledge about the mechanisms by which plants grow:

- **CO2 uptake** — Plants take up atmospheric CO2 and turn it into sugars. Ambient air is ~420 ppm CO2; in an indoor environment, a fruiting tomato depletes this fast. Claude tracks it and injects CO₂ to keep photosynthesis running at full rate.
- **Vapour pressure deficit** — Measures the difference between how much water vapour the air can hold vs how much it actually holds. Too low (humid/cold) and plants stop transpiring; too high (dry/hot) and stomata close. Claude manages air temperature, humidity and airflow to keep VPD in the sweet spot.
- **Stomata regulation** — The tiny openings on a plant's leaf open and close based on the difference between air and leaf temperature. Keeping this difference optimal keeps the stomata optimally open for growth.
- **Root zone enzyme activity** — Enzymes in the root zone help plants absorb nutrients, but they slow down in cold conditions. Claude tracks root zone temperature and maintains it for optimal absorption.
- **Root zone moisture** — Too much or too little soil moisture restricts nutrient uptake. Claude tracks soil moisture with probes and maintains it in an ideal window with pulses of irrigation.
- **Photosynthesis** — Light provides energy for the plant to produce sugars. In certain growth periods, additional light can increase photosynthesis and fruit production. Claude tracks and schedules ON/OFF cycles and light intensity accordingly.
- **Thigmomorphogenesis** — Plants exposed to wind produce thicker stems to withstand it, and thicker stems support larger fruits. Claude provides a controlled air stream to trigger this response.

![Plant Growth Mechanisms](/img/posts/2026-03-30-the-biggest-science-experiment/infographic.png)
<p style="text-align: center; font-size: 0.85em; color: #888;">Plant Growth Mechanisms</p>

A critical thing to note here is that the maintenance isn't weekly or daily as it is with many agricultural systems. Claude maintains these variables in their optimal range by checking in on their values every 30 min. Moreover, the results from experiments like this show just how many challenges farmers are up against when growing on open fields. None of the variables are really under their control other than irrigation scheduling. Just as in Idaho the temperature is too cold for plant growth in winter, in much of India it is often too hot and summer crops are adversely affected by this.

[Watch: Claude grows a tomato](https://www.youtube.com/shorts/IEZY8bASy9Y)

# What if Claude grew 100 tomatoes
Claude can learn only so much from one experiment growing a single tomato plant though. 

> What if it grew 100 plants and tried something slightly different in each case? 100 experiments could mean many times more learnings and at a faster pace than a single run. 

Perhaps when learnings occur at this pace, we could rapidly increase the quantum and diversity of food production while at the same time reducing our material footprint(water and energy) and growing farmer incomes as a result. 

This is the real world equivalent of the accelerated learning that is happening in AI data centers everywhere. In the case of Large Language Models (LLMs like ChatGPT) learning and improving requires more text data. The text of the internet - all the literature that has ever been written about agriculture and plant growth - is only adequate as a starting point though. The learnings possible through literature saturate and experiments are necessary. 

In some domains such as robotics, a first step might be experiments in simulated environments (i.e. think virtual robots learning to walk). In domains such as agriculture too this might be possible. But all experiments must eventually move to the physical world. In this scenario, human beings can serve as the labour measuring inputs given to Claude and changing temperature , humidity etc via controls as per Claude's instructions. This is only likely to slow down the pace of experiments, albeit in the short run it might be necessary, to avoid the costs of Sensors and actuators. Either way, this appears to be an experiment just waiting to be done and the effects of its outcome on agriculture, especially in the developing world are likely to be very consequential. 

> The fast growth of polyhouse based agriculture in India, is a tailwind that can only help make this more likely than not. The village of Gurha Kumawatan has [the highest concentration of polyhouses in India](https://theplate.in/how-polyhouse-farming-in-rajasthans-desert-is-turning-farmers-into-millionaires/). 

![An aerial view of Gurha Kumawatan in Rajasthan](/img/posts/2026-03-30-the-biggest-science-experiment/polyhouse-arial.jpg)
<p style="text-align: center; font-size: 0.85em; color: #888;">An aerial view of Gurha Kumawatan in Rajasthan showing polyhouses in every direction. Photo: Kishore Ravi</p>


# Business models and who holds the IP
- 1) perhaps it is seed companies that do the experiments , not farmers, they certainly have the capital. They could perform 100 or even a thousand experiments with their seedlings and the results (the Intellectual Property) could become a recommended guidance to farmers on how to grow from sowing to appropriate harvest time. To ensure a return on investment they could charge a premium for seeds + guidance.

- 2) alternatively it isn't seed companies but infrastructure companies that, they build custom physical infrastructure ideally suited for fitting out with sensors and actuators. They could also provide the AI model which observes and controls the growth experiments and generates them IP. More the number of farmers , more the experiments and thus more valuable the IP. These companies business model is thus to ensure farmers a given return. They control the production and thus know the likely tonnage. The market price is always volatile though and thus they keep a larger margin in return for taking on the risk.

- 3) lastly, perhaps it is a farmer co-operative, that purchases the physical infrastructure from companies that only build , and don't operate them. Instead farmer co-operative themselves operate this collective infrastructure. Practically it means that the co-operative hires specialized employees who understand this infrastructure and can advise farmers on how to maintain it. They play a role similar to the private company, but in a co-operative structure. In this case, if it succeeds , its likely that farmers get to keep a larger part of the profits, but they in turn take on a larger share of the risk of market price fluctuations.

It remains to be seen which model will eventually succeed, perhaps none of the three and something else entirely. 

# Supply and Demand
I have so far largely talked about growing supply, i.e. better control of agricultural plants inputs can serve to increase production. However increased production doesn't guarantee the economic well being of farmers. Market demand fluctuations could easily move price downwards and erode away the benefits of increased production. 

This problem isn't solved by farmers growing more of the same thing but growing more of many different things. The same rule that applies in entrepreneurship applies here. If you have an undifferentiated product in a competitive market your margins are tight and total income is at the mercy of market demand. 

This is true for millions of farmers in India who are growing the same product (rice, wheat) for near zero margins. They do this however because they know that the market demand for rice exists. They don't really know if the demand for gooseberry does. Polyhouse AI aided experiments as we've discussed could help reduce this risk by increasing the tonnage produced per rupee input. 

This helps cushion any price volatility and ensure good incomes. A world in which farmers produce 100 different crops and thus compete less against each other is one that's economically better for them rather than the current world in which the large majority of farmers produce only ~5 different crops.
