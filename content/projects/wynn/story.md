---
title: Story
---

<!-- {{< centerHeader >}}Initial Discovery{{< /centerHeader >}} -->

{{< smallHeader >}}Problem{{< /smallHeader >}}
{{< prominentText >}}How do we reduce concierge call volume so that desk staff could focus on more important matters?{{< /prominentText >}}

For this project, the primary business goal was reducing concierge call volume so they could focus on front-desk matters that really needed them.

For the user, the benefit is reducing friction for basic tasks like room control, ordering amenities, and making restaurant reservations.

---

{{< smallHeader >}}Research{{< /smallHeader >}}
{{< prominentText >}}Beginning to understand users with proto-personas{{< /prominentText >}}

Due to budget restrictions and a long distance from Wynn Resorts, we didn't have an opportunity to do up-front user research with actual guests at the hotel, though we knew there was interest from an internal survey that Wynn had conducted.

{{< statCard >}}
## 66.8%
of 40,000 guests surveyed said they would book a room with Alexa
{{< /statCard >}}

In light of these constraints, I designed four proto-personas: educated guesses at the sort of people who might be using Alexa to make reservations at a restaurant. These were not informed by any new research, outside of our conversations with subject matter experts. But they helped us develop a shared understanding, and facilitated prioritization efforts going forward.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_protopersonas.png" 
    class="wider" >}}

The main distinctions between these customer segments:

1. How familiar each persona is with Wynn/Encore’s offerings
2. Whether that person wants to explore or knows precisely what they want
3. Whether the person is alone or has a family. In other words, if they have other needs they need to negotiate.

Drawing from these four proto-personas, and in discussion with Wynn, I acted as product manager in drawing up core user stories that would guide our initial efforts.

<!-- {{< centerHeader >}}Design{{< /centerHeader >}} -->

---

{{< smallHeader >}}Rapid Prototyping and Scripting{{< /smallHeader >}}
{{< prominentText >}}Rapid prototyping of key user stories{{< /prominentText >}}

Before I script (and constantly throughtout the process), I talk everything I write out loud. This is important for at least two reasons:

1. It helps me keep the tone conversational
2. It reminds me that what I write will be heard, not read. It's the aural/audio equivalent of a napkin sketch.

Here's a recording of my first "talk-to-myself" process for the restaurant reservation flow, a high-priority flow.


 {{< figureSound
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_recording_1_iteration1.mp3"
    title="Aural Wifreframe: First iteration, personal voice memo"
    id="wynn-wireframe-1"
    class="wide-standard" >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_scripts_1.png" 
    class="wider" >}}

Though awkward and filled with too much of my own personality, it served as a starting point. I put it down on paper, and worked through several iterations, with the scripts evolving in a parallel fashion. I tested these informally, in stand-ups or with family and friends, to refine the overall flow.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_scripts_2.png" 
    class="wider" >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_scripts_3.png" 
    class="wider" >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_scripts_4.png" 
    class="wider" >}}

This culminated in a final iteration.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_scripts_5.png" 
    class="wider" >}}

{{< figureSound
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_recording_2_iteration5.mp3"
    title="Aural Wifreframe: Fifth iteration, recording of Alexa"
    id="wynn-wireframe-2"
    class="wide-standard" >}}

<!--
{{< figureVideo
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_videoprototype.mp4"
    title="Prototyped interaction, ahead of moderated usability testing"
    class="wider" >}}
-->

Hearing the final version, I had some reservations (pun intended). Although on paper, it had seemed like a good idea to split the "day" and "time" questions, it sounded awkward. And we had designed this for the persona who knew what they wanted ("The Familiar") , instead of for the more likely personas: people who did not necessarily know what restaurant they would like ("The Adventurer" and "The Parent").

Still, through the process we had aligned on the Wynn team's business objectives, as well as important voice and tone considerations. I felt good about launching into some usability testing.

---

{{< smallHeader >}}VUI Design / Content Strategy{{< /smallHeader >}}
{{< prominentText >}}Managing the complexity of hundreds of conversational flows{{< /prominentText >}}

As a conversational designer, I always begin with how humans speak. But how computers understand that speech is also important. To help the computer understand natural language, I have to detail intents﻿—understanding the different things that a person might want from a conversational interface.

In working with the subject matter experts at Wynn, we came up with nearly 100 intents—ranging from questions about amenities, night clubs, restaurants, facilities, car rentals, and nearby attractions. Each of these had an average of 30 utterances. And I wrote approximately 400 text-to-speech (TTS) responses that Alexa would utter.

{{< wrappers/grid class="wide grid-small" >}}

{{< statCard >}}
## 100
Intents
{{< /statCard >}}

{{< statCard >}}
## ~3000
Utterances
{{< /statCard >}}

{{< statCard >}}
## ~400
TTS Responses
{{< /statCard >}}

{{< /wrappers/grid >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_vui_1.png" 
    title="The beginning of a scripts document I wrote, outlining 80+ scripts / flows" 
    class="wider" >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_vui_2.png" 
    title="Part of our 'State Machine Diagram', a critical handoff document. Each grey circle represents an intent (something someone can say), and each blue box represents response." 
    class="wider" >}}

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/wynn/wynn_vui_3.png" 
    title="Part of a spreadsheet I wrote, outlining the different things somone can say to express each intent." 
    class="wider" >}}

---

{{< smallHeader >}}Launch{{< /smallHeader >}}
{{< prominentText >}}Assessing the impact{{< /prominentText >}}

Wynn launched a trial period in a few rooms, and after some positive feedback, it rolled out to all rooms. And from there, it appeared to be a big success. Some of the key stats from the project:

{{< wrappers/grid class="grid-large wide" >}}

{{< statCard >}}
## 85.6%
found the Alexa flow easy or very easy to use
{{< /statCard >}}

{{< statCard >}}
## 83.7%
were happy or very happy with the service
{{< /statCard >}}

{{< statCard >}}
## 4.8k
questions looking for bar or restaurant recommendations in the first two months, signicant for a voice-only application
{{< /statCard >}}

{{< statCard >}}
## 12k
questions just about the hours of operations of bars, restaurants, and workout facilities in the first two months
{{< /statCard >}}

{{< /wrappers/grid >}}

Although our team never got access to the metrics around concierge volume, we had reasonable grounds for considering the voice application a success, at least as a pilot. In the first two months, it handled 16.8k utterances. Across 4900 rooms in 60 days' time, that's 280 utterances a day. Said one executive:

> "[Has the Wynn skill been successful?] Are you kidding me? Alexa is answering more than 12,000 inquiries a month just about our hours of operations for our 18 bars and restaurants, spas, and workout facilities. Even if you split that number in half, that's the equivalent of a full-time employee."
> 
> -Wynn Resorts VP of Operations

The hestitation is that we never learned whether that was evenly distributed across rooms or that number was due to a few "power-users." And of course, at only 280 utterances a day, that means a significant number of devices were never interacted with on a per-day basis, though we also never learned the booking rate of these rooms during this two-month experiment.

Still, at least to management and the users polled, it appeared a success. [Amazon published their own case study for this](https://developer.amazon.com/en-US/alexa/alexa-for-hospitality/wynncase), advertising its success in hopes to appeal to other hotels. It seemed to have worked—[Marriott Hotels adopted a similar pilot strategy](https://www.hotelmanagement.net/tech/alexa-for-hospitality-marriott-adds-amazon-to-guest-experience-0), adding Amazon Alexa devices into hotels shortly after Wynn did.

<!-- In retrospection, what would I have done differently? And what might I have attempted had we been able to iterate on the product?

* **Establishing a clearer analytics strategy.** I would love to have helped Wynn think through, from the very beginning, about specific conversion KPIs. (Analytics for conversational AI platforms were still relatively new, and tracking conversions was still not an easy thing.) How many restaurant reservations were placed? Where in the conversational did people abort? How many utterances were said that had no matching intent we'd anticipated? In addition, we never got direct access to the metrics around whether actual concierge volume actually went down. Did Alexa displace calls to concierge? If so, why? If not, why not? In addition to these questions, we never figured out how to integrate Wynn's own metrics with the voice metrics. For example, it would have been great to know the percentage of hotel rooms with an Alexa device in it booked on any given day, so we could look at usage numbers in light of total possible users for each day.

* **Making a stronger case for early usability testing.** I wish I had fought harder to argue to our client that early prototyping was worth it, in spite of the cost and distance. We ended up developing a VUI interface with nearly 100 intents across a variety of domains without evaluative research with any actual guests. We were able to receive some direct feedback related to restaurant reservations after the soft launch, and I did some guerrila usability testing with friends and family. But the lack of direct access throughout pained me as a designer.

* **Working more closely with Wynn's internal team.** As an agency, we were very peripheral to Wynn's internal product and IT team that would be implementing this. It was this lack of close relationship that hurt our ability to conduct on-site or remote testing with real guests, or get direct access to key metrics. On later projects, I learned the importance of establishing contact with the right teams and people to secure access to real people in real time throughout the project.

* **Researching multi-lingual and cross-cultural performance.** In the course of researching personas, I realized that a sizable percentage of guests at Wynn Resort were visiting from other countries or cultures. By one estimate, 20% of the nearly 42 million visitors to Vegas in 2018 were international tourists. I wasn't able to test with international visitors, and that means several guests were probably frustrated that either their language or their accent was a barrier to use. -->

---

{{< caseStudyCTA >}}
## Want the whole story?
Whether you're a hiring manager or recruiter wanting more details, or a fellow designer wanting to discuss the fine craft of design with a friend, feel free to [reach out](mailto:hello@bryansebesta.com).
{{< /caseStudyCTA >}}