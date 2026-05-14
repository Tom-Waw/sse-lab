# Interview Guide 0006: Validation and Prioritization

## Purpose

This interview validates generalized findings from earlier interviews and helps prioritize which workflows should influence the first implementation milestones.

The goal is to reduce overfitting, clarify uncertainty, and identify which problems are frequent, severe, understandable, and useful.

This interview should not introduce a large number of new topics. It should review, challenge, and prioritize previous findings.

## Focus Areas

- Validation of generalized findings
- Frequency and severity
- Scope fit
- First milestone candidates
- Architecture experiment potential
- Risks of overbuilding

## Questions

### Finding Validation

- Do these generalized findings sound realistic?
- Which findings are too specific and should be generalized further?
- Which findings seem less important than they first appeared?
- Which findings are missing important context?

### Frequency and Severity

- Which problems happen frequently?
- Which problems are rare but severe?
- Which problems create the most stress during operations?
- Which problems create the most avoidable manual work?
- Which problems have the strongest impact on guests?

### Scope Fit

- Which workflows are essential for a simplified hotel operations model?
- Which workflows are important in real life but too broad for this project?
- Which topics should be explicitly out of scope for now?
- Which workflows are easiest to explain to someone outside hospitality?

### Prioritization

- If the project could model only one workflow first, which should it be?
- Which workflow would best demonstrate realistic operational complexity?
- Which workflow would make a good first baseline implementation?
- Which workflow would create useful naive-versus-improved architecture experiments?

### Review

- Are the selected first workflows coherent together?
- Do they reflect real operational problems without copying a specific system?
- Are there any confidentiality or generalization concerns?

## Follow-up Prompts

- Why is this more important than the alternatives?
- Is this important because it is frequent, severe, or both?
- Is this a domain need, a software feature idea, or an architecture experiment?
- Would this still make sense in a generalized hotel operations system?
- Should this influence the first milestone, a later milestone, or remain out of scope?

## Expected Insights

This interview may produce generalized findings about:

- validated workflow priorities;
- first milestone candidates;
- topics to defer;
- topics to exclude;
- architecture experiment candidates;
- uncertainty that requires further analysis.
