---
title: Measuring progress against documentation quality goals -- a practical checklist to evaluate documentation
permalink: /docapis_measuring_impact.html
course: "Documenting REST APIs"
weight: 12.92
sidebar: docapis
section: devportals
path1: /docapis_managing_dev_portals.html
last-modified:
---

As you set goals for your role or team, you might want to measure your impact on documentation quality in some way. The main reason for measuring your impact should be to evaluate your progress against your goals. If you don't have any data to provide feedback on your efforts, it's hard to know if you're making a difference.

Additionally, metrics are essential for business reasons: upper management will invariably ask you for metrics of some kind (because what you can't measure, you can't manage). Metrics will also be key if you're making the case for a promotion (upleveling) or defending your performance during annual review time. Ultimately, though, you need metrics to answer this question: Is what I'm doing making a difference?

Despite the importance of metrics about documentation quality, they are an elusive, holy-grail type task that almost no one in the industry has nailed down. In this section, I'll provide a strategy for making metrics more approachable by scoring docs against a rubric of best practices.

{: .note}
Note that this isn't a tried-and-tested methodology here but rather something I am still developing and experimenting with. As such, I value your feedback. I also have a survey at the end to gauge agreement with various ideas.

* TOC
{:toc}

## Doc surveys

The first inclination many have when measuring documentation quality (how good your docs are) is to conduct surveys with users. After all, it doesn't matter what the technical writer thinks of the documentation; it's what the user thinks, and how successful the documentation was in helping the user in some task, right?

To a degree, yes, you can only really evaluate the usefulness of documentation from the perspective of a user going through the documentation with some tasks in mind. However, surveys are a difficult, inefficient way to go about measuring documentation quality for several reasons:

* Survey responses aren't actionable
* Users aren't available for surveys
* Unbiased survey questions are difficult to formulate
* Users are sometimes unreliable

### Survey responses aren't actionable

First, feedback from users about documentation is often too general and unactionable to be helpful. If you do a satisfaction survey and find that only 30% of users would recommend the documentation to a friend, what can you do with that information? If surveys indicate that your docs are poor and need improvement, can you act on that? Which docs? Which parts need improvement? Are they "confusing and useless"? What's confusing or unhelpful about them? All of the docs, or just parts? Is the feedback a general impression overall, or focused on a specific user scenario with a single documentation topic?

Without more specifics, the information falls flat and doesn't lead to any actionable follow-up. If you can't identify the friction points and areas that need to be fixed, what good are the survey results? They might only serve to depress the technical writers. In looking into ways to measure information quality, I found Yoel Strimling's article [Beyond Accuracy: What Documentation Quality Means to Readers](https://www.researchgate.net/publication/331088095_Beyond_Accuracy_What_Documentation_Quality_Means_to_Readers) to be spot on in identifying the issues with surveys. Strimling says that questions in all types of feedback (whether asked in surveys, focus groups, face-to-face interactions, or other) need to be specific so as to be actionable. Echoing the conclusions of other researchers, Yoel explains:

> But it is not enough for us to collect meaningful feedback about our documentation from our readers. We also need to be able to use the information we collect to take actions that will help us directly address and prioritize the issues that are important to them.

In other words, surveys alone, without actionable feedback, aren't enough. Reading feedback that says docs are poor, incomplete, outdated, disorganized, etc., doesn't give writers a clear sense of what needs to be done. As a practitioner, above all else I'm focused on the practical.

### Users aren't available for surveys

Another problem with surveys is that most technical writers don't have direct and continued access to users to survey them on a regular basis. I wrote about the challenge of [reconstructing the absent user](/simplifying-complexity/reconstructing-the-absent-user.html) in my series on Simplifying Complexity. It's unfortunate but the norm that technical writers have very little contact with their target users.

### Unbiased survey questions are difficult to formulate

Let's say you do have access to users, another challenge with surveys is how to formulate the questions. You have to be skilled in the way you pose survey questions to avoid bias in the responses. Strimling dives into research about survey formulation and lists the characteristics of a good survey. For example, questions must be "long enough to be useful, and short enough to encourage participation" (quoting Barnum). They need to be unambiguous, non-threatening, easily answerable, clear, unassuming, etc. Survey questions are hard to formulate. If you're a regular reader of my blog, you've probably seen a lot of small surveys I include with each article. I've learned that formulating survey questions is an art, and questions need to be simple, unambiguous, and easy to answer. At the same time, you have to consider what the actual goals of the survey are. Surveys are hard to do right.

### Users are sometimes unreliable

Finally, another problem with surveys is with audience unreliability. We base the value of our docs around the user's perspective, but what if users are unreliable or unhelpful? There's a lot of variation, subjectivity, and unreliability with survey responses. Sometimes people use docs as a scapegoat for other issues related to poor product design, company dissatisfaction, or other issues. Often when I'm taking a survey, I base my responses on one part of the product or docs that I've been using, not on the whole. One bad topic can taint the user's response of the whole, distorting the quality measure for the docs.

Additionally, people who respond negatively in satisfaction surveys might not be your target audience. You might have been writing for the 80% of your audience already familiar with a certain framework, but your survey might include someone new to the framework who found the docs worthless.

Other times users might respond so hastily that their responses are cryptic and vague. Or a user might complain that the docs are confusing, but that doesn't tell the writer how to fix the issue. A user might provide general feedback, saying that the docs felt like they needed polish, or that they had trouble understanding/following them, or that they seemed incomplete. But without more specifics, this feedback isn't all that actionable.

### What can replace surveys?

Note that I'm not entirely dismissive of surveys; I'm only being realistic. If the survey's purpose is to highlight the importance of documentation in general, how critical it is for complete and accurate documentation to help users complete tasks, great. But that's a different purpose than measuring documentation quality. A metric about the importance of docs would support resourcing for doc efforts or other goals for establishing tech comm's importance. But to make improvements with quality, you need information that is much more specific and actionable, and that's where general surveys tend to fall short.

Rather than sink too much time and energy into surveys as the only way to measure doc effectiveness, I propose a much more concrete and realistic approach to measuring doc quality: detailed rubrics to assess docs. The rubric must take the general qualities of measurement (e.g., clarity, accuracy, relevance, findability, etc.) and make concrete what these abstract qualities mean and how they are implemented. Also, while many scholars have defined characteristics for information quality, I've yet to see a rubric specifically focused on developer documentation. In the sections that follow, I will go into specific detail for describing information quality with developer docs.

## Rubrics

Rubrics are a scoring matrix (or framework, or simply a quality checklist) you use to evaluate and score content based on various criteria. If documentation fulfills the criteria of the rubric, it's likely that the documentation is high quality and would rate well in user satisfaction surveys. If highly rated user satisfaction surveys don't follow from fulfilling the rubric's criteria, the rubric is likely misguided.

Many teachers use rubrics when grading student essays (e.g., a category for language, organization, reasoning, etc.). Rubrics give teachers a more objective framework of established criteria to assess and score content. For students, rubrics hold the promise of simplifying and demystifying the grading process. Rubrics can give students a clearer idea of what teachers are looking for, and why they earned a B instead of an A, for example.

Although rubrics are common, many teachers feel they aren't actually helpful. This is because rubric categories are usually too general and high-level, and students struggle to understand how their specific essay performed against the generalized criteria. For example, in [Does Your Rubric Punish Students?](https://makethemmasterit.com/2018/06/30/does-your-rubric-punish-students/), Jeffery Frieden explains two problems with rubrics:

> Problem #1: They lack clarity to inform students of what they did, or did not do, in their work.
>
> Problem # 2: They are designed to communicate student deficits, not student competency.

For example, if a teacher marks a student low on the reasoning category (perhaps due to some logical fallacies), the student might not understand without more specific feedback, Frieden explains. For a "Below Average" essay, the teacher might check a box next to a Reasoning category that says, "The text provides data and evidence that attempts to back up the claim and unclearly addresses counterclaims or lacks counterclaims." But this doesn't clearly communicate to the student what the issue is or what needs to be done. Instead, the rubric because an easy way to justify a deficit without actually helping the student improve their writing.

In the tech doc world, common categories in rubrics are equally high-level and general. For example, you might assess documentation against the following criteria:

* Readability
* Clarity
* Context
* Accuracy
* Organization
* Succinctness
* Completeness
* Findability

In Strimling's essay, he looks at previous research on the attempt to define information quality and finds a wide range of different quality definitions:

<a class="noCrossRef" href="https://www.researchgate.net/publication/331088095_Beyond_Accuracy_What_Documentation_Quality_Means_to_Readers"><img src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/documentation-quality-definitions.png" alt="Documentation Quality Definitions part 1" /></a>

<a class="noCrossRef" href="https://www.researchgate.net/publication/331088095_Beyond_Accuracy_What_Documentation_Quality_Means_to_Readers"><img src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/documentation-quality-definitions.png" alt="Documentation Quality Definitions part 2" /></a>

As you can see, defining information quality is a constant theme in tech comm research, and while the characteristics are somewhat consistent, they aren't described in the same way, and they are all general and abstract.

Strimling is troubled by the lack of a unified approach to documentation quality, by the slipperiness of terms and lack of consistency. He wonders, which of these qualities matter most to users?

Strimling aligns with researchers Richard Wang and Diane Strong (1996) because of the way their research aligns with the "voice of the data customer" and because of the soundness of their framework and research. After describing about 118 information quality dimensions, Wang and Strong boil them down to four main criteria. Yoel explains:

> Based on their categories, Wang and Strong (1996) concluded that high-quality data must be:
> * Intrinsically good
> * Contextually appropriate for the task
> * Clearly represented
> * Accessible to the consumer

You can read the original article by Wang and Strong in *Journal of Management Information Systems* if you have access to it, or [online here](http://mitiq.mit.edu/Documents/Publications/TDQMpub/14_Beyond_Accuracy.pdf). These researchers made a pivot in how they measured data quality &mdash; rather than considering the accuracy of the information on its own, they looked to see what aspects were important to users, and factored that user perspective into the quality assessment. They explain:

> The salient feature of this research study is that quality attributes of data are collected from data consumers instead of being defined theoretically or based on researchers' experience.

In other words, you can't measure data quality (DQ) without analyzing what quality dimensions are important to users. In their research, they settled on the four criteria that Strimling summarized:

> 1. The extent to which data values are in conformance with the actual or true values; (intrinsic DQ)
>
> 2. The extent to which data are applicable (pertinent) to the task of the data user; (contextual DQ)
>
> 3. The extent to which data are presented in an intelligible and clear manner and (representational DQ)
>
> 4. The extent to which data are available or obtainable. (accessibility DQ)

Wang and Strong's emphasis is on data quality, not necessarily documentation. Building on Wang and Strong, Strimling identifies 15 different dimensions to documentation quality and then asks users to rate them by importance. He arrived at the conclusion that these four categories are most important to users: accurate, relevant, easy to understand, accessible. These criteria are based on the level of importance assigned to them by the readers who participated in his study. He proposes that you can measure quality by answering these four questions:

> * Could you find the information you needed in the
document?
> * Was the information in the document accurate?
> * Was the information in the document relevant?
> * Was the information in the document easy to
understand?

(In later research, he is finding that "completeness" might be more important than "relevance.")

Similar to Wang and Strong's user-based DQ framework, these criteria aren't priorities from the writer but rather from users. Strimling says that in the interactions with users, you can assess documentation by asking them these questions.

## The problem with abstract definitions

These four criteria seem like a solid way to evaluate documentation if you have a way to frequently interact with your users. But even if you could regularly survey your users, these abstract categories don't provide details about *how* you might go about making the information more clear, relevant, accurate, and findable.

In other words, these categories are too high-level and general to actually be helpful to writers. For example, what does it mean for something to be clear when you consider different audiences and varying technical backgrounds? Is well-written code clear, without the need for any comments? The same could be said for every abstract category. The categories fail to specify tactics for executing clarity, relevancy, accuracy, and findability. *How* do you make something more clear and relevant?

If you're not a user (but rather a technical writer) trying to assess documentation through these four questions, the questions are also not helpful. They can't be fully answered by a non-user. For example, "Could you find the information you needed in the document?" Only the reader can answer this. "Was the information in the document relevant?" Again, only the reader can answer this, not the writer. "Was the information easy to understand?" Again, only the reader can answer this.

If you're the target audience using the docs and have just finished the task, then yes, you could answer these questions to assess the docs, but this returns us to the problem of relying on surveys to gather information to evaluate documentation. How can we break away from the dependence on user surveys but still develop a method for quality based on the user's perspective?

Fortunately, if we take the starting categories here (accessibility, accuracy, relevance, clarity), and we are confident that these attributes align with user priorities, then we only need to define how these attributes can be implemented in documentation in more specific, concrete, and actionable ways. This is a point Strimling starts to make in [So You Think You Know What Your Readers Want?](https://www.researchgate.net/publication/331088225). He says, "In lieu of feedback, what we need is a proven model of how readers actually define documentation quality (DQ), which we can then use to ensure that what we produce is useful to our audience." In other words, these four criteria can guide you unless you have more specific feedback. However, I am taking this topic to the next level by getting very specific about how to implement each of the more general criteria, without relying on user feedback. The strategy for implementing these data quality attributes instead relies on best practices for content design.

## Other research

Before jumping into the criteria, let's survey the information quality landscape a bit more, as there are a few other sources worth mentioning. First, Pronovix, a company that specializes in creating developer portals, holds regular [Developer Portal Awards](https://pronovix.com/blog/best-developer-portals-2020). As such, they provide general reasons why they rate some developer portals higher than others. For example, in [What is the MVP for a Developer Portal?](https://pronovix.com/blog/what-mvp-developer-portal), they write:

> We compiled a first list of questions that provides users with the information they might need while working with your API product:
>
> * What is this API?
> * How do I get started with this API?
> * What do I need to understand about this API?
> * How do I get X done with this API?
> * Do I know all the details of this API?
> * How do I use your API in Y?
> * Is somebody still working on this API?
> * Where do I go when I have a problem with this API?
> * How do I get access to this API?
> * Can I afford this API?
> * Can I trust this API?

When a user says the documentation is "unclear" or lacks "relevance," it's probably because the documentation does not address some of these questions. This is what I mean by specifying specific checklists for how to make documentation clear without solely relying on survey feedback.

These bullet points are all good questions that one would expect documentation (or a developer portal) to cover. See these articles from Pronovix describing more best practices for documentation and developer portals:

* [What goes into an award winning developer portal?](https://pronovix.com/blog/what-goes-award-winning-developer-portal)
* [How to Improve Developer Adoption and Onboarding](https://pronovix.com/blog/how-improve-developer-adoption-and-onboarding)
* [The Best Developer Portals of 2020](https://pronovix.com/blog/best-developer-portals-2020)

Keep in mind that Pronovix's focus is on developer portals, not standalone API documentation sites (they [explain the difference here](https://pronovix.com/blog/what-difference-between-api-documentation-and-developer-portal)). As such, they place more emphasis on how users interact both inside and outside the documentation, such as getting API keys from an admin portal, checking service status pages, participating in community, and more. Since most companies have multiple documentation sites, often aggregated in a portal, I think the emphasis on developer portals is actually more relevant.

Also, unlike scholarly research, Pronovix looks for best practices and successful patterns, like API explorers for interactivity, the ability to scan and locate reference material, site designs that inspires trust, clear use cases for the API, providing code samples in multiple languages, making onboarding simple and easy, fostering community, and more. Pronovix doesn't try to justify their criteria based on research or from studies that objectively verify and rank these characteristics. Instead, they tend to embrace industry standards and best practices that are generally accepted by practitioners.

Another great resource is [Nordic APIs](https://nordicapis.com/). In [5 Examples of Excellent API Documentation (and Why We Think So)](https://nordicapis.com/5-examples-of-excellent-api-documentation/), they evaluate 5 documentation sites based on these criteria:

* Authentication guide ☐
* Quickstart guide ☐
* Endpoint definitions ☐
* Code snippets ☐
* Example responses ☐

They highlight reasons they like various sites, noting that the lesson with Stripe is "don't overdo it." For Twilio, it's "be beginner-friendly." For Dropbox, it's "cater to unique dev backgrounds." For GitHub, "save developer time wherever you can." And for Twitter, "be flexible with how you present information."

Another Nordic article, [7 Items No API Documentation Can Live Without](https://nordicapis.com/7-items-no-api-documentation-can-live-without/) discusses 7 essential components in API docs:

* 1: An Authentication Scheme
* 2: HTTP Call Type Definitions
* 3: Endpoint Definitions
* 4: URI Structures, Methods, and Parameters
* 5: Human Readable Method Descriptions
* 6: Requests and Examples
* 7: Expected Responses

In my rubric, I've listed each of these items but only briefly and generally. Sites like these provide much more detailed guidance about how to optimize your documentation for each of these components.

## Technical writing handbooks

Another place to find quality checklists and guidance for implementing general characteristics like clarity, relevance, accuracy, etc., is in technical writing handbooks. In [*Developing Quality Technical Information: A Handbook for Writers and Editors*](https://learning.oreilly.com/library/view/developing-quality-technical/9780133119046/app01.html), the authors provide a mountain of detail for best practices. They divide their guidelines into these categories and subcategories:

* Easy to use
  * Task orientation
  * Accuracy
  * Completeness

* Easy to understand
  * Clarity
  * Concreteness
  * Style

* Easy to find
  * Organization
  * Retrievability
  * Visual effectiveness

You can score docs from 1 to 5 according to how well they fulfill each characteristic. The textbook has a lot of examples and detail about how to go about each of these qualities. There's even treatment of code samples. Here's the comprehensive quality checklist provided in the Appendix:

<a class="noCrossRef" href="https://learning.oreilly.com/library/view/developing-quality-technical/9780133119046/app01.html"><img src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/qualityguidelinestextbook2.png" alt="Quality checklist" /></a>

Overall, there are 60 specific characteristics within the various categories. Why not simply adopt this quality checklist? It wouldn't be a bad approach, for sure. And the principles are so widely held that few would object them. But I wanted something even more concrete, actionable, and focused on API documentation and developer portals.

## Standards specifications

Another place to look at information quality would be standards such as the [ASD-STE100](http://www.asd-ste100.org/). The ASD-STE100 standard was developed by the Aerospace and Defense Industries Association (ASD) to encourage simplified technical English (STE). STE consists of a dictionary of about 900 allowed words and a set of 65 writing rules. Together, this controlled language is formalized into a specification called ASD-STE100, which many regulatory industries must follow to ensure clear, consistent content.

In addition to a controlled vocabulary, the writing rules require you to use certain verb choices. For example, you generally keep sentences short, prefer active tense over gerunds, limit sentences to a single topic, avoid passive voice, and more. There are more than 65 writing rules. Usually you implement a language checker such as [HyperText](/2017/01/25/hyperste-simplified-technical-english-asd-ste100/) to check your content for adherence to the rules.

The result of combining a controlled vocabulary with this grammar yields content that is clear and easy to follow, especially for non-native speakers. Here's a sample from their Procedures section:

<a class="noCrossRef" href="http://www.asd-ste100.org/"><img src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/asdprocedures.png" alt="ASD-STE100 procedures" /></a>

Keeping instructional commands to a single command per step seems like a good practice. However, many of the guidelines seem more appropriate to a style guide because they are so granular and language-specific. But depending on your needs, you might adopt more of these principles into your criteria.

Another standard is [ISO/IEC 26514:2008 - Systems and software engineering — Requirements for designers and developers of user documentation](https://www.iso.org/standard/43073.html), which is a standard that "specifies the structure, content, and format for user documentation, and also provides informative guidance for user documentation style." Another is [IEC/IEEE 82079-1 - Preparation Of Information For Use (Instructions For Use) Of Products - Part 1: Principles And General Requirements](https://webstore.ansi.org/Standards/ISO/IECIEEE820792019?gclid=Cj0KCQiA6Or_BRC_ARIsAPzuer-sndUAjuadJ-nhVGSbZeUX-MfS_jFuZj3mSC_-eyEcRiP-LFyTuMMaAmpKEALw_wcB). Both of these standards publications require payment, but sometimes companies subscribe to these standards, and obviously referencing an ISO standard for a practice puts you in indefensible territory about the standard.

A standard developed by SAP and later generalized and adopted by tekom is [Standards and Guidelines for API Documentation](https://www.technical-communication.org/tekom/publications/specialist-books/detail/standards-and-guidelines-for-api-documentation) by Anne Tarnoruder. You can read a summary of the 68-page book in a tcworld article here: [Standardizing API documentation](https://www.tcworld.info/e-magazine/technical-writing/standardizing-api-documentation-949/). Tarnoruder explains, "The S&G cover both auto-generated and manually written API reference documentation, and apply to the major API languages and technologies, such as Java, JavaScript, MS.Net, REST and OData." Tarnoruder emphasizes clear naming guidelines for APIs and says, "Names are the user interface of APIs. Meaningful, clear, and self-explanatory naming is a key factor in API's usability and adoption." Technical writers often work with developers on names to ensure best practices. I covered some of these principles in my [summary of Arnaud Lauret's book, The Design of Web APIs](https://idratherbewriting.com/learnapidoc/evaluating-api-design.html). However, this is an area where API design and documentation seem to blend together. My focus here is more on documenting an API that has already been finalized rather than providing input on best practices for API design.

Tarnoruder provides templates for REST and OData APIs, if you're not already using something like OpenAPI. And she also provides detailed guidelines for documenting APIs such as Java with Javadoc.

For developer guides, Tarnoruder provides guidelines such as including "conceptual, setup, quick start and how-to information" and "does not contain implementation details irrelevant to users." This advice is fairly common. However, she also includes best practices for addressing both a code-first learning style versus a concepts-first learning style:

> Various usability studies show that API documentation users differ in their learning preferences:
>
> Those with a top-bottom approach would first read all the conceptual topics, and only then start trying the API calls.
> Those who prefer a bottom-up approach would delve right into code samples to get a quick hands-on experience with the APIs. ([Standardizing API documentation](https://www.tcworld.info/e-magazine/technical-writing/standardizing-api-documentation-949/))

This is something I covered in [How Developers Use API Documentation: An Observation Study](/learnapidoc/docapiscode_research_on_documenting_code.html#how-developers-use-api-documentation-an-observation-study) and is based on research by Michael Meng, Stephanie Steinhardt, and Andreas Schubert in [How Developers Use API Documentation: An Observation Study](https://sigdoc.acm.org/cdq/how-developers-use-api-documentation-an-observation-study/). The authors describe "opportunistic" behavior (people who learn by immediately pushing buttons and trying things out) versus "systematic" behavior (people who start by carefully reading the manual) as two common patterns of observed usage for developers using documentation. They encourage documentation to accommodate both learning styles.

## Other sources for quality

Many other sources can inform documentation quality. For example, the [Good Docs project](https://thegooddocsproject.dev/) aims to create templates that incorporate best practices. By using the [Overview template](https://github.com/thegooddocsproject/templates/blob/v0.1/api-overview/about-overview.md), you'll automatically address the various questions and topics needed here. The project has templates for an overview, quickstart, reference, discussion, how-to, logging, reference, tutorial, and more.

Another place to look for information quality is the DITA writing specification. This specification enforces best practices (a debatable point) through XML. For example, by following the elements for a concept or task, you'll include a [`shortdesc`](https://docs.oasis-open.org/dita/v1.2/cd03/spec/langref/shortdesc.html) element that provides a high-level summary of the topic. This information can be re-used elsewhere.

Additionally, DITA has various topic types (task, concept, reference, troubleshooting, glossary) that provide elements to guide you more successfully in these information areas. The whole idea of information typing is that different kinds of information follows specific patterns that one should follow. DITA builds on information typing theories that share commonality with Information mapping and other approaches.

In sum, my intent is not to exhaustively survey docs on information quality. As Strimling's earlier research pointed out, most people generally agree on the high-level categories. I want to instead provide specifics on implementation.

## An extremely detailed rubric

Now that I've set some of the background and context for this topic, let's move into a more practical realm. As I indicated earlier, my goal is to create a practical guide for measuring quality. Instead of looking at docs against a list of general, abstract criteria, I propose that we create enumerate a series of characteristics that, if fulfilled, should lead to all the more high-level categories of the rubric. Each of these characteristics must be specific, actionable, and unambiguous in how it would be implemented in your docs.

To get a better sense of what I'm driving at, let's jump right into these details and continue the discussion afterwards. Here are many ways that the more general attributes of findability, accuracy, relevance, and clarity, completeness, succinctness, etc., might be implemented in developer documentation. The criteria are in no particular order or weighting (more on that later). Also, the list shouldn't be seen as definitive or as some foolproof recipe for perfect documentation. Also, some points might apply more than others. Overall, these are criteria that will likely lead to a better experience with developer docs.

<style>
li.checkboxListType {
  list-style-type: none;
  margin-left: 25px;
  text-indent: -28px;
  margin-bottom: 20px;
  line-height: 24px;
}
input[type=checkbox] {
  margin-right: 10px;
}
</style>

{% assign cb = "<li class='checkboxListType' markdown='span'><input type='checkbox'>" %}
{% assign cb-end = "</li>" %}

<div style="background-color: #F0EFF8; padding: 15px; margin-top: 30px; margin-bottom: 30px;" markdown="block">
<div style="margin-top: 20px; margin-bottom: 20px; font-size:24px; text-align: center;">Developer documentation quality checklist</div>

### Findability

<ul class="checkLists">

{{cb}} The content is indexed in a general search engine and findable when you create searches with the product name and some key tasks. In some cases, there are entry points into the documentation on popular sites where users look for answers (for example, question-and-answer sites like Stack Overflow, knowledge bases, or other resources apart from a standard Internet search){{cb-end}}

{{cb}} The doc site has a site-specific search that lets users search within the documentation site itself. {{cb-end}}

{{cb}} Where possible, links are provided to connect users from the task domain to the documentation domain. For example, on a user interface, a help button might appear next to a confusing section that helps the reader locate the documentation for that section. Or in error messages, a link or code might help users get more troubleshooting information. {{cb-end}}

{{cb}} Each topic consolidates all necessary information about the topic in a standalone, modular way (rather than fragmenting the information into many small topics that require the user to bounce around, losing context). {{cb-end}}

{{cb}} The content doesn't have an endless FAQ with information that should have been integrated into more logical places in the document. {{cb-end}}

{{cb}} Topics that are highly related have a related links section on the page (or cross references in appropriate sections) linking the sections together. {{cb-end}}

{{cb}} If content has multiple versions, the versions are called out visibly for the topic and a selector or link allows users to navigate to the other versions. {{cb-end}}

{{cb}} When new features are released or significant updates are made to the documentation, these changes are called out in release notes. Changes aren't simply made on the sly without letting users know. {{cb-end}}

{{cb}} Content is organized primarily by task and from a user perspective rather than solely by doc type (that is, the content follows a task-based or user-based  organization scheme rather than a product-based organization). The exception is that reference content often consolidated on its own in an auto-generated output. {{cb-end}}

{{cb}} Reference material that has a large number of endpoints, functions, commands, or classes provides mechanisms to expand, collapse, sort, or filter the content. {{cb-end}}

{{cb}} Related doc sites are usually listed somewhere (at the bottom of the sidebar, or in top navigation) to help users navigate similar but separate docs {{cb-end}}

{{cb}} If you have lots of documentation sets relevant to users, the documentation is organized in a developer portal. The information hierarchy in the developer portal organizes content within a larger context or story, even if it's just a list of links under various categories. This organizational hub provides a space for developers to find, explore, and consume content from multiple doc sets in a way that tells the story of your company's products. {{cb-end}}

{{cb}} The most popular topics are highlighted in one of the introductory sections (such as the homepage), allowing users to easily find the most commonly used topics. {{cb-end}}
</ul>

### Accuracy

<ul class="checkLists">

{{cb}} Content has been reviewed by a subject matter expert within the past year. Ideally, each topic should include metadata such as the last-reviewed timestamp, last author, and the group that owns the content. {{cb-end}}

{{cb}} The documentation provides a visible timestamp of the last time it was edited so that users can gauge how current the documentation is. {{cb-end}}

{{cb}} If the content relies on third-party tools or services, the sections detailing the third-party tools or services are checked yearly to ensure the third-party tools haven't evolved or changed. {{cb-end}}

{{cb}} The steps in the tasks accurately lead to the results promised by the task, without missing any details. For example, if the instructions say to click a button name, the button is named the same way in the interface. If the instructions say to use a class, the class is spelled as it appears in the code library, etc. {{cb-end}}

{{cb}} Information isn't repeated in confusing, redundant, or inconsistent ways. For example, the documentation doesn't explain how to do a task one way in Topic A but then a different way in Topic B. If content is re-used, the re-use is usually single sourced to reduce inconsistency. {{cb-end}}

{{cb}} Screenshots and other visuals are up to date with the state of the interface (if there is one). {{cb-end}}

{{cb}} Links point to correct pages or are appropriately handled by redirects to equivalent pages. {{cb-end}}

{{cb}} Features that are no longer supported (or which have been deprecated) are clearly noted as such in the documentation. Preferably, if a feature has been deprecated, a migration path to an alternative solution is provided. {{cb-end}}

{{cb}} Code samples that can be copy and pasted actually work. {{cb-end}}

{{cb}} Code in sample apps matches the code described in the documentation. The sample app hasn't evolved in ways that no longer match the documentation. {{cb-end}}

</ul>

### Relevance

<ul class="checkLists">

{{cb}} The documentation doesn't just provide reference information (e.g., auto-generated API documentation) but also explains how to use the API with tutorials guiding users through common use cases and journeys. The content should address the *most common* use cases intended for the product. (Fringe use cases don't need to be documented because too much information can dilute the emphasis on the core journeys.) {{cb-end}}

{{cb}} Documentation is available at the same time the feature is released and made available to users, not after the fact. Versions in the release notes correspond with the actual version of the product. {{cb-end}}

{{cb}} Code samples are available in the user's target language. This might mean providing multiple code samples. {{cb-end}}

{{cb}} Options for support are provided, even if the support merely involves posting to a peer-monitored forum. {{cb-end}}

{{cb}} The code in the doc site offers interactivity that allows users to interact with the functions, API calls, or other calls, often using their custom data. Typically, with REST APIs, an API explorer allows users to try out requests using their own data. Seeing responses with your own data can make the API seem more relevant. {{cb-end}}

{{cb}} If the product has a code repository similar to features on GitHub, this repository is actively monitored when users log issues or submit pull requests. Users aren't simply ignored. {{cb-end}}

{{cb}} A feedback option is included in the docs so that the writers can stay attuned to what information readers might want to communicate to them. This helps users feel more relevant and listened to. {{cb-end}}

</ul>

### Clarity

<ul class="checkLists">

{{cb}} The [overview](docapis_doc_overview.html) explains the big picture and describes the problem that the tool or service addresses. {{cb-end}}

{{cb}} The [overview](docapis_doc_overview.html) provides a high-level description of the main uses cases or business objectives of the product. {{cb-end}}

{{cb}} The [overview](docapis_doc_overview.html) has diagram of the main components and how they interact. {{cb-end}}

{{cb}} For larger systems that might have multiple subsystems (e.g., groups of APIs for different scenarios), these subsystems have their own landing pages that resemble the higher-level overview (with use cases, diagrams, getting started links) but scoped to that specific subsystem. {{cb-end}}

{{cb}} Details about how to get access, permissions, and authorization to use the API are provided. The overview usually links out to a getting started topic that makes it easy for the user to sign up, register, get API keys or permissions, and start using the API. {{cb-end}}

{{cb}} The documentation provides opportunities for experiential/opportunistic users to start learning immediately through code and trial/error, and for more systematic users to learn by reading concepts first. {{cb-end}}

{{cb}} A sandbox environment is available for users to try out the tool on their own and get a better understanding of how it works. {{cb-end}}

{{cb}} If there are different roles and permission levels that correspond to varying capabilities, these roles are noted in all places they apply, such as within the individual API reference. For example, if only admin roles can use a certain API, this is noted in the API reference and in any places that use the API. {{cb-end}}

{{cb}} If the product has a code repository, the repository contains a Readme file that provides information similar to the overview, including information on how to contribute if applicable. (The readme might simply link to the documentation overview but also include unique sections such as how to contribute in the repo.) {{cb-end}}

{{cb}} Each task has a "Prerequisites" section that explains knowledge requirements, tool requirements, essential concepts, etc., necessary for completing the task. {{cb-end}}

{{cb}} Tasks are articulated through a series of specific, usually numbered steps or sections that reduce the complexity of the task. More complex tasks might require more granular and numerous steps or sections so as to reduce the complexity. (This is the primary way that technical writers simplify complexity.) {{cb-end}}

{{cb}} Specific steps for completing tasks are described in detail rather than glossed over in general ways &mdash; unless the task is something the audience is already familiar with. Overall, the documentation strikes a balance between providing enough detail for users to get the job done but not including too much detail that the reader is inundated with extraneous information. {{cb-end}}

{{cb}} Larger tasks that span multiple topics have a [workflow map](/simplifying-complexity/macro-micro.html) (or similar mechanism) that connects the topics together. {{cb-end}}

{{cb}} In places that are particularly confusing, appropriate visuals or additional examples have been added to reduce confusion. {{cb-end}}

{{cb}} If there are multiple paths to a solution, the documentation describes the simplest path (though other possibilities might be briefly mentioned). {{cb-end}}

{{cb}} Users can follow the documentation by themselves without relying on peer or customer support. A large number of support cases or forum threads containing questions that could have been answered in the documentation would indicate that users aren't self-sufficient through the docs. {{cb-end}}

{{cb}} A [getting-started tutorial](docapis_doc_getting_started_section.html) is provided for users to get started in an end-to-end way with the product, producing a sample output that builds their confidence. {{cb-end}}

{{cb}} [Code samples](docapis_codesamples_bestpractices.html) showing sample ways to use the API (or similar tools) are provided. In more robust scenarios, a [sample app](docapis_sample_apps.html) might serve as a reference implementation for users. In cases where a sample app complements the documentation, the documentation should refer to different aspects of the reference implementation.) {{cb-end}}

{{cb}} [Code samples](docapis_codesamples_bestpractices.html) are appropriately commented, either with inline comments, comments that preface or follow the sample, or both. Long code samples with no explanation aren't just dropped in. {{cb-end}}

{{cb}} The documentation's technical level is appropriate to the *target audience* but might not serve every possible audience (e.g., total newbies to a programming language might struggle with documentation intended for developers already experienced in that language). Usually, general concepts in a programming language that you assume the audience knows are not explained in the documentation. Instead, your company's product, configuration, and usage are covered in the context of the programming language. One exception is when the implementation requires a non-standard process or workflow that merits some explanation. {{cb-end}}

{{cb}} A one-pager [quick reference](docapis_doc_quick_reference.html) is available for the documentation so that users can get up and running quickly. The one-pager also allows users to quickly get a sense of the essential information and tasks for the tool or service. {{cb-end}}

</ul>

### Completeness

<ul class="checkLists">

{{cb}} For REST API documentation, the [OpenAPI standard](pubapis_openapi_intro.html) is used to describe the API. For [library-based APIs](nativelibraryapis_overview.html) like Java, the appropriate conventions for documentation in that language are followed (such as [Javadoc tags](nativelibraryapis_javadoc_tags.html)).{{cb-end}}

{{cb}} Reference material such as APIs (if applicable) follow a [common structure within each topic](docapis_api_reference_tutorial_overview.html), mostly following a request-response type structure. Typical sections include descriptions, parameters, sample requests or usage, and sample responses. {{cb-end}}

{{cb}} [Error messages](docapis_doc_status_codes.html) that users can encounter are documented and discoverable through search. {{cb-end}}

{{cb}} [Parameter documentation](docapis_doc_parameters.html) typically includes a description, data type, min/max values, sample values, and optional/required usage. {{cb-end}}

{{cb}} If there are pitfalls or other traps, gaps, and gotchas to avoid, these are noted in the documentation rather than hidden from the user. A section called ["Known Limitations"](/2010/12/16/known-limitations/) often contains this information. The documentation doesn't lie or mislead the user but rather is [transparent, honest, and helpful](/2017/07/13/transparency-in-documentation/) even if it means exposing the product's warts and revealing problems users will like encounter. {{cb-end}}

{{cb}} If there are [limitations and thresholds](/learnapidoc/docapis_rate_limiting_and_thresholds.html) (e.g., max number of API calls, max file sizes, max string lengths, max/min parameter values), these limitations are called out in the docs. {{cb-end}}

{{cb}} If a task is only available in certain contexts (locales, languages,  platforms, roles, versions), that information is noted clearly in the topic. For example, a tool that is globally available but with feature limitations for some areas might have a label on certain topics that say "US only," or "Enterprise Version Only," or it might have tabs that split the content into "Mac \| Windows \| Linux" steps. {{cb-end}}

{{cb}} The documentation has a troubleshooting section (either standalone or included within the section/topic it relates to) that provides information on how to solve common problems. The troubleshooting information indicates where things might go wrong and how to fix them. In other words, the documentation doesn't just describe the happy path. {{cb-end}}

</ul>

### Readability

<ul class="checkLists">

{{cb}} The sidebar navigation lets users take in a sense of the whole while also allowing users to expand more details as desired. The sidebar isn't a massive list of seemingly endless scrolling and expansion + expansion + expansion but divides up doc sets into logical groups, like books. For systems with large numbers of topics, progressive disclose techniques might be implemented across primary, secondary, and tertiary levels of information. {{cb-end}}

{{cb}} As the user navigates each topic, the sidebar navigation makes it clear where the user is in the navigation (e.g., the topic highlights clearly and the navigation sticks open at that level). Breadcrumbs might also help establish site context. {{cb-end}}

{{cb}} When a user click topics in the navigation, the UI doesn't shift context in jarring ways, such as taking the user to another doc set or changing stable navigation areas like the sidebar and header (which are usually consistent for every page). This jarring navigation often happens when sidebar entries point to topics in other doc sites. If this is the case, the external links have an icon indicating the link takes them to another site. {{cb-end}}

{{cb}} Navigation mechanisms work consistently across all docs in the developer portal. For example, in one set of docs, if top-level folders expand to show child items rather than opening to their own page, the same behavior is found in others. {{cb-end}}

{{cb}} Common topics have similar names across doc sets in the developer portal. For example, the Overview, Getting Started, Troubleshooting, Glossary, Release Notes, and Reference are named in consistent ways that help users understand how to navigate the site. One doc set shouldn't call a topic "Latest updates" and "First steps" while another uses "What's new" and "Quickstart." {{cb-end}}

{{cb}} Sentences are somewhat short, paragraphs are relatively small, and subheadings are frequent. A readability score will place the content at the high-school level, not college. {{cb-end}}

{{cb}} Subheadings follow a parallel structure so they can be more easily scanned and read. The subheadings are descriptive enough to allow users to get a gist of the page by merely reading the subheadings. {{cb-end}}

{{cb}} Topics usually have a [short summary below the title](/2018/09/15/pages-at-a-glance-feature/#enforcing-best-practices-with-structure) that encapsulates the main purpose of the topic. This helps users get a sense of the topic at a glance. {{cb-end}}

{{cb}} Unfamiliar words and jargon are defined in a [glossary](docapis_glossary_section.html). At times, the glossary terms are linked to their glossary definitions. {{cb-end}}

{{cb}} The language uses active voice (where warranted) with clear subjects and verbs positioned closely together. {{cb-end}}

{{cb}} Sentences are grammatically correct and read well, without distracting the user or calling attention to the language. {{cb-end}}

{{cb}} Individual sentences have one main idea. Paragraphs have one main point. {{cb-end}}

{{cb}} The formatting in code samples follows standard white spacing, line breaks, and other syntax for the language. Code syntax highlighting helps increase readability. {{cb-end}}

{{cb}} In code samples, placeholder text that needs to be customized is clearly indicated to the user. It's not confusing what is code and what needs to be changed, like `APIKEY`. {{cb-end}}

{{cb}} The content can be read on a mobile device in a usable way. For example, the responsive view allows users to navigate the sidebar links and view code samples. {{cb-end}}

</ul>
</div>

Did I miss anything? I probably missed 100 more details here. Feel free to let me know (either in the comments or survey) what could/should be added, especially if it's a major omission. But there's also something to be said for a practical list of key points (there are 70+ check boxes here!). The more criteria you add, the more laborious it becomes to evaluate docs. The most popular style guides (e.g., Strunk and White) are those that cover the main points you need rather than providing an exhaustive list, especially if many guidelines are already followed.

## Analysis and quantitative metrics

It's hard to imagine that documentation that checks all of these boxes wouldn't also score highly with user satisfaction surveys. Can you honestly see any documentation that legitimately satisfies all of this criteria as falling short with users? And yet, to achieve the level of information quality, we didn't have to rely on constant user surveys to gather feedback. By identifying best practices for content design (specifically for API/developer documentation), we're able to increase the documentation quality in more self-sufficient, self-directed ways.

One note: Sometimes poor API design will make even good docs problematic. If the API has inconsistent naming, incomplete parameters, doesn't map to user journeys, and is cumbersome to use, then documentation also becomes more cumbersome to follow and implement. Good docs can't fix bad API design, though they can make the user experience salvageable. If you have to explain string theory and Lagrange multipliers in your docs, give yourself extra points even if clarity is still debatable.

## Moving towards quantification

Now that we have a set of criteria, we can start to quantitatively measure documentation. To allow for some flexibility with each criteria, you might give documentation a score of 0 to 5 for each item. For example, if the documentation partially implements one of the criteria (e.g., some great code examples for one topic but missing in another), this is a way to give some credit without giving full credit.

It doesn't matter how many criteria you use. Some points will be more applicable than others, and by no means am I suggesting a universal list of golden attributes that serve all types of information! Also remember, I'm specifically focusing on developer docs. You might decide to add your own criteria, remove some of my points, or make other modifications.

Based on how many criteria you have and how you decide to score things, you'll have a total number of possible points. You can then calculate the percentage accordingly. If you add up the score and find that the documentation scores 40/70, then this is 57%, or an F. By assigning documentation a grade that aligns with school grades, it provides a familiar assessment of the documentation quality.

Taking the metrics one step further, you could give your documentation a grade point average by calculating the average of all the individual grades. For example, suppose you have 10 sets of documentation for 10 different products. The cumulative score would simply be the average. This could give you your documentation GPA. Quantitative metrics can be more fun to measure. One key point here is that we've moved from qualitative to quantitative using a set of consistent criteria for evaluation.

Granted, there are some assumptions here. Not all categories are equally important. This was one of the main goals of Strimling's research &mdash; to identify what matters most to users, not to writers. Users can probably overcome issues with readability as long as the content is accurate. Irrelevant content (e.g., the wrong user journeys) might be useless, no matter how well they are described. Code samples in the wrong language might not be a dealbreaker if they are well commented, etc.

In my weighting, everything has the same potential number of points without regards to the criteria's importance. I have omitted different weighting for each criteria or category because it's too difficult and varies too much by product/domain/audience. But you could implement a more sophisticated weighting system as long as the weighting leads to the same total. For example, for each criteria that falls under the most valued user categories (Findability, Accuracy, Relevance, and Clarity), you might double these points. Just be consistent.

Personally, I think it's impossible to impose an objective weight across each criteria. While a readability category such as "Sentences are grammatically correct and read well, without distracting the user or calling attention to the language" might not seem important, if the content is written by a non-native speaker and is extremely hard to follow or understand, this can be just as jarring as a non-functioning code example. There are degrees to which each of these criteria can be so poorly implemented or omitted that it takes on a larger weighting. Passive voice might not be problematic in places, but convert the entire document into passive voice and see how usable it is. Or write a beautiful flowing document with amazing clarity, yet get the code sample wrong, and the user experience plummets.

## Measuring progress

As you work on improving documentation, you could quantitatively say that you improved the documentation from a score of 42% to 75%, or something similar. For this quantitative progress to make sense, you need to use a consistent set of criteria applied in a similar way across docs.

Also, keep in mind that adding user satisfaction surveys to corroborate the improvements would be a good idea. But even without the corroboration, at least this rubric provides a more action-oriented way of addressing more fuzzy issues that users might report in a survey (e.g., docs are incomplete, confusing), and it provides a quantitative metric for measurement. If you're an editor, this list lets you audit your documentation to assess quality.

## Objections to "Tom's criteria"

My goal here was to find a way to assess documentation quality without relying solely on surveys, and to pin down the criteria for developer docs to a list of actionable, easy-to-understand criteria. I recognize that my list has no official research backing or data to support it &mdash; instead, these best practices come from my experience in the industry and from best practices that I have observed within the realm of developer documentation.

This is likely the problem with my approach: who's to say that documentation needs each of these criteria to succeed? It's possible that documentation might still be findable, accurate, relevant, and clear without many of these more concrete components, which would seemingly invalidate the approach here. Some will object these criteria are just random requirements from Tom's head without any grounding in reality. I don't have any user-based research to say that docs should be this way, that they should have an overview, that reference material should follow a consistent structure, that tasks should be detailed in steps, or that error messages should be documented, etc. As such, critics could dismiss a documentation's "score" as being meaningless, relying only on user feedback for their evaluation of docs.

If this is the feeling regarding reported metrics, remember that users surveys could both complement and confirm the approach here. User surveys specifically for docs that score highly should also rate higher in satisfaction surveys than surveys for docs that score more poorly. But again, to establish a kind of truth through surveys relies on a host of factors (objective, unbiased, unambiguous survey questions from a large sample of a representative audience across domains) that is likely difficult to pull off on a regular basis.

Overall, I am confident that few would object to most of the criteria here. Most of the details here would be agreed upon by both readers and writers with enough common ground as to be a practical guide for improving documentation quality. The criteria here are a starting point that can be refined and improved, checked against industry standards, against docs that are loved by users, against constant feedback, and other experiences.

## Survey

Please respond to a few questions so that I can understand your thoughts on this approach and whether I am headed in the right direction. There are 12 questions. These surveys help me leverage your experience and insight to check my approach and potentially course correct. You can view the [ongoing results here](https://www.questionpro.com/t/PHpuiZkbgw).

<script>
EMBED_PARAMS = {};
EMBED_PARAMS.surveyID =8043019;
EMBED_PARAMS.domain ="//www.questionpro.com";
EMBED_PARAMS.src ="//www.questionpro.com/a/TakeSurvey?tt=rME%2B18/h7CE%3D";
EMBED_PARAMS.width ="100%";
EMBED_PARAMS.height = "1200px";
EMBED_PARAMS.border = "hidden";
</script>
<div id="div_8043019"></div>
<script src="//www.questionpro.com/javascript/embedsurvey.js?version=1"></script>

*Special thanks to Yoel Strimling for his input on this article.*