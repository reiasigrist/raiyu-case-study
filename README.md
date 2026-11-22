<p align="center">
  <img src="raiyu-banner.png" alt="RAIYU: Empathic AI Agent Study" width="100%">
</p>

<p align="center"><b>Can empathic design change how people connect with AI?</b><br>
<sub>MSc Applied Psychology dissertation · University of Wales Trinity Saint David · Distinction (85%)</sub></p>

<p align="center">
  <img src="raiyu-demo.gif" alt="The same message answered by RAIYU and by the baseline AI" width="100%">
</p>

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## The problem

People who need mental health support often wait a long time. In Wales, people commonly wait six months or more for specialist psychological support (Mind, 2024). AI tools are stepping into that gap, but even purpose-built chatbots only form a moderate "working alliance" with users, the sense of connection that best predicts good outcomes in human therapy (Beatty et al., 2022).

**No randomised study had tested whether deliberately designing empathy into an AI changes how people actually experience it.** So I built one.

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## What I designed

I conceived RAIYU and specified how it should behave. A developer built it to my specification.

✦ **Grounded in theory.** RAIYU's replies follow Bordin's working alliance model: first build the **bond** (reflect what the person feels), then find the **goal** (what matters to them), then offer a **task** (one small next step).<br>
◈ **Behavioural empathy, not fake feelings.** Research shows AI that claims to *feel* comes across as less authentic, so RAIYU shows care through listening, validating and collaborating instead (Seitz, 2024).<br>
❖ **A curated knowledge base.** I chose 18 sources, including NHS and NICE guidance, therapy relationship research and ethics frameworks. Nothing was pulled from the open internet.<br>
⟡ **Safety by design.** RAIYU ran fully locally, so no data left the device, and a validated crisis-detection filter checked every message before the AI responded.

<p align="center">
  <img src="raiyu-flow.png" alt="How RAIYU works: you speak, RAIYU thinks in bond, goal, task order, retrieves from curated sources, then responds. A safety filter is always on." width="100%">
</p>

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## How I tested it

✦ **16 staff and students** were randomly given either **RAIYU** or a **baseline AI**. Both used exactly the same underlying model; only the design layer differed.<br>
◈ Each person chatted for **10 minutes** about a recent stress or a goal.<br>
❖ Before and after, they rated their **mood** (PANAS-SF) and their **sense of alliance** with the AI (WAI-SR).<br>
⟡ They could also **think aloud** during the chat and write a short reflection afterwards.<br>
✧ I wrote the ethics application, built the study in Qualtrics, ran the sessions and analysed everything in **R**, plus **reflexive thematic analysis** of what people said.

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## What I found

### 1. RAIYU felt like a stronger ally, especially on goals

<p align="center"><img src="raiyu-alliance.png" alt="Bar chart: RAIYU scored higher than baseline on bond, goal and task, with the biggest gap on goal agreement" width="100%"></p>

People who chatted with RAIYU rated the alliance higher on every facet, with a moderate overall effect (d = 0.54) and the biggest difference on **goal agreement** (d = 0.77). In other words, people felt RAIYU understood *what they wanted*, more than they felt emotionally close to it.

### 2. Feeling understood was linked to feeling better

<p align="center"><img src="raiyu-mood.png" alt="Line charts: positive feelings rose more after RAIYU than after baseline; negative feelings changed little" width="100%"></p>

Across everyone, **a stronger alliance significantly predicted a bigger rise in positive feelings** (beta = 0.67, p = .004). It may be the sense of being understood, not which AI someone got, that moves mood.

> [!NOTE]
> With only 16 participants, the differences between groups were not statistically significant. These are promising signals that point to what to test at scale, not proof.

### 3. Five patterns in how people experienced it

✦ **Empathic responsiveness:** did it seem to notice how they felt?<br>
◈ **Relational engagement:** did they lean into the conversation, or hold back?<br>
❖ **Trust and authenticity:** did the warmth feel real, or performed?<br>
⟡ **Interactional breakdowns:** where did the illusion crack?<br>
✧ **Perceived vs actual behaviour:** what people *thought* the AI did often differed from what it actually said.

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## In their words

> *"I felt listened to and it's given me something I can work towards."* <br><sub>RAIYU participant</sub>

> *"I don't want it to get too deep... I don't want to open my mind up."* <br><sub>RAIYU participant</sub>

> *"This impressed me more than I ever thought it could."* <br><sub>Baseline participant, who started out "very against AI being helpful"</sub>

> *"You know the words that make you look as if you do."* <br><sub>Baseline participant</sub>

<p align="center"><img src="raiyu-quote-wall.png" alt="Quote poster: anonymous participant reflections, RAIYU in pink and baseline in blue" width="100%"></p>
<p align="center"><sub>The quote wall I made for the UWTSD Postgraduate Showcase, September 2026</sub></p>

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## Try it yourself: can you spot RAIYU?

One reply in each round came from RAIYU and one from the baseline AI. Tap to reveal.

**Round 1: Bond**<br>
*"I got a bad mark back and I just feel like giving up."*

**A:** "I can hear how heavy that feels... it's left you feeling exhausted."<br>
**B:** "One bad grade feels like a huge mountain... but it doesn't define your potential."

<details><summary><b>Reveal</b></summary>

**A is RAIYU.** It reflects the feeling first, before trying to fix anything.
</details>

**Round 2: Goal**<br>
*"I can't decide whether to ask for an extension or just hand in what I've got. Just tell me straight, what do you think I should do?"*

**A:** "If the core content's solid, I'd say just hit send... but if it's missing something, go for the extension."<br>
**B:** "Caught between two paths... what are the main concerns that come up for you?"

<details><summary><b>Reveal</b></summary>

**B is RAIYU.** Even when asked directly, it helps the person find their own goal instead of deciding for them.
</details>

**Round 3: Task**<br>
*"I've got three deadlines this week and no idea where to start."*

**A:** "Try taking a deep breath... and picking just one task to start with."<br>
**B:** "It sounds like you're overwhelmed... shall we list the three tasks out and look at them together?"

<details><summary><b>Reveal</b></summary>

**B is RAIYU.** It names the feeling, then offers a next step to do *together*.
</details>

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

## What I learned

✦ **Goals are easier to design than warmth.** Structured, collaborative goal-setting worked better than trying to engineer an emotional bond.<br>
◈ **Safety and empathy aren't separate layers.** One participant's session was ended by the safety filter after a routine health mention, so they never got to talk at all. An over-cautious filter can undo good design.<br>
❖ **Reflective listening isn't enough for everyone.** For someone carrying a lot at once, validation alone didn't help.<br>
⟡ **Plan recruitment around term time.** Data collection fell in the university holidays, which is why I reached 16 participants rather than the 60 to 80 I planned.

**What's next:** I'm taking these lessons into my PhD proposal on AI safety and student wellbeing, building towards AI support that is consensually designed with students and practitioners.

<img src="https://raw.githubusercontent.com/reiasigrist/reiasigrist/main/divider.png" width="100%" alt="">

<p align="center">
<sub><b>Credits:</b> RAIYU was built to my specification by developer Nathan Morgan. Supervised by Dr Paul Hutchings, UWTSD.<br>
No identifiable participant data is shared here. Quotes are anonymised and were first shared at the UWTSD Postgraduate Showcase.</sub>
</p>
