# Compute Sponsoring  
*A category definition for advertising in Generative AI*  

**Version 1.0**  
February 2026  

**Author**  
Christian Leinberger  

**Published by**  
Compute-Sponsoring.org  

Compute Sponsoring is an open standard proposal initiated by wavebird.

---

## 1. Introduction

Generative AI (GenAI) is spreading rapidly and will shape the digital landscape of the coming decades. The central paradigm shift of this technology lies in how digital value is created.

In the classic software paradigm, value is created primarily once during development and then scaled through distribution. In GenAI systems, digital value is not created solely through the one-time creation of software, but situationally through generative compute at the moment of use.

Digital value creation becomes continuous.

Where compute becomes a constitutive part of usage, it simultaneously becomes a source of cost because it continuously binds resources. This creates a structural problem: systems must be limited, priced, or cross-subsidized. Advertising is a natural solution, but in the context of GenAI it creates a novel problem space. It intensifies two core risks: opacity and influence risk.

Classic advertising measurement captures exposures, but it does not sufficiently explain how those exposures relate to the concrete performance delivered by a system. At the same time, the closer monetization moves toward model intelligence, the greater the incentive risk becomes: where economic optimization and the production of intelligence come into contact, the question of epistemic integrity arises as a matter of principle.

Compute Sponsoring aims to enable transparent and integrity-preserving funding of GenAI through advertising, supporting sustainable and broad access to advanced systems.

---

## 2. Compute Sponsoring

Compute Sponsoring means, at its core, that a sponsorship exposure can be unambiguously attributed to a concretely identifiable compute unit.

Sponsorship denotes a financial contribution that is coupled to an exposure. A sponsorship exposure is a clearly labeled event that can be measured independently. Classic brand sponsorship and classic digital advertising are typical manifestations of this category. For reasons of readability, “advertising” is used below as an umbrella term for sponsorship exposures.

A compute unit denotes an identifiable unit of active compute. Depending on the system, it may be defined, for example, as a request, a generation, a token block, or a job. What matters is not the specific form, but that the unit is unambiguously determinable and used consistently within the system.

Sponsorship exposure (advertising) and compute unit thus stand in a defined coupling relationship: the advertising is attributable to a specific compute operation, and this attribution is repeatable and auditable.

The reference point is therefore not the content claim of a system or the superficial placement of an ad, but the concrete compute process.

---

## 3. Principles

The following principles must be satisfied for something to be considered Compute Sponsoring:

**Separation of AI and advertising**  
The AI model remains untouched by advertising. Advertising always takes place on a separate technical channel and is not part of the model’s processing.

**No input influence**  
Sponsor information is never injected into the model request and is not introduced into the prompt, the context window, or tool inputs.

**No output influence**  
The content of the output is never influenced by advertising. Advertising does not cause prioritizations, omissions, or rephrasings.

**Independence from system-level decisions**  
Advertising never determines the selection of the model or the tools. Advertising never influences moderation, thresholds, or enforcement logic.

**Data sovereignty**  
Sponsors never receive user-level or request-level semantic usage data. Sponsor reporting must not enable reconstruction of individual intentions, problems, or contexts.

**Advertising transparency**  
Ads are always clearly and fully labeled. Advertising is plainly recognizable and is not disguised as response content.

**Consent to the use of semantics**  
Semantic relevance targeting of ads based on user intention and/or model intelligence is tied to explicit consent. Without consent, no semantic relevance targeting takes place.

**Consent to persistence of semantics**  
Without explicit consent, semantics are not accumulated across sessions or condensed into a profile-like history. Without consent, no persistent semantic history for ad relevance targeting is created.

**Transparency of semantic relevance targeting**  
Users must be clearly informed when semantic relevance targeting is used for ad selection and delivery.

---

## 4. Classification of semantic relevance targeting

Where semantics arising from the use of GenAI systems can be used to select and deliver advertising in a relevance-targeted manner, there is a need for unambiguous naming. It must be traceable which semantic data are used and how long they are stored and used.

In the context of semantic relevance targeting, two dimensions are central: the source of the semantics used and the persistence of those semantics over time.

### Semantic Source

**S0: System context**  
Only system metadata are used to determine ad relevance. No semantics are used for relevance targeting.

**S1: Intention (user semantics)**  
Relevance targeting is based on the semantics of the current user intention. In practice, this usually derives from the prompt.

**S2: Model intelligence (model semantics)**  
Relevance targeting is based on the model-derived semantic signals. In practice, this usually derives from intermediate results or the model output.

**S3: Combined source (intention + model intelligence)**  
Relevance targeting is based on semantic signals from both user intention (S1) and model intelligence (S2).

### Semantic Persistence

**P0: No persistence**  
Semantics are not stored. Signals are purely transient.

**P1: Session persistence**  
Semantics remain usable within a session, without being carried across session boundaries.

**P2: Cross-session persistence**  
Semantics are stored and accumulated across sessions and used for semantic relevance targeting. This can give rise to profile-based advertising.

---

## 5. Compute Sponsoring profiles

The source and persistence of the use of usage-based semantics create a matrix from which different Compute Sponsoring profiles can be constructed:

|     | P0 | P1 | P2 |
|-----|----|----|----|
| S0  | Compute Sponsoring Neutral | Not applicable | Not applicable |
| S1  | Compute Sponsoring Situational | Compute Sponsoring Situational | Compute Sponsoring Profiling |
| S2  | Compute Sponsoring Situational | Compute Sponsoring Situational | Compute Sponsoring Profiling |
| S3  | Compute Sponsoring Situational | Compute Sponsoring Situational | Compute Sponsoring Profiling |

For S0, “Semantic Persistence” beyond P0 is not applicable, since no semantic signals are used.

**Profile 1: Compute Sponsoring Neutral (CS-N)**  
Compute Sponsoring Neutral describes Compute Sponsoring without any semantic relevance targeting. Advertising is based solely on system-level context signals (S0), or on no relevance signals at all. CS-N is the least invasive form of Compute Sponsoring.

**Profile 2: Compute Sponsoring Situational (CS-S)**  
Compute Sponsoring Situational describes semantic relevance of advertising in the moment, without accumulating semantic data beyond a session. Semantics are used to make advertising situationally more appropriate, either from intent (S1), from model intelligence (S2), or from intention and model intelligence (S3), but only transiently (P0) or within a session (P1). CS-S is the zone in which relevance can be used without generating profile-forming data.

**Profile 3: Compute Sponsoring Profiling (CS-P)**  
Compute Sponsoring Profiling describes systems in which semantic signals are accumulated across sessions (P2). Whether the source is intent (S1), model intelligence (S2), or both (S3) is secondary; what is decisive is the storage and use of semantics beyond specific usage situations. As soon as semantic data are stored across sessions, profile-specific advertising can emerge.

---

## 6. Notation: declaration of systems

For Compute Sponsoring to be deployed and communicated transparently as a category, it needs a concise notation that can be stated publicly. The declaration has two levels: the profile and the exact axis position.

|     | P0 | P1 | P2 |
|-----|----|----|----|
| S0  | CS-N (S0/P0) | Not applicable | Not applicable |
| S1  | CS-S (S1/P0) | CS-S (S1/P1) | CS-P (S1/P2) |
| S2  | CS-S (S2/P0) | CS-S (S2/P1) | CS-P (S2/P2) |
| S3  | CS-S (S3/P0) | CS-S (S3/P1) | CS-P (S3/P2) |

**Use case example**

A system has the following properties: the user submits a prompt. While the model processes the request, topic-specific ads are displayed based on the prompt. The prompt’s semantic content is not stored and therefore cannot be used for semantic relevance targeting of ads on the user’s next request, even within the same session.

The correct notation for this system is:

**CS-S (S1/P0)**

---

## 7. Conformity and disclosure

### Self-declaration

Until technical specifications and formal audit mechanisms are introduced, the notation can be provided via self-declaration.

The self-declaration includes:

- confirmation that advertising can be attributed to a compute unit  
- confirmation of compliance with the principles  
- determination of the semantic source (Sx)  
- determination of the semantic persistence (Px)  
- derivation of profile and notation (CS-x (Sx/Px))  

Declarations based on self-declaration should be marked with an asterisk, for example:

**CS-S (S3/P1)\***

It is recommended to make the label visible to the user while advertising is being shown.

---

## 8. Conclusion and invitation

Compute Sponsoring responds to a new structure: in GenAI systems, compute is a central component of usage, and intelligence is created in the moment of interaction. As monetization moves closer to this process, the risk of influence increases. Advertising is only viable in this environment if it has a well-defined reference point and if integrity is not merely asserted, but transparently declared and safeguarded.

This white paper defines Compute Sponsoring as the attribution of advertising to an identifiable compute unit. It formulates the principles that protect this category and provides, with Semantic Source and Semantic Persistence, a classification scheme from which profiles and notation follow.

Anyone who uses advertising in GenAI should also be able to name it.

The claim of version 1.0 is to define the category and provide a first, practical form of transparent disclosure.

You are invited to critique Compute Sponsoring, to sharpen it, and to further develop it toward technical specification and operationalization.
