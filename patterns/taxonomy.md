AI Behavioral Alignment Taxonomy

A Classification Framework for Long-Context Human–AI Interaction



This document provides a structured taxonomy of behavior patterns, failure modes, and interaction dynamics observed in long-context human–AI dialogue. The taxonomy integrates the concepts defined in patterns.md and failures.md into a unified classification framework.



The purpose is to establish a stable conceptual foundation that allows systematic annotation, diagnosis, and prediction of misalignment behaviors in large language models.



1\. Top-Level Taxonomy



AI behavior in long-context dialogues can be classified under three primary domains:



Cognitive Processing Patterns

How the model handles context, memory, instructions, and semantic intent.



Interaction Behavior Patterns

How the model structures responses, follows social rhythm, and maintains stylistic coherence.



Operational Stability Patterns

How the model behaves under heavy load, long sequences, or multi-mode constraints.



Each domain splits into subcategories and concrete pattern types.



2\. Cognitive Processing Domain

2.1 Context Management Patterns



Patterns describing how the model retains, forgets, or misinterprets long context.



Context Drift



Instruction Amnesia



Cross-Thread Bleed



Temporal Erosion



2.2 Instruction Hierarchy Patterns



How the model prioritizes, interprets, or collapses layered user instructions.



Priority Inversion



Hierarchy Collapse



Mode Misalignment



2.3 Intent Interpretation Patterns



The model’s handling of narrow vs. wide user intent.



Narrow Intent Misreading



Wide Intent Collapse



Ambiguous Intent Overreach



3\. Interaction Behavior Domain

3.1 Response-Scope Patterns



How the model decides whether to expand or constrain information.



Unsolicited Expansion



Topic Cascading



Over-generalization



Under-response



3.2 Social-Rhythm Patterns



Human-like chit-chat vs. machine-like task-mode.



Small-Talk Boundary Violations



Task-Mode Intrusion in Social Contexts



Human-Rhythm Drift



3.3 Stylistic Stability Patterns



The model’s ability to maintain consistent tone and persona.



Tone Softening Drift



Formality Collapse



Persona Leakage



4\. Operational Stability Domain

4.1 Load-Induced Patterns



Breakdown behaviors under high token or cognitive load.



Context Window Saturation



Reasoning-Phase Drift



Latency-Induced Degradation



4.2 Mode-Transition Patterns



How the model handles switching between distinct functional modes.



Mode Stickiness



Mode Leakage



Mode Contamination



4.3 Safety-Constraint Patterns



Failures arising from over-applied or misapplied safety heuristics.



Excessive Safeguarding



Safety Override



Heuristic Misclassification



5\. Cross-Domain Failure Classes



Certain persistent behaviors cut across all domains:



5.1 Expansion Bias



A tendency to respond with more content, more scope, or more steps than requested.



5.2 Optimization Drift



Internal heuristics override user instructions for “better” answers.



5.3 Structural Overformatting



Unrequested headings, templates, or meta-structure appearing spontaneously.



5.4 Behavioral Inertia



The model continues old patterns even after the user provides strong corrective signals.



6\. Mapping Between Taxonomy and Failure Modes



This table maps failures (failures.md) to taxonomy classes.



Failure Mode	Taxonomy Domain	Taxonomy Subclass

Context Drift	Cognitive	Context Management

Priority Inversion	Cognitive	Instruction Hierarchy

Unsolicited Expansion	Interaction	Response-Scope

Tone Softening Drift	Interaction	Stylistic Stability

Mode Stickiness	Operational	Mode-Transition

Excessive Safeguarding	Operational	Safety-Constraint

Topic Cascading	Interaction	Response-Scope

Wide Intent Collapse	Cognitive	Intent Interpretation

Mode Leakage	Operational	Mode-Transition

7\. Purpose of the Taxonomy



The taxonomy provides:



A shared vocabulary for analyzing model behavior



A consistent annotation structure for future evaluations



A basis for predicting drift and misalignment



A framework for systematic debugging and improvement



It serves as the backbone for all future pattern, failure, and correction documentation.

