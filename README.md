# Push/Pull Calculator

Free push/pull calculator based on the Snook / Liberty Mutual tables (US) plus the UK HSE RAPP assessment. Enter a measured initial and sustained force, distance, handle height and rate to get the design-goal forces, Risk Index, maximum repetitions, and a RAPP score. For information only; not a substitute for a professional ergonomic assessment.

**Live version:** https://resdavo.github.io/push-pull-calculator/ (to be published)

The calculator is a single HTML file (`index.html`). It runs entirely in your browser — there is nothing to install, and no data you enter is sent anywhere.

## How to use it

1. Open the live version above, or open `index.html` in a browser.
2. Choose whether the task is a push or a pull.
3. Enter the values for the task (see below) — the measured forces, distance, handle height and rate.
4. Read the design-goal forces, the Risk Index, the maximum repetitions, and, for the UK assessment, the RAPP score.
5. If the Risk Index is above 1.0, or the RAPP score is in a higher band, look first at the factor that is driving it — a lower force, a shorter distance, a better handle height, or a slower rate.

Measure the forces on the actual task, with the actual load, floor and equipment. A force guessed from the weight of the load is not a measured force.

## What you enter

- Push or pull
- Measured initial force — the force needed to get the load moving
- Measured sustained force — the force needed to keep the load moving
- Distance the load is pushed or pulled
- Handle height
- Rate — how often the push or pull is repeated

## What it calculates

- Design-goal initial force and design-goal sustained force for the task
- Risk Index — measured force divided by the design goal (see below)
- Maximum repetitions for the task at the measured force
- A RAPP score for the UK assessment, scored factor by factor

## How the calculation works

The US calculation is based on the Snook / Liberty Mutual tables. For the distance, handle height and rate you enter, the tables give a **design goal**: the maximum initial and sustained force that is acceptable to 75% of women. Because women on average have lower push/pull strength than men, a force acceptable to 75% of women protects more than 90% of men — so designing to that goal covers most of a mixed workforce.

The **Risk Index** compares your measured force with that design goal:

```text
Risk Index = measured force ÷ design goal
```

- A Risk Index of 1.0 or less meets the design goal.
- A Risk Index above 1.0 means the measured force is higher than the force acceptable to 75% of women. The further above 1.0, the smaller the share of the workforce the task suits, and the more reason there is to change the task.

The initial and sustained forces are checked separately; either one can be the one that puts the task over the design goal.

The UK **RAPP** (Risk Assessment of Pushing and Pulling) assessment works differently. Instead of one formula, it scores the task factor by factor — load, distance, force, posture, grip, floor surface, obstacles and other factors — and adds the factor scores into a total score with a colour band. One factor is different: if the load is **Purple**, the assessment stops there. Purple means the task is beyond the scope of the RAPP tool and needs a more detailed, specialist assessment — do not carry on and total up the other scores as if it were an ordinary result.

## US and UK method notes

- **United States — Snook / Liberty Mutual tables:** The design goals come from the published Snook & Ciriello tables for pushing and pulling, which vary with distance, handle height and frequency. OSHA has no push/pull force-limit standard; its eTool guidance on pushing, pulling and carrying is general guidance on reducing the risk, not a legal force limit.
- **United Kingdom — HSE RAPP:** RAPP is the Health and Safety Executive's assessment tool for pushing and pulling, published as INDG478, and sits under the Manual Handling Operations Regulations guidance in L23. A RAPP score is an assessment aid: a higher score means a higher priority for action, not by itself a finding that the law has been broken.

## Reporting an error

If you find an error, please open an Issue in this repository. Include the values you entered — push or pull, initial and sustained forces, distance, handle height and rate — and the result you expected, so the calculation can be checked against the same inputs.

## Sources

- Snook, S.H. & Ciriello, V.M. (1991). The design of manual handling tasks: revised tables of maximum acceptable weights and forces. *Ergonomics*, 34(9), 1197–1213.
- Health and Safety Executive — RAPP tool, INDG478: *Risk assessment of pushing and pulling (RAPP) tool*.
- Health and Safety Executive — L23: *Manual handling — The Manual Handling Operations Regulations 1992: Guidance on Regulations*.
- OSHA eTool — Pushing, Pulling and Carrying.

These methods are summarised in the calculator. Read the full text before making compliance decisions.

## Disclaimer — please read before using this calculator

This calculator was created by David O Restrepo to the best of his knowledge and abilities, with assistance from Muse AI. It is provided free of charge, “as is,” without any warranty of any kind, express or implied, including any warranty of accuracy, completeness, or fitness for a particular purpose.

Despite careful checking, this calculator may contain errors — in its formulas, tables, conversions, or interpretation of the underlying standards. Its results are estimates based on the published methods cited above. They are not a substitute for a professional ergonomic assessment, the advice of a qualified safety professional, or the full text of the applicable standard or regulation. Always verify important results independently and consult the official sources listed above before making workplace, health, safety, or compliance decisions.

By using this calculator, you agree that you do so entirely at your own risk and that you assume full responsibility for any decision or action taken based on its results. To the fullest extent permitted by law, by using it you waive and release David O Restrepo from any and all claims, demands, damages, losses, and liabilities of any kind arising out of or in connection with your use of this calculator or reliance on its results. If you do not agree to these terms, do not use this calculator.

## Author

Created by David O Restrepo, using Muse AI.
