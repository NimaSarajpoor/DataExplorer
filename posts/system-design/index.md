---
title: "system design: where to start?"
description: "Finding a roadmap for system design can be challenging!"
date: "2025-06-26"
categories:
  - system design
image: system-design.png
---

## What is "system design"?
According to [wikipedia](https://en.wikipedia.org/wiki/Systems_design), the basic study of system design is the understanding of component parts and their subsequent interaction with one another. Systems design has appeared in a variety of fields including computer/software architecture.

## When did I first face challenges in system design?
I was working on a project that was running 24/7. I was taksed with finding a solution for backfilling a large amount of data that was not processed in the past since the system was down. I had to think about different aspects such as: <br>
* How to ensure that the system can handle the large amount of data without crashing? <br>
* How to ensure that the data is processed in a timely manner? <br>
* What to do if the system fails during the backfilling process? <br>
* Can it run in parallel with the daily processing? Is there any dependency? <br>
* What was the reason of failure? Has there been any change in the format of incoming data? <br>


Each system design problem is unique. However, I think there should be some ways to improve such skills. In programming, we know that each problem can be unique. But there are some practices like [leetcode](https://leetcode.com/) that can help us to improve our skills. I think the same applies to system design. So, I did a quick search and I am going to share what I've found online.

## Resources to learn system design
* [System Design Interview – An insider's guide](https://www.amazon.ca/System-Design-Interview-insiders-Second/dp/B08CMF2CQF)
* [Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems](https://www.amazon.ca/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)
* [Grokking the System Design Interview](https://www.educative.io/courses/grokking-the-system-design-interview?utm_campaign=system_design&utm_source=google&utm_medium=ppc&utm_content=search&utm_term=course&eid=5082902844932096&utm_term=grokking%20the%20system%20interview&utm_campaign=%5BNew%5D+System+Design-Search-EU-Nov+24&utm_source=adwords&utm_medium=ppc&hsa_acc=5451446008&hsa_cam=21874477566&hsa_grp=175905880259&hsa_ad=735450354425&hsa_src=g&hsa_tgt=kwd-903484928147&hsa_kw=grokking%20the%20system%20interview&hsa_mt=e&hsa_net=adwords&hsa_ver=3&gad_source=1&gad_campaignid=21874477566&gbraid=0AAAAADfWLuT0LEe_NOnzSNDAv-MeepMgI&gclid=EAIaIQobChMIjZaDyrWPjgMVHET_AR13_gpbEAAYASAAEgJ12PD_BwE)

* [codemia system design](https://codemia.io/system-design)
* [system design primer](https://github.com/NimaSarajpoor/system-design-primer) 
* [codewars](https://www.codewars.com)
* [blogs to follow](https://workat.tech/system-design/article/best-engineering-blogs-articles-videos-system-design-tvwa05b8bzzr)

## First step?
I am not sure but as I was reading opinions on reddit, I realized that I should probably start with the book [System Design Interview – An insider's guide](https://www.amazon.ca/System-Design-Interview-insiders-Second/dp/B08CMF2CQF).