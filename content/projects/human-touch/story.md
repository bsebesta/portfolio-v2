---
title: Story
---

{{< smallHeader >}}Understanding the Problem / Complexity{{< /smallHeader >}}
{{< prominentText >}}Determining the users and the scope of the challenge{{< /prominentText >}}

Our initial discovery was focused on stakeholder interviews. We had access to a variety of key stakeholders responsible for shaping the project, and after reviewing the product and existing apps intensively, I began to iterate on key research questions we needed to answer from stakeholders.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_researchquestions.png" 
    class="wider" >}}

From there, we went through a variety of stakeholder interviews, talking to critical people from sales, product, and customer support to identify priorities and any potential pain points. I put together a four-page report, summarizing findings and leading into strategy.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_researchreport.png" 
    class="wider" >}}

A key hypothesis we hit upon was realizing that **we needed to simplify choice** for everyone

{{< calloutBox title="Hypothesis" class="wide" >}}Choice should be radically simplified, as most customers only use a few routines from the available 38 _and_ a voice interface is not ideal for browsing.{{< /calloutBox >}}

As you'll see below, this hypothesis, while simple, led us to rethink the entire experience of selecting a massage.

It should be mentioned that while we were focused on stakeholder interviews, we were also creating an initial list of user stories to design for based on our knowledge of the API. I facilitated this process by mapping our ideas onto a virtual whiteboard, and organizing them into a graph that allowed us to easily see priority and feasibility.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_storyprioritization.png" 
    class="widest" >}}

In parallel with the stakeholder interviews, we knew we needed to get a few key flows right for this Virtual Therapist idea—specifically, onboarding and the actual experience of massage selection.

---

{{< smallHeader >}}Redesigning Onboarding{{< /smallHeader >}}
{{< prominentText >}}Rethinking the onboarding and customer conversation process{{< /prominentText >}}

The app already existed, but a Virtual Therapist did not. So we devised the following flow as part of onboarding, triggered by the presence of the Super Novo X chair we were designing for.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_screenflow_onboarding.png" 
    class="wider" >}}

We knew that, from this very first moment, we would need to ask questions to facilitate a smarter massage selection. The remote, after all, had **38 massage options**. And from our research, we knew that most of these were not used or explored.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_remotedetails.png" 
    class="wider" >}}

And it makes sense! Even though the remote says "The easiest way to enjoy a massage is to simply choose from 38 preconfigured auto programs," that't not actually easy. [Research into decision-making suggests](https://thedecisionlab.com/reference-guide/economics/the-paradox-of-choice) that too many choices can lead to paralysis or dissatisfaction with any choice that _is_ made. Further, many of the choices on the remote were shrouded in mystery. Many people would not know what a "Swedish" or "Shiatsu" massage was, even after using the chair for some time.

So our hypotheses: a better choice architecture would:

1. Simplify, compartmentalizing choice into salient buckets
2. Educate, helping people understand _what_ they were choosing
3. Facilitate conversational choice

Through some iteration, we landed on the following flow, which we realized would allow anyone to reach _most_ of the 38 flows while radically simplifying the process.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_flow_onboarding.png" 
    class="wider" >}}

I then drew out a flow, using low-fidelity wireframes to keep the design-build process as tight as possible (and to focus stakeholders on the functionality).

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_screens_onboarding3.png" 
    class="wider" >}}

{{< figureVideo
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_prototype_onboarding.mp4"
    title="Prototyped interaction using the low-fidelity wireframes"
    style="max-width: 400px" >}}

In addition to showing the above designs to stakeholders, I also wanted to make sure that we made the assumptions _incredibly explicit_, both for communicating the principles underlying these flows and in providing a strong foundation for any usability testing we would do down the line.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_assumptions.png" 
    class="wider" >}}

The stakeholders, upon seeing the designs and the assumptions laid out, were excited.

---

{{< smallHeader >}}Redesigning Onboarding{{< /smallHeader >}}
{{< prominentText >}}Imagining how voice would integrate with the app{{< /prominentText >}}

With everyone _onboard_ with the _onboarding_, we had the fundamentals in place for training users on how to prompt for specific massages. We prototyped how this might look.

{{< figureImage src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_screens_onboarding2.png" class="wider" >}}

{{< figureVideo
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_prototype_selection.mp4"
    title="Selecting a massage" 
    style="max-width: 420px" >}}

We knew that, based on how users had selected preferences, this flow could change quite a bit. I proposed some of the following scripts.

{{< figureImage src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_script_1.png" class="wider" >}}
{{< figureImage src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_script_2.png" class="wider" >}}
{{< figureImage src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_script_3.png" class="wider" >}}

In addition to the above screens, we also prototyped two other flows: a "feedback" screen, allowing for quick adjustment to settings. And, of course, a settings screen for deciding on settings.

{{< figureImage 
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_screens_feedback.png" 
    class="wider" >}}

{{< figureImage 
src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_screens_settings.png" 
class="wider" >}}

{{< figureVideo
    src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_prototype_feedbacksettings.mp4"
    title="Giving feedback and changing settings" 
    style="max-width: 420px" >}}

{{< smallHeader >}}Transitioning to High-Fidelity{{< /smallHeader >}}
{{< prominentText >}}Creating a high-fidelity visual system{{< /prominentText >}}

{{< figureImage 
src="https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/human-touch/humantouch_preview_2.webp" 
class="wider"
title="Selections from the high-fidelity onboarding flow" >}}

---

{{< smallHeader >}}The Project's Conclusion{{< /smallHeader >}}
{{< prominentText >}}Due to priorities at Human Touch, the project stopped before we could rigorously test our assumptions{{< /prominentText >}}

One of the realities of agency life is _lots of contingency_. Due to the hardware around the chair taking longer than expected to deliver, the project was paused—and then I left. This left us with lots of research, some initial designs, and lots of untested assumptions.

---

{{< smallHeader >}}Retrospective{{< /smallHeader >}}
{{< prominentText >}}Had I been able to finish the project what would I have focused on?{{< /prominentText >}}

I would have focused on usability testing around the onboarding and massage selection flows. Some critical questions I would have liked to answer:

1. Did the goals we outline (relax specific muscle groups, tension relief, stretching, athletic performance) make sense? Do most users have one specific goal that they can prioritize easily? Or do most have multiple goals? And if the latter, would this screen have been difficult?
2. Did framing the specific massage names in "simpler" language, like renaming "Swedish" as a "Moderate" massage, make sense? For users primed by these screens and the language we use, what _words_ do they use?
3. Would users actually use the Virtual Therapist? Or would they select a massage using other means?
4. Is the voice and tone we selected (only implied by the time our project paused) a good fit for consumers of massage chairs? Did we strike a good balance between an "expert therapist" and the voice of a chair?

<!--

---

{{< caseStudyCTA class="wide" >}}
## Want the whole story?
These were highlights from the process, but if you want the whole story, reach out to me [via email](mailto:hello@bryansebesta.com) or [LinkedIn](https://www.linkedin.com/in/bryansebesta).
{{< /caseStudyCTA >}}

-->