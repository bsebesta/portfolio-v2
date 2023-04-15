---
title: Story
---

<!--
{{< caseStudyCTA class="wide" >}}
## Want the whole story?
Below are highlights from the process, but if you want the whole story, reach out to me [via email](mailto:hello@bryansebesta.com) or [LinkedIn](https://www.linkedin.com/in/bryansebesta).
{{< /caseStudyCTA >}}

---
-->

{{< smallHeader >}}Process{{< /smallHeader >}}
{{< prominentText >}}This project's initial complexity emerged from organizational and technical challenges{{< /prominentText >}}

...?

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/va-health/vahealth_process.png" 
    class="wider" >}}

The challenges were mostly the nature of the organization (a bureaucracy with a lot of red tape), the variety of stakeholders with conflicting priorities (patient safety, privacy, feature prioritization, etc), information architecture hurdles, and technical innovation (no sandbox or APIs we could test initially).

---

{{< smallHeader >}}Problem{{< /smallHeader >}}
{{< prominentText >}}The VA wanted us to explore an accessible, voice-first interface for veterans refilling prescriptions{{< /prominentText >}}

The US Department of Veterans Affairs provides prescriptions and prescription management to veterans across the nation. At the outset of the project, veterans could manage their prescriptions through web, mobile, and IVR touchpoints. But the IVR system was cumbersome, and the VA wanted to update their service to allow veterans to order prescriptions using a more natural conversational interface on smart speakers, specifically with Amazon Alexa.

{{< calloutBox title="Hypothesis" >}}A natural language interface, available on consumer smart speakers, and executed well, would appeal to veterans young and old, abled and disabled. It could also free up pharmacists for more complex tasks.{{< /calloutBox >}}

---

{{< smallHeader >}}User Research{{< /smallHeader >}}
{{< prominentText >}}
Understanding our users without direct access to them{{< /prominentText >}}

The VA is a large, bureaucratic, government agency. For this reason (and an overabundance of caution about veteran safety), we could not access real veterans, or real veteran data, until late in the game—after we’d built quite a lot, and after we’ve met a variety of hurdles and approvals.

Much of my role, therefore, was doing the best within these constraints—relying on stakeholder interviews, subject matter experts, previous personas developed by the VA, and audits of the existing web / mobile ecosystem. From these, I started to draw out some hypotheses.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah-discovery-artifacts.png" 
    class="widest" >}}

{{< centerHeader >}}Design & Research{{< /centerHeader >}}

{{< smallHeader >}}Defining the Scope{{< /smallHeader >}}
{{< prominentText >}}Focusing in on basic prescription refills—as well as listing prescriptions and tracking shipments{{< /prominentText >}}

We now had four things we had to keep in mind.

1. Technical constraints of Amazon Alexa
2. Technical constraints of the VA’s API
3. Practical limitations of a voice-only interface
4. Likely expectations of veterans

From this, we decided to focus on a small list of features for the MVP. Along with the basic mechanic of refilling eligible prescriptions, we also wanted to allow veterans to list all their prescriptions (whether they could refill them or not) and track shipments.

With these features decided on, we now needed to turn to the fifth thing to consider: stakeholder concerns.

---

{{< smallHeader >}}Communicating Design{{< /smallHeader >}}
{{< prominentText >}}Persuading client stakeholders regarding patient safety and best practices with voice interface design{{< /prominentText >}}

Early on, some stakeholders had the idea that veterans would request refills one-at-a-time, speaking aloud the prescription number of the pill bottle they wanted to refill.

Frankly, we hypothesized that few veterans would want to be tethered to their prescription bottle. After all, how is the voice app making a leap in accessibility if veterans have to read tiny print on a bottle to use the application?

But early thinking about the API indicated we might have to do this, so I drew up storyboards to help our team align on the context.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_storyboarding.png" 
    class="widest" >}}

As conversations progressed, we realized the API was more potent than we’d thought—we would be able to list our prescriptions. So we moved to persuade stakeholders by showing different versions and feature sets we could move forward with.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_scenarioevolution.png" 
    class="wider" >}}

We were excited to move forward, but several client stakeholders were still very concerned around patient safety. Some stakeholders wanted the voice application to have all the features of the mobile or web interfaces. One key stakeholder in particular was very difficult, until we realized that they didn’t see how the “MVP” could meet patient safety standards.

So with my PM, I helped establish a roadmap schedule, assuring all involved that for our purposes, “MVP” meant the simplest version of the app we could test with. We wouldn’t release the larger voice app until we had all features built. Though some elements of this plan felt unnecessary to us internally, it reassured stakeholders—allowing us to move forward.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_designstakeholders_2.png" 
    class="wider" >}}

---

{{< smallHeader >}}Information Architecture / Content Strategy{{< /smallHeader >}}
{{< prominentText >}}Preparing to prototypew with scriptwriting, aural wireframes, and outlining a language model{{< /prominentText >}}

We had finally gotten sufficient buy-in on our designs to move forward with testing. To test, however, we had to have a fairly robust prototype. To prepare, I outlined a voice and tone for the product, and wrote copy for standard and edge use cases. In total, this resulted in a 50-page document outlining all copy and wording that would be used in the voice application.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_scripts.png" 
    class="wider" >}}

Each of these scripts paired with an “aural” (or audio) wireframe. Unlike visual wireframes, which can be represented statically in space, voice interfaces are experienced temporally, in time. So while a script was helpful, it was not a “full representation” of what the experience would be like.

{{< figureSound
    src="https://bsebesta-portfolio.s3.us-west-004.backblazeb2.com/case-studies/va-health/VAH_AuralWiframes_PrescriptionFlowFull.mp3"
    title="Full prescription refill flow"
    id="vah-wireframe-3"
    class="wide-standard" >}}

Working from these scripts was a major exercise in designing the information architecture of the skill. We identified 52 intents—52 things a veteran might want from this skill—and matching utterances. For every intent, like asking for dosage instructions, there were many ways a veteran might express that. “How am I supposed to take this?” “How do I take this?” and “What are the dosage instructions?”

Parallel to this activity, I also drew up detailed plans of how the VUI would work for engineers to work from. Internally, we referred to these as “State Machine Diagrams.” Several of them took the form of multimodal swimlanes.

{{< figureImage 
    src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_smd_nlu-2.png" 
    class="wider" >}}

All of the culminated in an ability to create a working app. Below is the design, featuring accompanying visuals I helped design (within the constraints of Amazon Alexa’s visual design system).

{{< wrappers/grid class="wider grid" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/echoshow8-gen3-black-diagonal3-1.png" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/echoshow8-gen3-black-straight2.png" >}}
{{< /wrappers/grid >}}

{{< figureVideo
    src="https://bsebesta-portfolio.s3.us-west-004.backblazeb2.com/case-studies/va-health/vahealth-prototypevideo.mp4"
    title="Prototyped interaction, ahead of moderated usability testing"
    class="wider" >}}

---

{{< smallHeader >}}Moderated / Unmoderated Usability Testing{{< /smallHeader >}}
{{< prominentText >}}Learning how veterans refill prescriptions through moderated usability testing{{< /prominentText >}}

Finally, we came to testing. The focus was on moderated usability testing we would conduct at a VA facility in Virginia. We would have 8 participants, most of whom had some kind of disability (low vision being the most common). Eight participants wasn’t enough to give us statistically significant results, but it would help us catch major errors and de-risk the major flows.

{{< wrappers/grid class="wider" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/VAH_2022-04-29_UserTesting_picture4.png" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/VAH_2022-04-29_UserTesting_picture2.png" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/VAH_2022-04-29_UserTesting_picture1.png" >}}
  {{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/VAH_2022-04-29_UserTesting_picture3.png" >}}
{{< /wrappers/grid >}}

I led the design of the test and recruitment. I helped select screening criteria, send out pre-testing emails, and prepare test objectives and a field guide. And I conducted the interviews.

{{< calloutBox title="Testing Objectives" >}}
{{< rawhtml >}}
1. (Scenarios 1.1) Are the instructions for account linking clear? Can a veteran walk through this and enter their right credentials?
2. (Scenarios 1.2-1.5) Can a veteran understand Alexa's PIN flow?
3. (Scenarios 1.7) Do a majority of veterans have a sense of what each of these options will do? Does the information architecture make sense to them? Is the double-inclusion of "prescriptions" tricky? Could we shorten the first two menu items in any way?
4. (Scenarios 2.2.1-2.2.2) Is the yes/no prompt clear? If a veteran has a question while a prescription is presented, do they know what to do? (And if not, how do they behave?) Is the lack of a "yes" acknowledgement acceptable?
{{< /rawhtml >}}
{{< /calloutBox >}}

{{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_fieldguidetesting.png" class="callout__small wide" >}}

Testing went really well. Overall feedback was really positive, validating several of our hypotheses. Three stand-out quotes we shared later in a topline report with stakeholders:

{{< wrappers/grid class="wider" >}}
    {{< calloutBox title="Quote" >}}“Wow, how easy that would be! How easy is that! mean, if it works like that... God, yeah, please.”{{< /calloutBox >}}
    {{< calloutBox title="Quote" >}}“1000 super easy... I do MyHealtheVet [the web/mobile interface] right now, where I do my prescriptions on the app. [But] I have a hard time seeing the screen. If I could talk to it, I'd talk to it, because I love to talk.”{{< /calloutBox >}}
    {{< calloutBox title="Quote" >}}“That would be handy... in the sense that right now, I have to pull everything up on my computer. With this, I could be in any room of my house and pull it up. could be in my kitchen and be like, 'Ooh, am I going to run out of this?' and pull it up on my kitchen [Alexa], before I walk 3 rooms over and forget that I have to reorder my prescription. So yeah, having just that alone, because I take pills in different rooms depending on what time of the day it is, would be really handy.”{{< /calloutBox >}}
{{< /wrappers/grid >}}

In spite of the delayed usability testing, which is not ideal in any project, these results suggested that our early discovery efforts—drawing on personas, subject matter experts, stakeholder interviews, and audits of the existing ecosystem—were done well. The results visibly excited our team and our client, even the most skeptical.

I also prepared a testing guide for unmoderated usability testing we were planning to do ahead of a soft launch.

{{< figureImage src="https://www.bryansebesta.com/wp-content/uploads/2023/01/vah_uatfieldguide.png" class="callout__small wide" >}}

---

{{< smallHeader >}}
Being Mugged by Reality{{< /smallHeader >}}
{{< prominentText >}}
Amazon pulls the plug on consumer-facing medical voice apps just as we prepare for a soft launch{{< /prominentText >}}

Unfortunately, we faced a swift disappointment at the projects end. Just as UAT was about to begin, and as we were preparing to “soft launch” the Alexa voice app among family and friends, Amazon announced layoffs in departments associated with Amazon Alexa.

In the wake of these layoffs, we learned that [Amazon had dropped support for HIPPA compliant skills](https://voicebot.ai/2022/12/06/amazon-to-end-support-next-week-for-third-party-healthcare-alexa-skills-with-hippa-requirements/). (HIPPA laws are a series of regularly standard that outline the lawful disclosure of protected health information in the United States.) Without this support, the project, as we had envisioned it, was terminated. There was no way to launch a consumer-facing voice application for Alexa that dealt with medically-sensitive information.


{{< centerHeader >}}Takeaways{{< /centerHeader >}}

{{< smallHeader >}}How did it all end?{{< /smallHeader >}}
{{< prominentText >}}
Amazon pulls the plug on consumer-facing medical voice apps just as we prepare for a soft launch{{< /prominentText >}}

So how do you measure success on a long project like this—that never shipped?

Because the product never shipped, we never had access to statistically significant data—like conversion rates, total prescriptions refilled over this channel, total time spent on the product, and qualitative reviews. But it was not entirely unsuccessful. Two key business outcomes included:

* **Convincing skeptical stakeholders.** We managed to convince some very skeptical stakeholders that a natural-language, conversational interface—if executed well—would be valued by veterans, especially those with disabilities (e.g. low vision). The topline research reports and quotes from our interviews visibly excited these stakeholders, and excitement shouldn’t be discounted. Nor should the power of user research to be the most potent persuasion tool in product design. That research was what tipped the stakeholders toward buy-in.
  
* **Paving the way for an integrated conversational AI product strategy.** A consumer-facing Alexa voice application was never the endgame. This was always envisioned to pave the way to integrate voice inputs into the mobile app. In this modality, voice could work as a powerful input, and voice paired with visuals could work well as a powerful output. Although the Amazon Alexa chanel never worked out, conversations were being had about pivoting our work in this direction.

---

{{< caseStudyCTA >}}
## Want the whole story?
Whether you're a hiring manager or recruiter wanting more details, or a fellow designer wanting to discuss the fine craft of design with a friend, feel free to [reach out](mailto:hello@bryansebesta.com).
{{< /caseStudyCTA >}}