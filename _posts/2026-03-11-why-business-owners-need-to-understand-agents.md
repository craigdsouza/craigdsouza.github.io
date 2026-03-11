---
layout: post
title: "Why Business owners need to understand agents"
date: 2026-03-11
tags: [AI, agents, business]
image: /img/posts/2026-03-11-why-business-owners-need-to-understand-agents/agents-blog-header-blueprint-quilt-mixed-media.png
---


## What are agents?
![](/img/posts/2026-03-11-why-business-owners-need-to-understand-agents/agents-blog-header-blueprint-quilt-mixed-media.png)

If you're reading only popular traditional media outlets on AI, you know something is happening, but you're unsure of what. You know you're being told your industry could be disrupted, but as a business owner , you're not being advised what you can do to avoid being disrupted. You've probably heard of chatGPT. You may even be using this and other language models to frequently answer your queries. If that's all your doing I'm afraid to say you're only scratching the surface. I'm here to tell you that you need to understand `Agents`. What are agents? They're simply language models (probabilistic) paired together with deterministic tools. You see, language models are creative. Their creativity is an essential ingredient in their problem solving ability. However at times the lines between creative answers and wrong answers get blurred. This makes LLMs by themselves unstable. They need a *harness* , i.e. tools that are deterministic in nature that LLMs can use to produce outputs with greater accuracy. 

## What can Agents do today?

AI has changed and with it our understanding of the term must evolve. From 2022-2023 AI primarily meant chatbots like chatGPT. Since 2024, AI came to mean Agents, more specifically Agents developed for Programming. Since the turn of 2026, its clear that AI and `Agents` mean something more. Agents aren't only programming, they're engineering software - from architecture design to development and testing. Early adopters are already seeing results of early experimentation with Agents. Some companies are deploying Agents to full-time deployment.  The Pune edition of the [Fifth Elephant Conference](https://hasgeek.com/fifthelephant/2026-pune/) (February 27-28th), organized by Hasgeek at Nutanix's Hinjewadi campus was one such event that saw many early adopters congregate together. 

![](/img/posts/2026-03-11-why-business-owners-need-to-understand-agents/clint-open-floor-office-v1.png)

Nearly every technology company now uses AI agents for code generation, the number one use case. This means using AI to develop new product prototypes and even launch features. That isn't sufficient though. If your product team is launching new features everyday your QA team needs to keep up. Manas Chaturvedi from IDfy (risk evaluation and fraud detection) talked about how their QA teams began using AI agents to write and maintain tests for software, relegating their QA engineers to a more supervisory role. 

Prasanth Jayaprakash (Equal Experts) shared how their team built a lead generation system from scratch, not using agents , but using AI to accelerate software development for the pipeline. Neha from the retail company Target described how Agentic Generative AI (aided by classical Machine Learning) is helping validate and enhance item data (i.e. products sold by Target) including marketing description and images.

It wasn't only software companies. Himanshu Agrawal from Johnson Controls talked about experiments in having the operations of buildings - lighting, energy generation, HVAC etc. orchestrated by AI agents. These agents are fed data - sensor telemetry readings, building plans and more and given an objective. The agents software architecture allows it to reason over this data, develop hypotheses and propose preventive maintenance or work orders.   

## Evaluating the work of agents
Having said this, the agents we're talking about are still better thought of as toddlers, they need hand-holding. Eventually you can expect them to outdo us but at this stage, you should expect them to make mistakes every once in a while. Thus our role as agent-builders is to 
1) give the agent a goal, preferably a measurable goal and a metric for it to know if it has accomplished the goal or how close it is to doing so. 
2) to provide assistance in the form of context, guidelines and sometimes hard constraints. This one gets less relevant over time as the AI models that power AI agents get more intelligent. 

![](/img/posts/2026-03-11-why-business-owners-need-to-understand-agents/agent-workflow-validation-v4.png)

As [Atharva Raykar](https://atharvaraykar.com/), from Nilenso (a tech co-operative) talked about, "to prevent errors from compounding" we need to design the agents workflows as multiple units of work , gated by mechanisms to verify correctness of the output at each stage. Evaluation was a running theme through the talks. Himanshu put it as "the LLM only proposes (building controls)", the system validates. [Prasanna Bhogale](https://theclarkeorbit.github.io/pdfs/causality_fifthel_pune2026.pdf) (Romulan AI) described how encoding the knowledge of professionals down (as causal graphs) can ensure AI agents don't fall into a trap of confusing correlation with causation. In a hands-on session, Kiran Kulkarni and Utkarsh Dighe (unravel.tech) in a [hands-on session](https://github.com/unravel-team/real-agents-workshop) showed how we don't have to come up with the perfect prompt to chat with AI. We can have AI agents optimize on different prompt styles until a metric we care about is maximized. 

## Agents for domains outside software

Ok, but wait, what if you're not a technology company? What if most of your employees don't write code? Does AI still have relevance for you? Absolutely yes! Your team may not write code but you still have institutional knowledge , workflows and Standard Operating Procedures (SOPs). Let's say that you are a law firm. A part of your work is reviewing contracts. You have a standard template that you expect the contracts to be in. You can ask an Agent to review the contract that you've received against the standard template and flag any deviations, in plain English. Without agents you would have either had a para-legal spend hours reviewing the contract in detail or hired a software developer to automate the scanning of the contract. 

![](/img/posts/2026-03-11-why-business-owners-need-to-understand-agents/non-tech-ai-agents-wordcloud-v1.png)
Agents are inherently doers and the breadth of their inbuilt skills is vast. But agents don't necessarily understand company context. That's where SKILLS come in.
### SKILLS
The primary UI through which you might leverage agents is through Claude's Co-Work, Google's Anti Gravity or Open AI's Codex which all teach the concept of Agents with customizable SKILLS. These SKILLS are nothing but simple markdown (plain-text) documents where you store objectives, detailed guidelines, SOPs, and hard constraints written down in plain English. This way if you have a process that repeats but isn't the same every-time, you would write it up as a SKILL to save employees time. They can simply invoke a SKILL instead of repeating instructions. Agents in Claude for instance can use SKILLs once invoked to manipulate documents in most popular formats, Word, Spreadsheets, Slides. They can also connect to most popular Cloud services. Anyone can write up a SKILL document, but you would typically take the assistance of AI in a chat interface to write it up. 

A SKILL is not simply a software program written in human language. Its much more. SKILLs are inherently flexible. This means that if we give an Agent a SKILL document for instance with guidance on how to fetch data from a particular website and the guidance in the document doesn't match the reality the Agent is able to understand the higher level objective described in the SKILL and find other ways to achieve the objective. 

![](/img/posts/2026-03-11-why-business-owners-need-to-understand-agents/skills-plugins-handoff-v1.png)
### Plugins
Often times problems are complex enough that sub-processes can be defined. These problems then require multiple SKILLs rather than a single one. A simple example is the work of a marketing team. Marketing involves working with material that goes onto different surfaces (website, product, brochure, social media etc). This involves review of copy and images for brand consistency and technical aspects, such as dimensions. The collateral then has to be repurposed for each surface. SKILLs can come in at each stage, whether review or repurposing. This leaves the marketing team to focus simply on the ensuring the Agent is optimizing for the correct metric, one that is relevant for the business. This is where human judgement and accountability is important. Agents might even choose metrics in some cases, but in the end a human is accountable. 
## Conclusion
This is just the beginning. AI Agents are beginning to prove their usefulness in less technical domains of knowledge work. You can think of agents as being packaged expertise of specialists that can be run by generalists. A well organized business, empowered by agents can now take on the work of 100 people with a team of 10. Many projects previously thought of as impossible or economically infeasible now become possible with agents. Their implementation can amplify the business's top line and optimize its bottom line. 

The bottleneck no longer is expertise, its judgement. So what are you going to have your agents build?!
