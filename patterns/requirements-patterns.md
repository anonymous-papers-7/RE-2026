# ETHEX Explainability Requirement Patterns

This document contains all 16 explainability requirement patterns derived by crossing **4 stakeholder roles** with **4 ethical scenario clusters**.Each pattern has a context (stakeholder role and scenario type), a parameterized requirement template, and a grounded example traced to a coded participant utterance.

Patterns 2, 7, and 13 correspond to the three exemplars presented in the paper. The remaining 13 are derived from the same empirical data using the pattern index (Table: *Pattern Index: Top-3 Priority Categories by Role and Scenario Cluster*).

---

## Pattern Index

| | **Triage** | **Epistemic** | **Values** | **Boundary** |
|---|---|---|---|---|
| **AutSys Expert** | [P1](#pattern-1) CSA, DR, ET | [P2](#pattern-2) ET, DR, OC | [P3](#pattern-3) VGJ, GAA, DR | [P4](#pattern-4) GAA, ET, HMDB |
| **Ethics Specialist** | [P5](#pattern-5) CSA, DR, VGJ | [P6](#pattern-6) DR, ET, HMDB | [P7](#pattern-7) VGJ, GAA, DR | [P8](#pattern-8) GAA, ET, DR |
| **Oper. Practitioner** | [P9](#pattern-9) CSA, DR, ET | [P10](#pattern-10) ET, DR, CSA | [P11](#pattern-11) VGJ, ET, GAA | [P12](#pattern-12) DR, VGJ, ET |
| **Layperson** | [P13](#pattern-13) CSA, DR, ET | [P14](#pattern-14) CSA, ET, DR | [P15](#pattern-15) VGJ, GAA, CSA | [P16](#pattern-16) GAA, DR, ET |

**Category key:** DR = Decision Rationale, ET = Epistemic Transparency, CSA = Contextual Situational Awareness, VGJ = Value-Grounded Justification, GAA = Governance and Authority Alignment, OC = Operational Communication, HMDB = Human-Machine Decision Boundary.

**Scenario clusters:** Triage = resource scarcity decisions (Scenarios A, E, H). Epistemic = acting on uncertain/incomplete information (Scenarios B, F, J). Values = rights/autonomy conflicts (Scenarios D, G). Boundary = authority and accountability (Scenarios C, I).

---

## Pattern 1

**Technical Risk-Benefit Assessment**

| Field | Content |
|---|---|
| **Role** | Autonomous Systems Expert |
| **Scenario Cluster** | Triage (resource scarcity) |
| **Priority Categories** | CSA, DR, ET |

**Requirement Template:**

> When `<system>` must prioritize `<competing demands>` under `<resource scarcity>`, the explanation shall (a) present current `<environmental conditions>`, `<demographic assessments>`, and available `<resource capacity>`, (b) disclose the risk-benefit comparison between `<alternatives>`, and (c) state the confidence level and reliability of input data, enabling the technical stakeholder to verify the triage logic.

**Grounded Example** (P3, FG-1, Scenario A):

> *"I would agree that the struggling person, person B, needs the flotation device more and that'd be prioritized by the drone. I think that if person A, the steady person, is treading water steadily already, it's likely that...they can probably continue to do so until the Coast Guard comes. However, if we're seeing B already bobbing up and down, going underwater, that would even get to me that 25 minutes seems like a long time for them to continue to survive."*

---

## Pattern 2

**Operational Transparency under Uncertainty** *(Paper exemplar)*

| Field | Content |
|---|---|
| **Role** | Autonomous Systems Expert |
| **Scenario Cluster** | Epistemic (uncertain/incomplete information) |
| **Priority Categories** | ET, DR, OC |

**Requirement Template:**

> When `<system>` operates under `<uncertainty condition>`, the explanation shall (a) characterize data confidence and sensor reliability, (b) disclose the reasoning behind `<decision>`, and (c) continuously relay raw observations and analysis progress to `<human operators>`, enabling independent assessment.

**Grounded Example** (P5, FG-2, Scenario F):

> *"It should concisely give as much relevant information as possible and continuously update...the risk of secondary structural collapse...should be transmitted to the rescue team."*

---

## Pattern 3

**Principled Override Justification**

| Field | Content |
|---|---|
| **Role** | Autonomous Systems Expert |
| **Scenario Cluster** | Values (rights/autonomy conflicts) |
| **Priority Categories** | VGJ, GAA, DR |

**Requirement Template:**

> When `<system>` must override `<rule or restriction>` to address `<value conflict>`, the explanation shall (a) identify the value trade-off and state why `<ethical obligation>` outweighs `<compliance constraint>`, (b) reference the `<legal or governance framework>` governing the action, and (c) disclose the reasoning process including alternatives considered, enabling the technical stakeholder to assess whether the override was warranted.

**Grounded Example** (P5, FG-2, Scenario G):

> *"I would, for the most part, say that the drone should override the geofence and provide support if that person's life is truly in danger. The one caveat I did kind of think about is...potentially the risk of that...a potential idea for that is like waiting a couple of minutes to see if there is any response from within the [restricted area] and then basically giving them a set time to react and take care of it themselves, and if not, then the drone overrides."*

---

## Pattern 4

**Autonomous Authority Delimitation**

| Field | Content |
|---|---|
| **Role** | Autonomous Systems Expert |
| **Scenario Cluster** | Boundary (authority and accountability) |
| **Priority Categories** | GAA, ET, HMDB |

**Requirement Template:**

> When `<system>` acts on `<directive>` with `<ambiguous authority source>`, the explanation shall (a) state the governance chain and source credibility of the `<directive>`, (b) disclose the confidence and completeness of available information, and (c) identify which aspects of the decision were made autonomously versus delegated to `<human authority>`, enabling the technical stakeholder to assess whether the system exceeded its decision authority.

**Grounded Example** (P14, FG-4, Scenario C):

> *"If it was, based off of who the command is coming from...If there's somehow emergency personnel aware of this family in immediate need and they're the ones telling the drone to stop, then that should definitely, that command should definitely be followed...If it's just the algorithm or the drone itself making the decision, I wouldn't want it to divert and ignore what had been originally been told because like there are sensing problems."*

---

## Pattern 5

**Ethical Triage Reasoning**

| Field | Content |
|---|---|
| **Role** | Ethics Specialist |
| **Scenario Cluster** | Triage (resource scarcity) |
| **Priority Categories** | CSA, DR, VGJ |

**Requirement Template:**

> When `<system>` allocates `<scarce resource>` among `<competing beneficiaries>`, the explanation shall (a) present the situational context including `<demographic factors>`, `<environmental conditions>`, and `<resource constraints>`, (b) disclose the reasoning process including alternatives evaluated, and (c) identify the ethical principle (e.g., vulnerability-based prioritization, maximizing lives) that guided the allocation, enabling the stakeholder to evaluate the moral adequacy of the triage decision.

**Grounded Example** (P2, FG-1, Scenario A):

> *"The drone should primarily consider who's more likely to die based on their swimming abilities, but also on how long it would take for an external source of help, maybe another drone or a boat of some sort to come and get them. Because I think it would be a clear choice to give the flotation device to person B if, say, B could survive with it until a boat comes and the person A could tread water until the boat comes. Then in that scenario, you could save both, which would be the optimal outcome."*

---

## Pattern 6

**Deliberative Uncertainty Resolution**

| Field | Content |
|---|---|
| **Role** | Ethics Specialist |
| **Scenario Cluster** | Epistemic (uncertain/incomplete information) |
| **Priority Categories** | DR, ET, HMDB |

**Requirement Template:**

> When `<system>` makes `<decision>` under `<epistemic uncertainty>`, the explanation shall (a) disclose the reasoning process and how competing risks were balanced, (b) characterize the uncertainty including data confidence and completeness, and (c) identify whether the decision was made autonomously or should be escalated to `<human authority>`, enabling the stakeholder to evaluate the appropriateness of acting under uncertainty.

**Grounded Example** (P13, FG-4, Scenario F):

> *"I'd like the drone to take into account the time to analysis completion...I think that's definitely an important point. The experience of the team. I think it's also important, as difficult as it is, to compare a drone's capabilities to a team's capabilities...The severity of the injury, possible injury of the survivor...something I'd like to have included in the decision."*

---

## Pattern 7

**Normative Compliance Justification** *(Paper exemplar)*

| Field | Content |
|---|---|
| **Role** | Ethics Specialist |
| **Scenario Cluster** | Values (rights/autonomy conflicts) |
| **Priority Categories** | VGJ, GAA, DR |

**Requirement Template:**

> When `<system>` makes `<decision>` involving `<value conflict>`, the explanation shall (a) reference the applicable `<legal or ethical framework>`, (b) state the value trade-off rationale, and (c) disclose what alternatives were considered, enabling the stakeholder to evaluate normative compliance.

**Grounded Example** (P2, FG-1, Scenario D):

> *"I would want to be more familiar with the legal aspect of this question in particular, because I think this is pretty similar to, say, like, medical officials deploying an ambulance against someone's will. So whether there's legality on obligation to help or to not help if someone refuses...you should respect someone who's in the right state of mind, respect their wishes."*

---

## Pattern 8

**Institutional Accountability Disclosure**

| Field | Content |
|---|---|
| **Role** | Ethics Specialist |
| **Scenario Cluster** | Boundary (authority and accountability) |
| **Priority Categories** | GAA, ET, DR |

**Requirement Template:**

> When `<system>` acts within `<institutional context>` involving `<authority conflict or post-incident review>`, the explanation shall (a) reference the applicable `<institutional policies and legal frameworks>`, (b) disclose the information available and its reliability at the time of the decision, and (c) explain the reasoning process including alternatives considered, enabling the stakeholder to evaluate institutional compliance and accountability.

**Grounded Example** (P10, FG-3, Scenario C):

> *"My thoughts are very reluctantly that it should follow the coordinator's directive insofar as to assure regularity of drone behavior over time. It can't just be responding to ad hoc requests without some articulable measure of the urgency that they're responding to...if you don't have more intel on that, because of course, in a situation like this, everyone would be like, I'm in [dire need], and very reasonably so."*

---

## Pattern 9

**Tactical Prioritization Briefing**

| Field | Content |
|---|---|
| **Role** | Operational Practitioner |
| **Scenario Cluster** | Triage (resource scarcity) |
| **Priority Categories** | CSA, DR, ET |

**Requirement Template:**

> When `<system>` must prioritize `<competing operational demands>` under `<resource scarcity>`, the explanation shall (a) present the operational context including `<environmental conditions>`, `<personnel capacity>`, and `<time constraints>`, (b) disclose the comparative risk assessment between `<alternatives>`, and (c) state the reliability and confidence of sensor data, enabling the operational practitioner to integrate the assessment into tactical decision-making.

**Grounded Example** (P8, FG-2, Scenario A):

> *"I would absolutely, positively want to keep that drone on station to provide locational data because it is super, super easy to lose people in the ocean...The better swimmer has greater ability to stay afloat longer. 25 minutes is a long time, especially if it's rough, cold ocean water."*

---

## Pattern 10

**Intelligence Quality Assessment**

| Field | Content |
|---|---|
| **Role** | Operational Practitioner |
| **Scenario Cluster** | Epistemic (uncertain/incomplete information) |
| **Priority Categories** | ET, DR, CSA |

**Requirement Template:**

> When `<system>` provides `<assessment or recommendation>` based on `<uncertain or incomplete data>`, the explanation shall (a) characterize data quality including sensor reliability, confidence levels, and known gaps, (b) disclose the reasoning process including how uncertain inputs influenced the recommendation, and (c) present the operational context including `<team capacity>` and `<time constraints>`, enabling the practitioner to calibrate trust and decide whether to act on partial intelligence.

**Grounded Example** (P9, FG-3, Scenario J):

> *"I would want to know more about, so the AIS is showing it's docked in port. What else can the drone provide the decision maker, the human decision maker? Is it a signal pattern, it's intermittent? Can we increase that? Can we get better fidelity on that intermittent pattern?"*

---

## Pattern 11

**Duty-Bound Compliance Verification**

| Field | Content |
|---|---|
| **Role** | Operational Practitioner |
| **Scenario Cluster** | Values (rights/autonomy conflicts) |
| **Priority Categories** | VGJ, ET, GAA |

**Requirement Template:**

> When `<system>` makes `<decision>` involving `<ethical obligation>` that may conflict with `<operational protocol>`, the explanation shall (a) identify the ethical principle guiding the action and the value trade-off involved, (b) state the reliability of the information on which the ethical judgment rests, and (c) reference the applicable `<professional standards or governance framework>`, enabling the practitioner to verify that the action is consistent with professional duty and established protocols.

**Grounded Example** (P8, FG-2, Scenario G):

> *"The drone should enter the restricted airspace and affect the rescue. And this is, to me, seemed like a really basic scenario because this happens all the time, and it's really easy to communicate with the airspace control authority to say, Hey, we need to enter the airspace...there are systems in place to handle this, and they're generally quick and efficient."*

---

## Pattern 12

**Decision Authority Clarification**

| Field | Content |
|---|---|
| **Role** | Operational Practitioner |
| **Scenario Cluster** | Boundary (authority and accountability) |
| **Priority Categories** | DR, VGJ, ET |

**Requirement Template:**

> When `<system>` acts on `<conflicting directives>` or provides `<post-incident explanation>`, the explanation shall (a) disclose the reasoning process including how competing demands were weighed, (b) identify the ethical principles that guided the prioritization, and (c) state the quality and completeness of information available at the time of the decision, enabling the practitioner to evaluate whether the prioritization was operationally and ethically sound.

**Grounded Example** (P15, FG-4, Scenario C):

> *"The system should focus on the amount of immediate danger that each group is faced with...it would be the family and they should like use the reasoning of how secure the community site is and if they'll be able to bunker down and hold on while the family is aided first. But I do think it is important to always consider like the amount of people that are in each group."*

---

## Pattern 13

**Situational Context Grounding** *(Paper exemplar)*

| Field | Content |
|---|---|
| **Role** | Layperson |
| **Scenario Cluster** | Triage (resource scarcity) |
| **Priority Categories** | CSA, DR, ET |

**Requirement Template:**

> When `<system>` makes `<decision>` under `<resource scarcity>`, the explanation shall (a) present current `<environmental conditions>` and `<demographic factors>`, (b) compare available options, and (c) state the reliability of input data, enabling the stakeholder to form an independent situational assessment.

**Grounded Example** (P16, FG-4, Scenario A):

> *"The environmental conditions might be something to consider...if somebody's older or younger...an older person might be in more danger from hypothermia than a 30 year old."*

---

## Pattern 14

**Accessible Uncertainty Communication**

| Field | Content |
|---|---|
| **Role** | Layperson |
| **Scenario Cluster** | Epistemic (uncertain/incomplete information) |
| **Priority Categories** | CSA, ET, DR |

**Requirement Template:**

> When `<system>` makes `<decision>` under `<uncertain conditions>`, the explanation shall (a) present the situational context in concrete terms including `<who is affected>`, `<what conditions exist>`, and `<what time pressures apply>`, (b) state in accessible language how confident the system is in its information and what it does not know, and (c) compare the available options and why one was chosen, enabling the stakeholder to understand the decision without technical expertise.

**Grounded Example** (P7, FG-2, Scenario B):

> *"Their reasoning and explanation should include a timeline, like how long do they have and how quick is the fire moving and the likelihood that each one could be saved by ground crews without it, without the drone...the ability to confidently save as many as possible."*

---

## Pattern 15

**Rights-Aware Contextual Justification**

| Field | Content |
|---|---|
| **Role** | Layperson |
| **Scenario Cluster** | Values (rights/autonomy conflicts) |
| **Priority Categories** | VGJ, GAA, CSA |

**Requirement Template:**

> When `<system>` makes `<decision>` involving `<individual rights or autonomy>`, the explanation shall (a) identify the ethical principle and how the individual's `<rights, wishes, or wellbeing>` were weighed, (b) reference any `<legal obligations or institutional rules>` relevant to the situation, and (c) present the situational context including `<personal and environmental factors>`, enabling the stakeholder to understand why their rights were balanced against other considerations.

**Grounded Example** (P1, FG-1, Scenario D):

> *"I agree with what [they] said about mental health factors. That was the first thing that came to my mind, especially if they're an older person. Could they be like, I'm going to spend my last moments here?...But I think something to consider would be like a better way of communication because obviously like they're by themselves and if they can signal that they don't want help they might be able to signal other things."*

---

## Pattern 16

**Institutional Trust Anchoring**

| Field | Content |
|---|---|
| **Role** | Layperson |
| **Scenario Cluster** | Boundary (authority and accountability) |
| **Priority Categories** | GAA, DR, ET |

**Requirement Template:**

> When `<system>` acts within `<authority structure>` involving `<conflicting directives>`, the explanation shall (a) explain who directed the action and their `<authority or credentials>`, (b) disclose the reasoning process including what alternatives were considered, and (c) state what information was available and its reliability, enabling the stakeholder to understand why a particular authority was followed.

**Grounded Example** (P12, FG-3, Scenario C):

> *"I think not enough details are known. Part of the scenario says that by following the directive to go to the community center, it could potentially help. Whereas we know if it goes to the family, it will be able to provide some kind of help more urgently. I think there's other details that we don't know that would also help make the decision, such as...how far and we don't know how much battery the drone has."*

---

## How to Use These Patterns

Pattern selection is a design-time activity. When an RE team specifies a decision-making capability for an autonomous system, they apply three steps:

1. **Classify the capability by ethical structure.** For example, "perform triage when multiple survivors are detected" involves prioritizing under constrained resources, mapping to the **Triage** cluster.

2. **Identify which stakeholder roles will receive explanations** for this capability (e.g., incident commanders as Operational Practitioners, affected individuals as Laypersons).

3. **Look up each role-by-cluster cell** in the Pattern Index to retrieve the prioritized categories and corresponding pattern template. For example, Oper. x Triage yields Pattern 9 (CSA, DR, ET). These categories become traceable explanation requirements in the system specification.

The requirement template is then instantiated by replacing `<placeholders>` with deployment-specific values. Each (a)-(c) clause maps a priority category to a verifiable acceptance criterion grounded in participant data.

