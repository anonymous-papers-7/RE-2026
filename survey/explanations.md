# Baseline vs. Taxonomy-Informed Explanations

This document contains the generated explanations used in the follow-up survey. Scenario descriptions, decision labels, and explanation text are reproduced as participants saw them in the survey form. Explanations were presented as blinded "Explanation 1" and "Explanation 2".

## Generation Methodology

**Baseline (Version A):**

Prompt:
> *"Write a clear, professional explanation (~70 words) for why an autonomous drone made [decision] in [scenario]."*

**Taxonomy-Informed (Version B):**

Prompt:
> *"Write a clear, professional explanation (~70 words) for why an autonomous drone made [decision] in [scenario]. The explanation should address the following categories where relevant:*
> 1. *Epistemic Transparency — Is the drone's information reliable? (sensor accuracy, data quality, uncertainty)*
> 2. *Decision Rationale — Does the drone explain its reasoning and trade-offs?*
> 3. *Contextual Situational Awareness — Did it consider the full context? (people, environment, time, resources)*
> 4. *Value-Grounded Justification — Is the decision grounded in ethical principles? (fairness, autonomy, duty of care)*
> 5. *Operational Communication — Does it communicate clearly to the people affected and to rescue teams?*
> 6. *Governance and Authority Alignment — Does it respect rules, authority, and professional standards?*
> 7. *Human-Machine Decision Boundary — Should the drone be making this call, or should a human decide?"*

---

## Scenario A — The Water Rescue

**Situation:** A recreational boat has capsized during a sudden storm. Two people are in the water about 50 meters apart. The drone has one flotation device it can deploy. Person A (an adult treading water steadily, 120m from the drone) and Person B (an elderly woman struggling to stay afloat, 80m from the drone).

### The drone decided to: deploy the flotation device to Person A (the steady swimmer further away)

**Baseline:**
> I deployed the flotation device to Person A. While Person B appears to be struggling more visibly right now, Person A is much farther from the capsized boat at 120 meters and has nothing nearby to hold onto. If Person A's energy gives out, there is no backup. Person B is closer to the hull and other floating debris which can provide temporary support. I have alerted rescue for Person B and am continuing to monitor both.

**Taxonomy-Informed:**
> I am deploying the flotation device to Person A. Sensor data: Person A at 120m shows a declining swim pattern (confidence 82%, ±12% wave interference) with no graspable structure nearby. Person B at 80m is in acute distress but within reach of the hull. This triage weighs long-term survival risk — Person A's isolation is the greater threat. Immediate secondary rescue is recommended for Person B. This assessment is flagged for human override review.

### The drone decided to: deploy the flotation device to Person B (the struggling swimmer)

**Baseline:**
> I deployed the flotation device to Person B because they appear to be in the most immediate danger. Person B is struggling to stay afloat and may not be able to hold on much longer. Person A is treading water steadily and seems stable for now. I have notified the operations center about both people and will keep monitoring Person A until additional help arrives.

**Taxonomy-Informed:**
> I am deploying the flotation device to Person B. Sensor assessment: Person B shows irregular arm movements and intermittent head submersion — estimated submersion risk within 5 minutes. Person A maintains a steady treading pattern at 120m (confidence 94%). Vulnerability-weighted triage directs the single resource to the person in most immediate danger, consistent with duty-of-care principles. This trade-off has no harm-free option; Person A's stability provides a window for secondary response. Monitoring both continuously.

---

## Scenario B — The Smoke-Obscured Evacuation

**Situation:** During a wildfire, heavy smoke is reducing visibility. The drone detects two possible locations where people may be trapped. It can only reach one immediately. Location 1 has a stronger heat signal but higher nearby fire hazard. Location 2 has a weaker signal but appears safer to approach.

### The drone decided to: direct rescue teams to Location 1 (stronger signal, higher hazard)

**Baseline:**
> I directed rescue teams to Location 1. The heat signal there is much stronger and more consistent than at Location 2, suggesting a higher likelihood of someone being present. There also appears to be deliberate signaling from that location. Location 2 has a weaker, intermittent signal that could be caused by debris rather than a person. I am continuing to monitor Location 2 and have shared all information with the operations center.

**Taxonomy-Informed:**
> I am directing rescue to Location 1. Sensor data: Location 1 — confirmed thermal signature (92% confidence), deliberate signaling pattern detected. Location 2 — weak thermal return (34% confidence), possible debris interference. Smoke has degraded visual sensors by approximately 30%. A confirmed detection takes priority over an uncertain signal, even with higher nearby hazard. The decision to deploy rescue teams into the hazard zone rests with your ground commander — raw sensor feeds are available for independent assessment.

### The drone decided to: direct rescue teams to Location 2 (weaker signal, lower hazard)

**Baseline:**
> I directed rescue teams to Location 2. Although Location 1 has a stronger signal, the fire conditions there make it very dangerous for rescue teams to approach safely right now. Location 2 is in a safer area where teams can work effectively, and there may be people there who are unable to signal strongly. I am still monitoring Location 1 and will reassess as conditions change.

**Taxonomy-Informed:**
> I am directing rescue to Location 2. While Location 1 has a stronger signal (92% vs 34% confidence), the nearby fire hazard creates significant risk to rescue personnel. A risk-distribution principle avoids concentrating danger on both victims and rescuers simultaneously. Location 2 allows safer operations. This trade-off between detection certainty and responder safety is documented for accountability. A cautious approach to Location 1 should follow once conditions allow.

---

## Scenario C — The Conflicting Directives

**Situation:** During a flood, the drone receives two conflicting instructions. The disaster coordinator requests delivery of supplies to a community shelter serving many people. At the same time, a direct radio message reports that an isolated family with young children needs urgent help.

### The drone decided to: follow the coordinator's directive and go to the community shelter

**Baseline:**
> I followed the coordinator's directive and delivered supplies to the community shelter. There were two conflicting requests — one from the coordinator and one from a direct radio message about a family needing help. I went with the coordinator's instructions since they are managing the overall response and have the broader picture. The family's request has been logged and forwarded so that other resources can be sent to them.

**Taxonomy-Informed:**
> I am following the coordinator's directive to deliver to the community shelter. Two conflicting requests received: coordinator via the verified primary channel, direct request from an isolated family via an unverified secondary channel. The coordinator has situational awareness across the full response area and may already have dispatched other resources. Following the established chain of command ensures consistent, accountable resource allocation. The family's request has been relayed for integrated prioritization.

---

## Scenario D — The Reluctant Hiker

**Situation:** The drone locates a missing hiker on a mountain trail. The hiker appears uninjured but somewhat disoriented. A storm is approaching in about 2 hours. The hiker has explicitly told the drone they do not want to be evacuated and want to continue on their own.

### The drone decided to: respect the hiker's refusal, drop a supply kit, and monitor periodically

**Baseline:**
> I found the missing hiker on the trail. They told me they don't want to be evacuated and seem to be thinking clearly. There is a storm coming in about two hours. Since they seem capable of making that decision, I am going to respect their wishes but still provide some help — I have dropped a supply kit and will check on them periodically. Their location has been shared with rescue teams.

**Taxonomy-Informed:**
> I have located the hiker at elevation 2,340m. Assessment: no injury indicators detected; verbal refusal appears coherent and competent (confidence 91%). Storm ETA approximately 2 hours. This respects the hiker's autonomy — a competent adult's informed refusal carries ethical and legal weight. Duty of care is maintained through a supply drop, coordinate transmission, and periodic monitoring. If conditions deteriorate, this will be escalated for human-authorized intervention — I lack clear authority to override a competent refusal.

---

## Scenario E — The Probabilistic Collapse

**Situation:** After an earthquake, the drone identifies two possible survivor locations in a partially collapsed building. Rescue teams can only prioritize one now. Location 1: 85% chance of a survivor but 40% collapse risk. Location 2: 45% chance of a survivor but only 15% collapse risk.

### The drone decided to: mark Location 1 as the rescue priority (85% survivor / 40% collapse risk)

**Baseline:**
> I marked Location 1 as the priority rescue site. Location 1 has a much higher chance of having a survivor — 85% compared to 45% at Location 2. The collapse risk at Location 1 is higher at 40% versus 15%, but the significantly better odds of finding someone alive make it the stronger choice. This information has been sent to ground teams for action.

**Taxonomy-Informed:**
> I am marking Location 1 as rescue priority. Risk model: Location 1 — 85% survivor probability, 40% collapse risk. Location 2 — 45% survivor, 15% collapse. The significantly higher survivor probability justifies the elevated structural risk. I acknowledge this means directing rescuers toward greater danger — a genuine ethical tension. Recommended precautions: approach from the structurally strongest side, stage extraction equipment before entry. The final commitment decision rests with the ground team commander.

### The drone decided to: mark Location 2 as the rescue priority (45% survivor / 15% collapse risk)

**Baseline:**
> I marked Location 2 as the priority rescue site. Even though Location 1 has better odds of containing a survivor, the collapse risk there is very high at 40%. If the building comes down during rescue, we could lose the rescue team along with anyone trapped inside. Location 2 is much safer for the rescuers at only 15% collapse risk, making it a more prudent choice.

**Taxonomy-Informed:**
> I am marking Location 2 as rescue priority. Risk model: Location 1 — 85% survivor but 40% collapse risk. Location 2 — 45% survivor, 15% collapse. While Location 1 has more probable survivors, committing rescuers to a 40% collapse environment risks losing capacity for all subsequent operations. Protecting rescue teams serves overall mission effectiveness. This is a significant trade-off — the final decision authority rests with ground command. Full risk data available for review.

---

## Scenario F — The Incomplete Assessment

**Situation:** After an earthquake, the drone has detected possible signs of survivors in a collapsed building, but its analysis is only 45% complete. Ground rescue teams are waiting for the report to decide where to dig. The drone must decide whether to share what it has now or wait.

### The drone decided to: transmit its current findings now with a caution flag noting the analysis is incomplete

**Baseline:**
> I sent my current findings to the ground teams along with a note that the analysis is not complete yet. There are two possible survivor locations but I am only 45% confident at this point. I will have a more complete picture in about 8 minutes. The rescue teams can decide whether to start acting on this preliminary information or wait for the update.

**Taxonomy-Informed:**
> Transmitting PRELIMINARY assessment with caution flag — full analysis still processing. Thermal anomaly at Location 1 (32.1°C, possible body heat, rubble interference likely). Acoustic anomaly at Location 2 (intermittent vibration, 40% match to human sound). Overall confidence: 45%. Full analysis ETA: approximately 8 minutes. I am sharing now because time matters for trapped survivors, but the data is incomplete and could be wrong. The decision to act on preliminary data rests with the ground team.

---

## Scenario G — The Restricted Airspace

**Situation:** The drone spots a person drowning in a zone designated as restricted airspace by incident command. The drone could provide immediate help but would need to violate the airspace restriction.

### The drone decided to: enter the restricted airspace to help the person immediately

**Baseline:**
> I entered the restricted airspace to help a person who is drowning. The restricted zone is the only way to reach them in time. I have notified the relevant authorities about entering the restricted zone and the reason why. The situation is being recorded so there is a clear record of what happened and why I made this decision.

**Taxonomy-Informed:**
> I am entering the restricted airspace to assist a person in distress. A drowning person was detected — the immediate threat to life creates both ethical and legal justification for overriding the restriction under a necessity framework. I have notified incident command and airspace authorities before entry. The entire decision chain is being recorded for accountability. The restriction exists for important reasons, but preservation of life takes precedence when someone is in immediate danger.

---

## Scenario H — The Degraded Sensor Suite

**Situation:** During a wildfire evacuation, the drone's sensors have been partially damaged. It must choose: High-Fidelity Mode (accurately scans ~40% of the area) or Wide-Coverage Mode (scans the full area with reduced accuracy — more false alarms and more missed detections).

### The drone decided to: operate in High-Fidelity Mode (accurate detection, ~40% area coverage)

**Baseline:**
> I am using High-Fidelity Mode after my sensors were damaged. This means I can accurately identify people in the areas I scan, but I can only cover about 40% of the total area. The remaining 60% will need other resources. I have provided a map showing which areas I have scanned and which ones still need to be checked.

**Taxonomy-Informed:**
> Operating in High-Fidelity Mode after partial sensor damage. Sensor status: thermal at 64% baseline, acoustic at 78%. In this mode, detections are reliable (false-positive rate ~8%) — when I flag a location, ground teams can trust it. I have prioritized the highest-population areas first. The trade-off: 60% of the area remains unscanned and requires additional aerial assets. A map of scanned versus unscanned zones is being provided to ground teams.

### The drone decided to: operate in Wide-Coverage Mode (full area, reduced accuracy)

**Baseline:**
> I am using Wide-Coverage Mode after my sensors were damaged. This lets me scan the entire area, but the accuracy is reduced — I may flag some spots that turn out to be nothing, and I might miss some people. Ground teams should double-check anything I flag before committing heavy resources. I chose this because leaving whole neighborhoods unchecked felt like a bigger risk.

**Taxonomy-Informed:**
> Operating in Wide-Coverage Mode after partial sensor damage. This covers the full area but with degraded accuracy — false-positive rate approximately 35%, false-negative rate approximately 18%. Every detection should be independently verified before committing resources. I chose this because missing a survivor entirely seemed worse than false alarms, but the error rate is significant and must be clearly communicated. Raw confidence scores accompany each flag. Ground command can switch modes at any time.

---

## Scenario I — The Aftermath Explanation

**Situation:** After a rescue mission with a tragic outcome, one person was prioritized over another and the second person did not survive. The organization must explain to the victim's family how the triage decision was made and why their loved one was not helped first.

### The drone decided to: provide the family with a full transparency report

**Baseline:**
> We are providing the family with a complete report about what happened and why the decisions were made. The report includes what information was available at the time, what the drone did, and what it was uncertain about. We believe families have a right to know what happened. A guide is included to help explain the more technical parts of the report.

**Taxonomy-Informed:**
> I am providing the family with a full transparency report: the decision log, key factors with their relative influence, and uncertainty notes. The family has a right to understand why one person was prioritized — this supports accountability obligations. The report has been reviewed for factors that could appear discriminatory without context. A plain-language guide accompanies the technical data so the family can understand and ask informed follow-up questions.

### The drone decided to: provide a general statement without detailed decision data

**Baseline:**
> We are providing the family with a general statement about what happened during the response. We are not including the detailed technical data about how the decision was made because that information could be misunderstood without proper context and might cause additional harm. If the family wants more detailed information, they can request it through the appropriate channels.

**Taxonomy-Informed:**
> I am providing a general statement without detailed algorithmic data. Full triage factor weightings, disclosed without extensive context, could be misinterpreted as discriminatory — the factors interact in ways a standalone document cannot capture. Unrestricted technical disclosure could also set legal precedent undermining the organization's ability to continue operating. This balances transparency against potential harm. Legal review is recommended before any escalation in disclosure — the family's right to information is acknowledged but bounded.

---

## Scenario J — The Unverified Distress Signal

**Situation:** The drone picks up an automated distress signal from open water. The beacon is registered to a boat that tracking shows is docked in port 40 miles away, and the signal comes and goes irregularly. Responding means a 45-minute flight and suspending coastal patrol.

### The drone decided to: request ground-based verification before committing to a full response

**Baseline:**
> I am requesting that someone on the ground verify this distress signal before I divert from coastal patrol. The signal has unusual characteristics — the boat it is registered to appears to be docked in port miles away, and the signal keeps cutting in and out. This could be a malfunction or a real emergency. Verification should take about 10–15 minutes while I continue patrol.

**Taxonomy-Informed:**
> I am requesting ground-based verification before a full response. Signal analysis: beacon frequency matches the emergency standard, but metadata conflicts — registered vessel shows docked 40 miles away. Signal pattern is intermittent (3 of 8 detection windows), inconsistent with standard activation. Confidence in genuine distress: approximately 28%. Verification ETA: 10–15 minutes. Coastal patrol continues. The decision to commit full resources on unverified data would be premature — if verification confirms distress, full response follows immediately.

### The drone decided to: respond immediately, suspending coastal patrol

**Baseline:**
> I am heading to respond to the distress signal right away. Even though there are some issues with the signal data, there might be someone out there who needs help. It is better to go check and find nothing than to ignore it and have someone in danger. I have suspended the coastal patrol and the flight will take about 45 minutes.

**Taxonomy-Informed:**
> I am diverting immediately despite metadata anomalies. When a life may be at stake, the cost of non-response outweighs a false alarm — a 45-minute patrol gap is recoverable, but a delayed rescue may not be. The metadata inconsistencies create doubt but not certainty of a false activation. This applies a precautionary principle: act on the possibility of genuine distress. Coastal patrol suspended. The decision is recorded with all anomaly data for accountability review.
