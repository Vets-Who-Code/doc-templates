# {{ project_name }} Design Doc

## About this doc
Metadata about this document. Describe the scope and current status.

This doc describes the technical approach, milestones, and work planned for the [{{ project_name }}]({{ product_requirements_doc_link }}) linked to the Product Requirements Doc.

---

### Sign off deadline
**Date:** {{ sign_off_deadline }}

### Status
**{{ status }}**

### Author(s)
{% for author in authors %}- {{ author }}
{% endfor %}

### Sign offs
{% for sign_off in sign_offs %}- *{{ sign_off }}*
{% endfor %}

_Add your name here to sign off._

---

## Context
A sentence or two on the **what**—what is being built.

Then include the **why**—metrics we intend for. [Link to Product Requirements Doc]({{ product_requirements_doc_link }}) for details.

---

## Non-goals
What is out of scope for this project that we don’t want to focus on?

{% for item in non_goals %}- {{ item }}
{% endfor %}

---

## Terminology
Define any new terms that are used in the document.

---

## High-Level Approach
Explain the technical approach in a few sentences so the reader understands the system flow.

---

## Alternatives Considered
Bullet points of alternative approaches considered and why they were not chosen.

{% for alternative in alternatives %}- **{{ alternative }}**
{% endfor %}

---

## Detailed Design
- APIs
- DB tables modified
- Data models changed
- Any diagrams that help the reader understand at a high level

---

## Risks
What can go wrong with the proposed approach? How are we mitigating that?

{% for risk in risks %}- **{{ risk }}**
{% endfor %}

---

## Test Plan
How will this approach be tested? 

- Browser testing? 
- Manual testing? 
- Any tricky parts to test? 

Adding information here also makes it easier to justify longer timelines.

---

## Milestones
How will the work be divided into chunks of progress?

_Focus on user milestones rather than technical ones. Example: having a minimal working feature behind a feature flag initially._

I usually add **1 week per 2 weeks of expected feature work**.

{% for milestone in milestones %}- **{{ milestone.name }}:** {{ milestone.date }}
{% endfor %}

**Rough ETA of project finish date:** {{ project_finish_eta }}

**Project retro:** {{ project_retro }}

---

## Rollout Plan _(Optional)_
How will you gradually ramp up usage of the feature for safety?

{% for step in rollout_plan %}- {{ step }}
{% endfor %}

---

## Open Questions
Anything still being figured out that could use additional eyes or thoughts.

---

## Parties Involved
Who is working on this? Are there any external teams that need to sign off?

{% for party in parties_involved %}- **{{ party.role }}:** {{ party.name }}
{% endfor %}

---

## Appendix
Add any detailed figures you didn’t want to inline for space.
