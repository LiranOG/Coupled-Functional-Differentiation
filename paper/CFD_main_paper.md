---
title: "Coupled Functional Differentiation: A Mechanism-Based Theory of the Multi-Level Human System"
author: "Liran M. Schwartz"
orcid: "0009-0008-8035-1308"
affiliation: "Independent Researcher, Haifa, Israel"
date: "May 2026"
version: "v2.0 — Working Draft / Preprint"
status: "Preprint — Not Peer-Reviewed"
license: "MIT"
---

# Coupled Functional Differentiation: A Mechanism-Based Theory of the Multi-Level Human System

**Liran M. Schwartz**
Independent Researcher, Haifa, Israel
ORCID: [0009-0008-8035-1308](https://orcid.org/0009-0008-8035-1308)

*Version 2.0 — Working Draft / Preprint, May 2026*

## Abstract

> **Disclaimer:** This is an independent working paper/preprint. It has not undergone peer review, and all claims are provisional and subject to revision based on future empirical testing and community critique. This preliminary framework is submitted for open community feedback and pending empirical validation.

This paper develops a mechanism-based theory of the human social system that resolves a tension internal to existing macrosociological accounts: the simultaneity of strong functional autonomy among societal subsystems and the increasingly tight, fast, and consequential interdependence among them. Building on Luhmann's theory of functional differentiation, Fiske's relational models, Coleman's micro–macro architecture, and Bhaskar's critical realism, we specify a single Core Generative Mechanism (CGM): functionally differentiated subsystems, each operating under a distinct binary code and a set of programs, engage in selective and asymmetric structural coupling through identifiable communication channels (contracts, money, electoral mandates, scientific publication, algorithmic feeds), generating in parallel both coordination across subsystems and tension between codes. The ego — the layered biological-cognitive-affective-motivational complex of the individual, organized around survival, recognition, and status, with affective valence on an approach/avoidance (love/fear) axis — is the locus where the loops of this mechanism meet: macro-level outputs are internalized through it, micro-level decisions are aggregated from it. The aggregate institutional layer functions as a social operating system: ideology and religion serve as the categorical glue that allows millions of unacquainted egos to coordinate; the legal subsystem replaces individual revenge with formal procedure; money operates as a "religion of trust" sustained by technology and information; affective states translate into institutional categories ("altruism becomes tax, fear becomes national security"). At the global scale, the joint operation of these loops constitutes a modern Leviathan — a globally coupled multi-system network in which money, technology, ideology, and education form a self-reinforcing cycle. From the single CGM we derive (i) the conditions under which one subsystem colonizes another; (ii) the conditions under which small-group logics flip; (iii) the conditions under which globally synchronized crises emerge; and (iv) the predicted effect of surveillance-capitalist platforms — namely, the predictive anticipation of individual decisions before reflective thought has occurred — on individual autonomy. We formalize the theory through a system of difference equations, specify a corresponding Agent-Based Model (COFD-ABM), and deduce sixteen directional, falsifiable propositions, including an explicit falsification criterion. The theory's scope conditions are specified, and it is compared systematically with world-systems theory, neo-institutionalism, network/complexity science, and analytical sociology.


**Keywords: functional differentiation; structural coupling; emergence; critical realism; Coleman boat; relational models; surveillance capitalism; agent-based modeling.**



## 1. Introduction

### 1.1 The puzzle: autonomy with interdependence

A persistent and partly unresolved problem in macrosociology is that two empirical regularities about modern societies appear to be in tension. On the one hand, modern societies exhibit pronounced functional differentiation: legal decision-making is not reducible to economic calculation, scientific validation is not reducible to political legitimation, religious or aesthetic judgment is not reducible to either (Luhmann, 1995, 2012). Each subsystem operates under a distinctive binary code (legal/illegal, true/false, profit/loss, governing/opposition) and through programs (statutes, methods, budgets, electoral procedures) that translate that code into operational decisions. On the other hand, these same societies exhibit increasingly tight cross-system coupling: financial shocks propagate to political legitimation in days; algorithmic prioritization of media content reshapes political discourse in hours; legal classifications determine access to economic credit; scientific outputs are filtered by economic and political programs before reaching public knowledge.


A reductionist response to this tension dissolves it by collapsing the differentiation: every subsystem is "really" about power (Foucault), or capital (orthodox Marxist accounts), or status (some strands of evolutionary psychology). Reductionism gains parsimony at the cost of empirical adequacy: it cannot explain why a judge applying contract law does not behave as a profit maximizer, why a peer reviewer does not behave as an electoral strategist, or why a religious authority typically resists conversion of sacred categories into market categories. A pluralist response, conversely, simply lists the autonomous subsystems and asserts their irreducibility, but in so doing risks losing explanatory traction over the very interdependencies that make modern societies fragile to systemic crises.


The theory presented here is a third option. It accepts the irreducibility of subsystem codes (against reductionism) while specifying the precise channels, mechanisms, and quantitative regimes through which interdependence is produced and through which it sometimes catastrophically tightens (against descriptive pluralism). Its central claim is that autonomy and interdependence are produced by a single generative mechanism — selective, asymmetric structural coupling — and that observable systemic properties at every scale, from individual disposition formation to global crisis dynamics, are the deductive consequences of how that mechanism operates under varying conditions of coupling density, exposure intensity, and buffering.


An earlier informal formulation of this theory, by the present authors, located the starting point of analysis in the ego — the individual self, composed of biology, cognition, affective valence (organized along an approach/avoidance axis the original sketch glossed as "love/fear"), and a motivational stack anchored in survival, recognition, and status. From there, the original sketch traced a path: the ego participates in small groups, where micro-cultural rules emerge ("what is funny, what is forbidden, who leads"); these scale into communities and nations whose accumulated practices function as a social operating system; ideology and religion serve as the categorical glue allowing millions of unacquainted egos to coordinate; institutionalized politics, law, and economy crystallize as autonomous subsystems; algorithms and aggregated information come to predict the ego's next step before reflective thought has occurred; and the resulting global formation operates as a "Leviathan" of mutually reinforcing systems in which money feeds technology, technology shapes ideology, and ideology recursively shapes the education through which the next generation's ego is formed. We retain every one of these substantive insights. The present formulation locates the theory's generative claim at the level of subsystem coupling rather than at the ego, because that is the level at which the regularities the theory predicts become formally tractable. But the ego is preserved as the locus where all four loops of the CGM meet (§3.1), and the original sketch's specific framings — fear/love valence, micro-cultural markers, social-OS metaphor, ideology-as-glue, money-as-religion-of-trust, the predictive anticipation of the ego, and the explicit Leviathan loop — are integrated as named substantive components throughout §3 and §4. The two formulations are dual descriptions of the same dynamics, with the formal core (§4.3) supplying the bridge.

### 1.2 What this paper contributes

The paper contributes the following to the literature:


A single Core Generative Mechanism (CGM) from which the macro, meso, and micro phenomena treated in separate literatures (Luhmann, Fiske, Coleman, Hedström) are recovered as special cases.

A formalization of Luhmann's previously under-operationalized concept of structural coupling into a measurable coupling matrix, with thresholds beyond which qualitative regime change is predicted.

A reconstruction of Fiske's four relational models as a dynamic switching system with specifiable situational triggers and reconciliation mechanisms, integrating Expectation States Theory and Social Identity Theory.

A treatment of surveillance capitalism not as a metaphor but as a derived case of the theory, with explicit measurable predictions about individual reflective autonomy.

Sixteen directional, falsifiable propositions, with an explicit falsification criterion that, if met, would force abandonment or fundamental revision of the theory.

A system-dynamics formalization and an Agent-Based Model specification (COFD-ABM) that instantiate the theory computationally.

A systematic comparison with four rival theoretical traditions, identifying anomalies the present theory resolves and conceding domains in which rival theories retain priority.

An explicit anchoring of the theory's individual-level locus in the ego as the meeting point of all four loops (§3.1.1), preserving the bottom-up insight of the theory's original informal formulation while subordinating it to the mechanism-based generative claim.

A formalization of the aggregate institutional layer as a Social Operating System (§3.4.1) within which ideology and religion serve as categorical glue uniting unacquainted populations, an affect-to-institution translation table maps population-level affective states to institutional outputs, and common-good legitimation rhetoric appears as a structural requirement rather than as cynical rhetoric.

An explicit derivation of the Leviathan loop — money → technology → ideology → education → ego → system → money — as the canonical closed-orbit trajectory of the system's state space (§3.7).

### 1.3 Plan of the paper

§2 develops the philosophical and methodological grounding (critical realism, the typology of emergence, scope conditions). §3 presents the Core Theoretical Model: the CGM and the four cross-level loops formalized as Coleman-boat instantiations. §4 operationalizes the theory's central concepts and introduces the formal core. §5 deduces the sixteen propositions and the falsification test. §6 compares the theory with rival traditions. §7 discusses unresolved tensions. §8 concludes. Appendices contain the equation system, the ABM specification, and an extended proposition table.



## 2. Philosophical and Methodological Grounding

### 2.1 Why a stance on the philosophy of science is necessary here

Two of the theory's central commitments — that there exist generative mechanisms not directly observable, and that some macro-level properties are not reducible to lower-level descriptions — are non-trivial in the current methodological landscape, where strong empiricism in some quarters demands that any theoretical entity be reducible to operational measurements, and where strict reductionism in others denies the explanatory necessity of macro-level constructs. We therefore cannot proceed without an explicit stance on these matters.

### 2.2 Critical realism

We adopt critical realism in the tradition of Bhaskar (1975, 1979) and its sociological development by Archer (1995, 2003). Critical realism distinguishes three ontological strata: the empirical (events as experienced), the actual (events as they occur, whether experienced or not), and the real (the underlying structures and mechanisms that, when activated, produce events). Three commitments follow.


First, mechanisms are real but not always activated. The mechanism by which financial contagion propagates through a tightly coupled banking network exists whenever the network has the relevant topology, but does not produce observable contagion until a triggering shock activates it. This implies that empirical absence of an outcome does not imply absence of the mechanism — a point of consequence for falsification, addressed in §5.


Second, explanation is multi-level and non-reductive. The fact that a judge reaches a particular decision is partly explained by the legal subsystem's code and program (a real mechanism at the institutional stratum), partly by the judge's internalized dispositions (a real mechanism at the personal stratum), and partly by the case at hand (an event at the empirical stratum). None of these is reducible to the others without remainder.


Third, emergence is permitted ontologically. We do not adopt the position that all macro-level properties must be epistemologically equivalent to micro-level descriptions. The next subsection makes this precise.

### 2.3 Weak and strong emergence

Following Bedau (1997), Chalmers (2006), and the formal treatments in complex-systems theory (Crutchfield, 1994), we distinguish:


Weak emergence: a property is weakly emergent if it is in principle computable from the behavior of lower-level components plus their interaction rules, but is not predictable in closed form and arises only through simulation or actual operation of the system. Most properties studied in complexity science (flocking, traffic patterns, market microstructure) are weakly emergent.

Strong emergence: a property is strongly emergent if it is not even in principle reducible to lower-level descriptions; it represents genuine ontological novelty.


The theory advanced here is a weak-emergence theory. We claim that the macro-level properties of the human social system — synchronized crises, norm cascades, autonomy erosion under platform mediation — are computable from the joint operation of the CGM at the level of individuals, groups, and subsystems, given the coupling matrix and exposure parameters. We do not require strong emergence and explicitly disavow it: there is no claim that the social system has properties that could not, in principle, be recovered from a sufficiently detailed multi-level simulation. This commitment matters because it makes the theory computationally tractable (the ABM specified in Appendix B is, in principle, capable of regenerating its predicted macro-properties) and methodologically more conservative.

### 2.4 Scope conditions

Theories of long historical reach are tempting but rarely useful. The present theory is bounded as follows.


Temporal scope. The theory is intended to apply to societies after the consolidation of functional differentiation — that is, roughly, post-1800 in Western Europe and North America, with progressively later onsets in other regions. In societies organized primarily on segmentary or stratified principles (Luhmann, 1995, ch. 4), the differentiation premise of the CGM does not hold, and the theory's predictions cannot be expected to apply.


Cross-system scope. The theory applies to societies in which at least four of the seven subsystems we treat (legal, economic, political, scientific, religious, aesthetic, mediatic) are operationally autonomous. In societies where, for example, the legal subsystem is fully subordinated to the political (autocratic regimes with no rule-of-law independence) or the scientific to the religious, the CGM predictions about colonization (§3.4) apply, but the cross-coupling predictions of §3.5 require modification.


Scale scope. The propositions about global-scale emergence (§3.7) require a baseline of cross-border information, financial, and migratory flows above thresholds that did not exist before the latter twentieth century. We make no claims about pre-1945 globally synchronized crises, except to note that earlier crises (e.g., 1873, 1929) provide partial test cases that we discuss in §5.


Conditions under which the theory is expected to fail. The theory is most likely to fail (a) in small, isolated communities with low cross-subsystem coupling, where the loops simplify to the point of triviality; (b) in totalitarian regimes that suppress the autonomy of multiple subsystems simultaneously, where the CGM's operating premise is violated; and (c) in periods immediately following catastrophic shocks (war, mass-casualty disaster) when subsystem codes themselves are temporarily suspended. We discuss the implications of these limitations in §8.2.

### 2.5 Methodological pluralism

The theory is testable through a deliberately wide range of methods. Different propositions admit different instruments: laboratory experiments for group-level logic switching (P1, P8); cross-cultural psychology for emotion-internalization differentials (P2); computational network analysis for cross-subsystem coupling indices (P3, P7, P14); NLP on institutional texts for colonization signatures (P4); longitudinal cohort studies for developmental internalization (P6, P15); historical comparison for buffering effects (P14); behavioral measurement for platform-mediated decision latency (P9). The theory is not the property of any one methodological tradition.



## 3. Core Theoretical Model

### 3.1 The Core Generative Mechanism (CGM)

We state the mechanism in compact form, then unpack it.


CGM. Functionally differentiated subsystems, each operating under a distinctive binary code and a set of programs, engage in selective and asymmetric structural coupling through identifiable communication channels. This coupling produces, simultaneously and as joint outputs of the same operation: (i) coordination across subsystems sufficient for joint operation, and (ii) tension between codes that propagates through the channels. Both outputs feed back onto individual cognition, through internalization processes whose rate is a function of exposure frequency, cognitive load, reinforcement schedule, and developmental window, and onto small-group dynamics, through situationally triggered switching among four relational logics. The macro-level properties of the system — coordination, volatility, contagion, norm cascades, and autonomy erosion — are weakly emergent from the joint operation of these processes, given the topology and tightness of the coupling matrix and the buffering capacity of the relevant institutional channels.


Five components of the CGM require unpacking.


Component 1: Differentiated subsystems with codes and programs. Following Luhmann (1995, 2012), each subsystem reduces the complexity of its environment by applying a binary code: legal/illegal, true/false, profit/loss, governing/opposition, sacred/profane, beautiful/banal, news/non-news. The code does not by itself generate decisions; decisions are generated by programs — specific rules, methods, statutes, budgets, and procedures — that translate the code into operational outputs. Programs differ across cases (criminal procedure vs. contract law; experimental method vs. observational study; monetary policy vs. fiscal policy), but they all serve the function of applying the code.


Component 2: Selective and asymmetric coupling. Subsystems are not isolated. They are coupled through specifiable channels: the legal and economic subsystems are coupled through the contract, the property registry, and the limited-liability corporation; the political and economic subsystems through taxation, fiscal policy, and central banking; the scientific and political through research funding agencies; the scientific and economic through patent law; the mediatic and political through electoral coverage and platform algorithms. We call the coupling selective because not every output of one subsystem reaches every other (most legal decisions are not economically salient; most scientific findings are not politically actionable), and asymmetric because the rate at which subsystem A's outputs influence B is generally not equal to the rate at which B's outputs influence A. Asymmetry, formalized as a non-symmetric coupling matrix Γ in §4.3, is essential to the theory: it is what makes colonization possible.


Component 3: Joint outputs — coordination and tension. A single contract simultaneously coordinates legal and economic subsystems (it makes joint operation possible) and produces tension between them (the legal subsystem's conception of a binding promise is not identical to the economic subsystem's conception of an enforceable claim). Coordination and tension are not separate processes in sequence; they are simultaneous outputs of the same coupling event. This dual character is what permits both the stability and the fragility of differentiated societies.


Component 4: Feedback to individuals via internalization. The outputs of subsystems do not remain at the institutional level. Through repeated exposure — schooling, news consumption, contractual interaction, religious participation, courtroom observation, scientific training, platform-mediated content — individuals internalize the codes and the programs in the form of dispositions, expectations, and category systems (Vygotsky, 1978; Berger and Luckmann, 1966; DiMaggio, 1997). Internalization is not uniform: it is faster at developmental sensitive periods, faster under high reinforcement, slower under high cognitive load, and selectively accelerated for codes whose channels are dense in the individual's environment.


Component 5: Feedback to groups via situational logic switching. Small groups (households, work teams, friend groups, deliberative bodies of fewer than approximately 150 members) operate under one or more of Fiske's (1991, 1992) four relational models: Communal Sharing (CS), Authority Ranking (AR), Equality Matching (EM), and Market Pricing (MP). Groups do not select these logics arbitrarily; they switch among them in response to situational cues (resource scarcity, external threat, ideological homogeneity, task interdependence) which themselves are functions of the outputs of the institutional subsystems above them. Logic switching is the channel through which subsystem operations reach the level of face-to-face interaction.


The remainder of §3 derives the four cross-level loops from the CGM as Coleman-boat instantiations. Before turning to the loops, we make explicit the locus where they meet.

#### 3.1.1 The ego as the locus where the loops meet

The CGM is stated at the level of subsystem coupling because that is the level at which its formal regularities are tractable. But the loops do not operate in an empty intersubjective space: they meet, biographically and materially, in the individual self — the ego. Every operation of Loop 1 (internalization) terminates in an ego; every operation of Loop 2 (aggregation) originates in egos; the situational cues that trigger Loop 3's small-group logic switches are perceived and weighted by egos; the second-order observations of Loop 4 are produced by ego-bearing social scientists and are received by ego-bearing readers. The ego is not an additional level above or below the subsystems; it is the substrate on which the subsystems' operations register and from which their inputs are drawn. We follow the original informal sketch in giving the ego this anchor position, while declining to treat it as the generative element of the theory.


Composition of the ego. Four interacting layers, treated as an integrative processing complex rather than as a list (extended in §3.2 and §4.2):


Biological substrate. From subcellular regulation through neural circuitry to the autonomic and endocrine systems, the biological layer constrains throughput, energy availability, and plasticity. It does not, by itself, determine the content of experience; it sets the bandwidth in which content is generated.

Cognitive layer. Perception, attention, memory, language, and thought, organized along the System 1 / System 2 distinction (Kahneman, 2011). System 1 supplies fast automatized output from internalized categories; System 2 supplies slow, effortful evaluation of those categories under sufficient resources and latency.

Affective layer. The full Plutchik-Ekman-Barrett spectrum (joy, sadness, anger, fear, disgust, surprise, contempt, trust, anticipation, and the complex emotions — guilt, pride, shame, nostalgia — that are constructed from these). The original informal framing reduced this spectrum to a single axis of love versus fear. We retain that simplification as a useful valence axis capturing the most fundamental approach/avoidance dimension of motivated cognition: many institutional translations (see §3.4) become legible only when one notes that the institutions are, at scale, processing the population's aggregated love-side or fear-side affect into operational outputs (national security being the most consequential institutional translation of population-level fear; collective social insurance, of population-level love or solidarity). The full spectrum, however, remains the empirically correct apparatus for individual-level emotional analysis.

Motivational layer. A hierarchy organized around survival (physiological and physical safety), recognition and status (acceptance and standing within a reference group), and meaning (purpose, self-actualization). The original sketch correctly highlighted survival, recognition, and status as the chief motivational anchors. Following Kenrick et al. (2010), we reject any strict bottom-up sequence: motivational priorities reorder according to context, life stage, and threat. A satiated but threatened ego may rank survival first; a hungry but secure one, belonging.


Why these four interact rather than aggregate. The integrative claim is that the four layers are not independent. A cultural category enters via cognition, is tagged with affective valence through reinforcement, is incorporated into the motivational hierarchy as a goal or constraint, and is constrained by biological substrate. To understand any individual decision is to understand the joint state of all four. To understand any aggregate institutional outcome is to understand how individual decisions, generated under specific joint states across a population, propagate through Loop 2.


Where the ego sits in the loops. Loop 1 deposits internalized categories into the cognitive layer (with affective tagging and motivational integration during deposition). Loop 2 draws on the resulting dispositions when individual decisions are aggregated through markets, elections, opinion formation, and other channels. Loop 3 reaches the ego only indirectly — through the institutional artifacts (contracts, taxes, platforms) that the ego encounters in everyday life. Loop 4 reaches the ego both directly (through education in social-scientific frameworks) and indirectly (through institutional reforms shaped by such frameworks). The ego is therefore the biographical unit of the theory; the subsystems are the systemic units. Both descriptions are required; neither is reducible to the other.

### 3.2 Loop 1 — Internalization (macro → micro): The Coleman boat downward

The first loop is the macro-to-micro arc of the Coleman (1990) diagram, instantiated under the CGM.


Actors and entities. The macro side: the seven subsystems and their programs. The micro side: individual agents with cognitive, emotional, motivational, and biological states.


Channels. Schooling (program: curriculum); news and platform media (program: editorial selection and algorithmic prioritization); contractual interaction (program: contract law); courtroom and police interaction (program: criminal and civil procedure); religious participation (program: liturgy, doctrine, ritual); scientific training (program: peer review, replication norms); aesthetic exposure (program: canon, criticism, gallery and platform curation); workplace participation (program: employment law and corporate procedure).


Mechanism. Internalization in the Vygotskian-Brunerian sense: external symbolic-categorical structures, encountered repeatedly through these channels, come to constitute the internal structures through which the individual perceives, evaluates, and decides. Crucially, this process operates before the individual is capable of reflective evaluation of the categories themselves; categorization precedes critique (Vygotsky, 1978; Bruner, 1990; Geertz, 1973; DiMaggio, 1997). The four micro-level layers introduced in §3.1.1 — biological substrate, dual-process cognition (Kahneman, 2011), affective spectrum (Ekman, 1992; Plutchik, 2001; Barrett, 2017) including the foundational love/fear (approach/avoidance) valence axis, and motivational hierarchy anchored in survival, recognition, and status (Maslow, 1943; updated in Kenrick et al., 2010) — are not a list but an interactive processing complex: cultural categories enter through cognition (System 2 effortful learning, then System 1 automatization), are tagged with affective valence through reinforcement (categories repeatedly paired with reward or threat acquire correspondingly approach- or avoidance-loaded valence), are integrated into the motivational hierarchy as goals or constraints (categories that promise recognition and status are more readily internalized than categories without motivational anchoring), and are constrained by biological substrate (energy, neuroplasticity, age). Internalization that recruits all four layers — cognitive comprehension, affective tagging, motivational anchoring, and biologically appropriate timing — is the deepest and most durable; internalization that operates on cognition alone, without affective or motivational engagement, is fragile.


Temporal dynamics. Internalization is fastest during developmental sensitive periods: roughly ages 0–7 for syntactic and basic categorical structures, roughly ages 12–25 for institutional logics and abstract codes (Werker and Hensch, 2015; on the second window, Steinberg, 2014; Sapolsky, 2017). It is slow, costly, and incomplete in adulthood; resocialization in late adulthood almost always retains residues of prior internalization.


Conditions of amplification. Loop 1 amplifies when (i) exposure frequency is high, (ii) reinforcement is consistent (low signal noise), (iii) cognitive load is moderate (enough resources for learning, not so much that other tasks dominate), and (iv) the individual is within a sensitive period.


Conditions of dampening or breakage. Loop 1 is dampened or broken when exposure to a code is sparse, when codes are inconsistent (the school teaches one moral framework, the family another, the platform a third), or when the channels themselves are obstructed (illiteracy preventing access to legal categories; geographic isolation from monetary economy).


The Coleman boat. Macro: subsystem programs and codes. Bridge down: exposure through the channels. Micro: internalized categories, dispositions, and expectations. Bridge up: individual decisions made under those dispositions. Macro again: aggregate behavior that re-stabilizes (or destabilizes) the subsystem programs.

### 3.3 Loop 2 — Aggregation (micro → macro): The Coleman boat upward

The second loop is the micro-to-macro arc.


Actors and entities. Individuals (with internalized dispositions from Loop 1, situational and biological inputs) and small groups; on the macro side, subsystem programs.


Channels. Markets (aggregating consumer choices into prices); elections (aggregating individual preferences into political mandates); reproduction and migration (aggregating fertility and movement choices into demographic and labor-market shifts); informal opinion formation (aggregating individual judgments into public opinion as measured by polls, social-media trends, and electoral signals); scientific publication (aggregating individual results into bodies of established knowledge); courts (aggregating disputes into precedent).


Mechanism. Aggregation is rarely a simple sum. It depends on (i) the number of agents N, (ii) interaction density ρ, (iii) behavioral heterogeneity H, and (iv) the strength σ of relational coupling among agents. The aggregation function f(N, ρ, H, σ) takes very different forms across channels: it is approximately linear for some forms of public-opinion aggregation under standard polling conditions, but radically non-linear for opinion cascades on networked platforms (Centola, 2018; Watts, 2002), for financial-asset price formation under leverage, and for political mobilization under emotional contagion. Non-linearity is the source of the upward loop's most important property: small variations in micro-level inputs can produce categorical macro-level shifts.


Group-level logic switching as a sub-mechanism of aggregation. Loop 2 does not run directly from individual to system. It runs first through the small-group level, where individuals' internalized dispositions are filtered through a relational logic — CS, AR, EM, or MP — that is itself a function of situational cues (Fiske, 1991, 1992). The dynamics of logic switching, presented next, are therefore embedded inside Loop 2.


Observable markers of small-group micro-culture. Before turning to the formal switching dynamics, we note that the active relational logic in any small group is empirically tractable through a small number of concrete cultural markers, which jointly constitute what may be called the group's micro-culture: (i) what is funny — the humor norms of the group, encoding shared assumptions about what may be ridiculed and what is protected; (ii) what is forbidden — the speech and conduct prohibitions that demarcate insider from outsider; (iii) who leads — the implicit or explicit authority structure, including who initiates topics, whose interruptions are tolerated, whose proposals are adopted; (iv) how disagreement is handled — whether through hierarchical resolution (AR), consensus-seeking (CS), turn-taking (EM), or transactional negotiation (MP); (v) how new members are absorbed — whether through assimilation (CS), apprenticeship (AR), parity (EM), or contractual onboarding (MP). These markers, jointly, supply behaviorally codable indicators of the active logic. They are also the medium through which the ego's foundational motivation for recognition and status within the reference group expresses itself empirically: the ego seeks validation precisely along the dimensions encoded in these markers, and the channel through which the marker-system is transmitted, contested, and updated is language — which is, accordingly, neither incidental nor a separable variable but the constitutive medium of small-group operation.


Logic switching dynamics. We reconstruct Fiske's typology as a state machine. Let S ∈ {CS, AR, EM, MP} be the active logic in a group at time t. Let u be a cue vector with components for resource scarcity, external threat, ideological homogeneity, and task interdependence. Each logic has a characteristic activation profile in u space:


Communal Sharing (CS) is activated by high ideological homogeneity, high external threat, and low task differentiation. Empirically: kin groups, religious communities under siege, military units in combat, mutual-aid societies.

Authority Ranking (AR) is activated by high task interdependence, asymmetric expertise or risk, and large group size. Empirically: military command, surgical teams, hierarchical workplaces. Expectation States Theory (Berger et al., 1977) supplies the sub-mechanism: task-relevant status cues generate expectations that crystallize into stable hierarchies even in initially undifferentiated groups.

Equality Matching (EM) is activated by moderate group size, repeated interaction, and absence of formal exchange media. Empirically: turn-taking norms, rotating chairs, gift exchange in Maussian (1925) reciprocity.

Market Pricing (MP) is activated by the presence of monetary or quasi-monetary exchange media, by interaction across group boundaries (especially with strangers), and by acute resource scarcity that breaks down trust-based logics.


Reconciliation of conflicting logics. When situational cues activate multiple logics simultaneously, the group must reconcile. Three sub-mechanisms of reconciliation are observed: (a) status arbitration (a high-status member's preferred logic prevails), drawing on Social Identity Theory (Tajfel and Turner, 1979) and Expectation States dynamics; (b) narrative reframing (the situation is recategorized so that a single logic becomes appropriate, e.g., a workplace social event is reframed as either "team bonding" — CS — or "networking" — MP); (c) logic stratification (different aspects of the same interaction are assigned to different logics, e.g., the family business runs MP for transactions with non-kin and CS within kin). Which sub-mechanism is selected is itself a function of the dominant subsystem code in the surrounding institutional environment: Loop 1 supplies the priors that bias reconciliation.


Differential predictions. Under conditions of externally imposed resource scarcity, MP displaces EM in groups whose pre-existing norms favor equality (P1 in §5). Under conditions of acute external threat plus ideological homogeneity, CS displaces both AR and MP, even where previously stable hierarchies existed (P12).


Coleman boat closure. The macro inputs (subsystem codes, situational cues) bias group-level logic activation; the active logic shapes individual decision; the aggregated decisions feed back as macro inputs (votes, prices, scientific outputs).

### 3.4 Loop 3 — Horizontal Coupling (meso → meso): Coordination, tension, and colonization

The third loop runs across subsystems at the same hierarchical level.


Actors and entities. Subsystems and the institutional bridges between them.


Channels. Identified by inspection of which institutional artifacts simultaneously belong to two or more subsystems. The contract belongs jointly to the legal and economic subsystems (a contract is both a legally enforceable instrument and an economic transaction). Tax law belongs jointly to the legal, political, and economic subsystems. Research grants belong jointly to the political (allocator) and the scientific (recipient). Patent law couples the scientific to the economic. Electoral law couples the political to the legal. Platform algorithms couple the mediatic to the economic and the political. Religious endowments and tax exemptions couple the religious to the legal and the economic.


Mechanism: structural coupling, formalized. We represent the cross-subsystem coupling as a directed weighted graph with adjacency matrix Γ. The entry γ_{ij} measures the rate at which outputs of subsystem i perturb the operations of subsystem j, given a unit perturbation in i. Coupling is selective (most γ_{ij} are zero or near-zero), asymmetric (γ_{ij} ≠ γ_{ji} in general), and time-varying (γ_{ij} can grow under technological or institutional change). Three regimes are distinguishable.


Sparse coupling regime (most γ_{ij} ≈ 0). Subsystems operate effectively in isolation. The system is robust to local shocks but slow to coordinate. Pre-modern stratified societies approximate this regime within most domains.

Moderate coupling regime (γ_{ij} > 0 for the major institutional bridges; row sums of Γ moderate). The defining condition of mature differentiated modernity. Coordination is achieved at acceptable systemic risk; subsystem autonomy is preserved through buffering institutions.

Tight coupling regime (γ_{ij} large; row sums approach a critical value τ_c). Contagion across subsystems becomes the dominant dynamic. Local perturbations propagate before buffering can absorb them. The 2008 financial-political crisis, the COVID-19 economic-political-mediatic synchronization, and the platform-era convergence of mediatic and political dynamics are all instances. We predict that crisis frequency and synchronization rise super-linearly as Γ approaches τ_c (P3, P7).


Colonization. Subsystem A is said to colonize subsystem B when the operations of B come, over time, to be governed by A's code rather than B's own. Colonization is a long-run, asymmetric outcome of coupling under power asymmetry. We do not assume that subsystems are equal in power: the coupling matrix Γ is asymmetric, and so are the institutional resources subsystems can deploy to defend their codes against external encroachment. The economic colonization of education, in which the educational subsystem's program comes to be evaluated in terms of profit/loss-equivalent metrics (return on investment, employer demand, "human capital"), is the canonical contemporary example (Slaughter and Rhoades, 2004; Brown, 2015). Indicators of colonization (operationalized in §4.1) include (i) terminology drift in institutional discourse measurable by NLP on legislative, regulatory, and curricular texts (P4); (ii) personnel exchange across institutional boundaries, measurable as transitions of senior personnel between subsystems; (iii) regulatory capture metrics from the political-economy literature.


Power asymmetry, theorized. We reject the implicit symmetry of the original framework's claim of equal autonomy. Subsystem power is a function of (i) resource control — direct command over scarce resources whose consumption other subsystems require (the economic subsystem controls capital, the political subsystem controls coercion, the mediatic subsystem controls attention); (ii) infrastructural reach — the breadth of the channels through which the subsystem's code can be transmitted (post-platform mediatic reach is far greater than pre-platform); and (iii) temporal speed — the rate at which the subsystem can produce decisions (algorithmic mediatic decisions: milliseconds; financial decisions: seconds; political decisions: months; legal decisions: months to years; scientific decisions: years). Asymmetric speed creates a structural advantage for fast subsystems: by the time slower subsystems can respond, the fast subsystem has already shifted its outputs. This is a major source of contemporary instability.


Coleman boat closure for Loop 3. This loop is the meso–meso analog: the bridge runs not through individuals but through institutional artifacts (the contract, the tax form, the platform feed, the research grant). Individuals participate in Loop 3 by virtue of their roles within institutions, but the loop's dynamics are largely inter-institutional.

#### 3.4.1 The aggregate institutional layer as a Social Operating System

The set of differentiated subsystems, taken together with their coupling matrix Γ, constitutes what we will call — adopting a useful framing from the original informal sketch — the Social Operating System (Social-OS) of a community, city, or nation. The metaphor is informative if treated with care. An operating system in the technical sense supplies a stable abstraction layer over heterogeneous lower-level resources, mediates between concurrent processes, allocates scarce resources according to procedural rules, and maintains identity over time despite turnover in the entities running on it. The Social-OS does the analogous work at the social scale: it supplies a stable categorical layer over heterogeneous individual egos and small groups, mediates between subsystems' concurrent operations through structural coupling, allocates resources through political and economic programs, and maintains continuity of categorical content across generations through Loop 1 internalization. Three theoretical claims about the Social-OS deserve foregrounding.


Claim 1: ideology and religion as the categorical glue. A defining problem of large-scale societies is how millions of egos who will never interact face-to-face can coordinate at all. The Fiskean relational logics of §3.3 are designed for groups within Dunbar's (1992) limit (~150) and break down at larger scales: I cannot maintain Communal Sharing with strangers, nor sustain Equality Matching with millions, nor know enough about an out-of-sight other to enter Authority Ranking with them. The functional answer that emerged historically is the abstract object of identification — the nation, the faith, the ideological community, the platform-enabled imagined community (Anderson, 1983) — which the ego is taught to identify with and toward which the ego's affective load (especially on the love side of the love/fear valence axis) is redirected. The original informal sketch captures this exactly: "instead of loving my friend, I learn to love my country, or my idea." Ideology and religion thus operate not (only) as belief systems but as categorical scaffolding that allows Fiske-style logics to be applied vicariously, through identification with an abstract object, to populations far exceeding the cognitive limits on direct relational logic. This is why religious participation, national ritual, and ideological speech have such disproportionate institutional consequences: they sustain the categorical scaffolding without which large-scale coordination would dissolve back into the limits of face-to-face interaction.


Claim 2: the affect-to-institution translation table. A central mechanism of the Social-OS is the translation of population-level affective states into institutional categories. The original informal sketch identifies two of the most consequential translations directly: altruism becomes tax (collective social insurance is the institutional translation of the population's love-side, prosocial affect into a routinized economic-political program), and fear becomes national security (the population's fear-side affect is translated into institutional capacity for coercion, surveillance, and external defense). Several others can be added in the same form. We summarize them in Table 1A.


**Table 1A. Affect-to-institution translation under the Social-OS.**



The translation, in each case, is not a metaphor: it is a literal institutional mechanism by which an affective state, when distributed across a sufficiently large population, is processed by the relevant subsystem according to its code into a routinized output. This is why the original informal sketch's observation that "the law replaces personal revenge with cold and calculated order" is not merely a colorful description but a precise statement of one row in the translation table: the legal subsystem's distinctive contribution is the substitution of programmatic adjudication for affective retaliation, achieved by routing the affective input through procedures whose code (legal/illegal) is indifferent to the litigant's emotional state. Similarly, the original sketch's framing of money as "a religion of trust" captures the fact that monetary value is sustained by population-level confidence in a categorical system whose operational substrate (numbers in databases) has no intrinsic worth: the economic subsystem performs, at scale, the same coordinative function for trust that organized religion performs for reverence.


Claim 3: legitimation in the language of the common good. A persistent feature of political discourse in differentiated societies is that decisions made under the political subsystem's distinctive code (governing/opposition; effectively, the ranking of political coalitions) are systematically presented in the language of the common good rather than in the code's own terms. The original informal sketch puts this directly: political decisions are still driven by the status and ego of leaders, "but wrapped in the language of the common good." The theory does not regard this rhetorical wrapping as cynical or anomalous; it is a structural requirement. Because the political subsystem must coordinate populations far exceeding any face-to-face group, its decisions must be presented in categories that the population's internalized dispositions (Loop 1) can register as legitimate. The categories of the common good — fairness, security, freedom, prosperity — are precisely those that the affect-to-institution translation table already supplies. Legitimation rhetoric is, accordingly, a reverse-direction Loop 1 operation: the political subsystem encodes its outputs in terms of the categories that Loop 1 has already deposited in the population's cognition, securing uptake and compliance. When the rhetorical wrapping fails to match the substantive output (when, for instance, decisions framed as "the common good" are perceived as benefiting only a faction), the resulting legitimacy crisis is one of the most consistent precursors of political instability.


The Social-OS framing thus integrates three distinctive observations from the original informal sketch — ideology/religion as glue, affect-to-institution translation, and common-good legitimation rhetoric — as substantive consequences of the CGM operating at population scale.

### 3.5 Loop 4 — Self-Reflection (the system observing itself)

The fourth loop is distinctive: it is the system's second-order observation of itself, in Luhmann's (1995) sense.


Actors and entities. The social-scientific subsystem (a sub-component of the scientific subsystem) and the entities that consume its outputs (policy makers, journalists, educators, platforms, the general public).


Channels. Academic publication; popular non-fiction and journalism summarizing social-scientific work; policy advice and "evidence-based" governance; curricular incorporation of social-scientific frameworks into education at every level.


Mechanism: performativity. When social-scientific knowledge is incorporated into the entities it describes, it can change those entities (Merton, 1948; Hacking, 1995; MacKenzie, 2006; Callon, 1998). Three modes are observable:


Looping effects (Hacking): the categories used to describe social actors are taken up by those actors and become part of their self-understanding, changing their behavior, which in turn changes the empirical phenomenon the categories were originally meant to describe.

Performative theory uptake (MacKenzie): when economic actors are trained in rational-choice or option-pricing theory, their behavior moves toward the model, and the model's empirical accuracy increases as a result of its having been taught.

Reflexive policy (Beck, 1992; Giddens, 1991): policy makers act on social-scientific predictions, altering the conditions on which the predictions were based.


Temporal dynamics. Loop 4 runs slowly relative to the other three. Knowledge production has a lag of years; uptake into education has a further lag of years to decades; behavioral effect after uptake has its own lag. Total round-trip time is on the order of a decade or more. This slowness is one of the system's most important buffering mechanisms: it provides time for course correction. Conversely, when Loop 4 is accelerated — for example, by platform-era data feedback that allows real-time incorporation of behavioral measurements into platform design — the buffering disappears (P9).


Coleman boat closure. The macro outputs of Loop 4 are revised programs of the social-scientific subsystem, which then feed back into the educational and policy programs that operate in Loops 1, 2, and 3. The micro mediation is the individual social scientist whose work, training, and incentives are shaped by the very system they study.

### 3.6 Derived case 1: Surveillance capitalism

Surveillance capitalism (Zuboff, 2019) is not introduced here as a metaphor or as a contemporary illustration. It is derived from the CGM as the predicted outcome of a specific configuration of the four loops.


Configuration. Consider a technological-mediatic platform that (a) accelerates Loop 1 to milliseconds (algorithmic content selection produces continuous, individualized exposure to subsystem codes at frequencies orders of magnitude greater than previous media), (b) accelerates Loop 2 (aggregated user behavior is computed as input to the platform's optimization in real time), (c) accelerates Loop 3 (the platform serves as a coupling channel between mediatic, economic, and political subsystems with response times in seconds to hours), and (d) compresses Loop 4 to the same temporal scale (the platform's own observation of user behavior is used to redesign the platform within the same operational cycle).


Predicted outcomes.


Erosion of reflective autonomy — the predictive anticipation of the ego. Reflective deliberation requires latency: estimates from cognitive psychology place deliberative processing at a minimum of approximately 500 milliseconds for habitual override and 3–5 seconds for substantive deliberation (Evans and Stanovich, 2013). Platform-mediated decision environments that close the user-decision-feedback loop below these thresholds reduce the share of decisions in which Loop 1 internalized dispositions can be reflectively interrogated by System 2 cognition before action. The original informal sketch named this outcome with precision: the platform comes to predict the next step of the ego before the ego itself has thought of it. This is not a poetic exaggeration but a literal description of the operational state achieved when the platform's predictive accuracy on the user's next action exceeds the user's own reflective bandwidth. It is the operational meaning of "autonomy erosion." It is measurable along two complementary dimensions: (a) decision latency in platform-mediated environments — how long the user takes between presentation of a choice and selection — and (b) accuracy of platform predictions of subsequent user behavior — how often the platform's anticipated next action matches the action the user takes. The theoretical prediction is in P9: when (a) declines and (b) rises in tandem, the predictive-anticipation regime has been entered.

Asymmetry of information. The platform observes and aggregates user behavior at scale; users do not observe the platform's aggregated patterns. This asymmetry is not incidental but is a direct consequence of the coupling configuration: the platform sits at the convergence of Loops 1–4 and is uniquely positioned to extract their joint signal.

Subsystem colonization vector. The platform, situated in the mediatic subsystem but operationally driven by the economic subsystem's profit/loss code (because platform revenue depends on attention monetization), provides a fast colonization channel from the economic to the mediatic, and from the mediatic into political and aesthetic subsystems. Predicted indicators: rising share of mediatic content selected by economic-code-driven algorithmic systems; declining share of editorial-mediatic-code curation; corresponding measurable changes in political discourse (hyper-virality of high-arousal political content) and in aesthetic markets (algorithmically optimized cultural production).


The point is methodological: surveillance capitalism is not an additional phenomenon the theory must explain in an ad hoc fashion. It is the predicted outcome of a particular configuration of coupling and exposure, derivable from the CGM.

### 3.7 Global-scale emergence: the modern Leviathan

We now address the macro-most level: the globally coupled multi-subsystem network. We follow the original informal sketch in calling this configuration the modern Leviathan — adopting the term not as Hobbes's anthropomorphic sovereign but as a heuristic name for what is, technically, a globally coupled multi-system network in which the four loops have been accelerated to the point that no single subsystem can operate independently of the others. The technical and the heuristic terms are, throughout this paper, interchangeable; we retain both because the heuristic captures something the technical term tends to obscure: the experiential character of living within such a system, in which individual decisions, collective outcomes, and institutional reforms increasingly behave as moves within a single interlocked dynamic rather than as independent actions in separate domains.


Definition of emergence at this level. Following the weak-emergence commitment of §2.3, the global system has properties that are computable from, but not predictable in closed form by, the dynamics of its components. Three such properties are theoretically derivable and empirically measurable.


Synchronization volatility. Defined as the cross-subsystem correlation of output volatility (e.g., correlation of financial-market volatility with political-system volatility with media-attention volatility), measurable on rolling windows. Predicted to rise non-linearly as the coupling matrix Γ approaches τ_c.

Norm cascade frequency. Defined as the rate at which previously stable normative consensuses in one subsystem rapidly shift due to propagation from another (Centola, 2018; Sunstein, 2009). Predicted to rise with mediatic-channel speed and with cross-subsystem coupling tightness.

Reflective-autonomy index. Aggregated measure of decision latency and prediction-by-platform accuracy across the population; predicted to decline as Loop 4 compression increases.


The canonical Leviathan loop. The original informal sketch identifies a specific recurrent cycle that the present theory recovers as the most consequential of the system's emergent loops: money → technology → ideology → education → ego → system → money. We unpack the cycle in the theory's own terms.


Money → technology. The economic subsystem, operating under its profit/loss code, allocates capital to technological development whose return is measured in economic terms. Technologies whose deployment promises monetizable returns are funded preferentially; technologies whose returns are diffuse, slow, or non-monetizable are systematically under-funded.

Technology → ideology. Deployed technologies — especially mediatic and platform technologies — reshape the channels through which the population's exposure to ideological content is constituted. The shift from broadcast media to algorithmically curated platforms is the canonical contemporary instance: it does not merely change the speed of ideological transmission but changes the selection criteria, favoring high-arousal, high-engagement content over content selected by editorial-mediatic codes.

Ideology → education. Educational institutions, themselves subject to political and economic pressures, incorporate ideological content into their programs — through curriculum design, through the categorical frameworks taught as common sense, and through the meta-level skills (or lack thereof) cultivated in students. The resulting cognitive equipment of the next generation is shaped accordingly.

Education → ego. Through Loop 1 internalization, especially during the developmental sensitive periods identified in §3.2, the categorical frameworks delivered through education become constitutive of the next generation's egos: their default cognitive categories, their affective taggings, their motivational priorities, and the specific calibration of their love/fear valence axis are all shaped by what education has deposited in them.

Ego → system. Through Loop 2 aggregation — through markets, elections, opinion formation, reproduction, scientific publication, and institutional participation — the resulting egos collectively constitute the next-period inputs to the subsystems whose outputs initiated the cycle.

System → money. The aggregated system outputs, mediated through political and economic institutions, redirect the next round of capital allocation, completing the loop.


The cycle is not a metaphorical one; each arrow corresponds to one of the formal loops or sub-mechanisms specified in §3.2–§3.6. It can be made fully formal by tracing it through the equation system of §4.3: the path from a capital-allocation decision in subsystem i = economic, through a technology-output update, a mediatic-exposure update, a Loop 1 internalization update for the next-cohort egos, a Loop 2 aggregation, and a return to subsystem i's next-period inputs, defines a closed orbit through state space whose period and amplitude are functions of the coupling matrix Γ and the loop-rate parameters. The Leviathan loop is, accordingly, the canonical closed-orbit trajectory of the system, and its tightness is a primary indicator of how much the system has consolidated into the regime in which individual reflective autonomy approaches its lower bound.


Distinguishing theoretical from empirical claims. The original framework referred to "the global system of 2026" as if describing an empirical state. The present revision treats any specific claim about a calendar year as a theoretically derived scenario under stated assumptions: namely, that the trajectories of platform-channel speed, cross-subsystem coupling, and Loop 4 compression that have been documented from approximately 2010 onward continue at rates consistent with their observed first-derivative through 2024, and that no major institutional buffering is introduced. Under those stated assumptions, the theory predicts (a) a continuing rise in synchronization volatility, (b) a continuing rise in norm-cascade frequency, (c) a continuing decline in the reflective-autonomy index, and (d) a continuing tightening of the Leviathan loop's closed orbit. Each of these is, in principle, empirically tractable; each is, in principle, falsifiable. The label "scenario," not "description," is essential to honest theorizing.



## 4. Operationalization and Formalization

### 4.1 Concept Operationalization Table

For each central concept of the theory, we provide a nominal definition (what the concept is), an operational definition (how it is to be measured), candidate empirical indicators, and, where appropriate, threshold or phase-transition values that distinguish qualitatively different regimes.


**Table 1. Operationalization of central concepts**


### 4.2 The micro-level integrative model

We unify the four micro-level layers — biological, cognitive, emotional, motivational — as an interactive processing complex governed by the following:


Cognitive throughput is bounded by the biological substrate (energy availability, working-memory capacity, age-conditioned plasticity).

System 1 processes (Kahneman, 2011) operate on internalized categories from Loop 1; their output dominates when cognitive load is high or when latency is below the deliberative threshold.

System 2 processes can override System 1 only when sufficient attentional resources are available and latency permits; deliberation is slow and effortful.

Affective processes (in the Plutchik-Barrett-Ekman tradition) modulate both: high-arousal states bias toward System 1; specific affective states (anxiety, anger, disgust) bias toward specific category invocations (Lerner et al., 2015). The full spectrum reduces, at the most aggregated level, to the love/fear valence axis introduced in §3.1.1: approach-side affect (love, trust, anticipation, joy) and avoidance-side affect (fear, anger, disgust, sadness). The reduction is lossy at the individual level — guilt, pride, and the other complex emotions cannot be cleanly placed on a single axis — but is informative at the population level, where the affect-to-institution translation table of §3.4.1 operates predominantly along this axis.

Motivational hierarchy does not unfold strictly bottom-up (against simplistic Maslow). Per Kenrick et al. (2010) and updated motivational research, motivational priorities reorder according to context, life stage, and threat: a hungry but secure individual may pursue belonging over food; a satiated but threatened individual reverses. The three primary anchors — survival, recognition, and status — are present across all reorderings; what varies is their relative weighting. Recognition and status anchors are the principal channel through which small-group dynamics (§3.3) drive individual behavior, since they are the dimensions along which the group's micro-cultural markers (what is funny, what is forbidden, who leads) supply or withhold validation.


The empirical hypothesis derived from this model is P2: cross-cultural variance is greater for "complex" emotions whose generation depends heavily on internalized categorical structures (guilt, pride, shame, nostalgia) than for "basic" emotions whose generation involves more direct biological substrate (fear, surprise, disgust). This hypothesis is testable using existing cross-cultural emotion-research methodologies and provides a falsifier for the priority claim of Loop 1 internalization for complex emotional content.

### 4.3 Formal core: the equation system

We provide a system of difference equations that captures the four loops as derived from the CGM. Indices: i, j denote subsystems (i, j ∈ {1, …, 7}); k denotes individuals; g denotes groups.


Loop 1: Internalization. Internalization score I_{k,i,t} of individual k for subsystem i at time t:


I_{k,i,t+1} = I_{k,i,t} + α · w(d_k) · E_{k,i,t} · r_{k,i,t} · (1 / (1 + c_{k,t})) · (I_max,i − I_{k,i,t})


where α is a learning-rate constant; w(d_k) is a developmental-window weighting (peaks during sensitive periods); E_{k,i,t} is exposure frequency to subsystem i's code; r_{k,i,t} is reinforcement consistency; c_{k,t} is cognitive load; I_max,i is the saturation level. The (I_max − I) term ensures asymptotic approach to saturation rather than unbounded growth.


Loop 2: Aggregation. Macro output O_{i,t} of subsystem i:


O_{i,t} = f_i ( N, ρ, H, σ, {decisions of agents k mediated by their group's active logic S_{g(k),t} }, {subsystem inputs from coupled subsystems j → i with weights γ_{ji}} )


where f_i is the subsystem-specific aggregation function. The dependence on the active group logic links the loop to the switching dynamics of §3.3.


Logic switching. Probability that group g's active logic at time t+1 is S given current cue vector u_{g,t}:


P(S_{g,t+1} = S | u_{g,t}) = exp(β · v_S · u_{g,t}) / Σ_{S'} exp(β · v_{S'} · u_{g,t})


a softmax over logic-specific cue sensitivity vectors v_S, with inverse temperature β controlling switching responsiveness. Reconciliation under multi-logic activation is modeled as biased toward the logic favored by the highest-status member (Expectation States) or by the surrounding subsystem's dominant code.


Loop 3: Cross-subsystem coupling. Coupling matrix update:


Γ_{t+1} = Γ_t + η · ΔΓ_t − μ · B_t


where ΔΓ_t reflects the formation of new institutional bridges, η is an adoption rate, B_t is the buffering capacity in place, and μ is the buffering effectiveness. The dynamics of subsystem outputs under coupling:


O_{i,t+1} = (1 − δ) O_{i,t} + δ Σ_j γ_{ji} O_{j,t} + ε_{i,t}


where δ is a coupling-influence rate and ε_{i,t} is exogenous noise/shock to subsystem i. The largest eigenvalue λ_max(Γ) determines whether perturbations damp or propagate; when λ_max approaches 1, the system enters the tight-coupling regime where local shocks become global.


Loop 4: Performative reflection. Knowledge-induced revision of programs:


Programs_{i,t+Δ} = Programs_{i,t} + φ · K_t · ψ_i


where K_t is the social-scientific knowledge stock at t, Δ is the uptake delay, φ is the uptake rate, and ψ_i is the subsystem-specific performativity factor. When Δ is large (slow Loop 4), the system has time for course correction; when Δ approaches the operating tempo of Loops 1–3, the buffering function of Loop 4 disappears.


The full equation system is computationally tractable and is the basis for the Agent-Based Model specified in Appendix B.

### 4.4 What the formalization buys us

The formalization is not decorative. It enables three things absent from the original framework: (a) threshold-based predictions, including the τ_c prediction for crisis synchronization (P3); (b) counterfactual analysis, by simulating the system with one or more loops severed (P5; P14); and (c) regime characterization, distinguishing the sparse, moderate, and tight coupling regimes by their distinct macro-dynamics. The price of formalization is the requirement to specify constants (α, β, η, δ, μ, φ) whose empirical values are not yet well-established. Calibration of these constants is itself a research program; we discuss it in §8.4.



## 5. Empirical Propositions

We now deduce sixteen directional, falsifiable propositions from the theory, each specifying independent variable(s), dependent variable(s), scope conditions, and a suggested empirical test. The first fifteen are tests of the theory's generative predictions; the sixteenth is the explicit falsification criterion.

### 5.1 Group-level propositions

P1. Resource-scarcity displacement of Equality Matching by Market Pricing. In small groups whose pre-existing dominant logic is Equality Matching, externally imposed resource scarcity exceeding 25% per-capita decline over six months will produce a measurable shift toward Market Pricing as the dominant logic, even where group ideology favors equality.


IV: per-capita resource decline (continuous).

DV: behavioral coding of group interactions for MP indicators (explicit pricing, transaction documentation, accounting language).

Scope: small groups (N ≤ ~50) under pre-shock EM dominance.

Test: longitudinal field studies of communities under economic shock; quasi-experimental analysis of cooperatives undergoing financial stress.


P8. Status-cue activation of Authority Ranking. In initially undifferentiated face-to-face groups under task-interdependent conditions, exposure to even minimal task-relevant status cues will reliably produce stable AR hierarchies within five interaction sequences. The hierarchy's correspondence to actual task ability rises over time but does not start at chance.


IV: presence and salience of task-relevant status cues.

DV: hierarchy stability and ability-correspondence over time.

Scope: face-to-face groups, task-interdependent conditions.

Test: laboratory experiments using standard Expectation States designs (Berger et al., 1977).


P12. Threat-plus-homogeneity activation of Communal Sharing. Under conditions of acute external threat plus high ideological homogeneity (≥0.8 on standard ideological homogeneity index), CS displaces both AR and MP, and group-internal hierarchy-salience drops, even where pre-existing norms favored hierarchy.


IV: external-threat salience × ideological-homogeneity index.

DV: behavioral indicators of CS (sharing without account-keeping; collective rather than individual referent).

Scope: groups with prior AR or MP dominance.

Test: ethnographic and survey research in religious communities under persecution; military units in active combat; comparison with control communities lacking threat or homogeneity.

### 5.2 Individual-level propositions

P2. Differential cross-cultural variance for complex vs. basic emotions. The cross-cultural variance of expression patterns for complex emotions (guilt, pride, shame, nostalgia) significantly exceeds that for basic emotions (fear, surprise, disgust).


IV: emotion type (complex vs. basic).

DV: cross-cultural variance of expression patterns and self-reported elicitation.

Scope: cultures along the continuum of WEIRD-to-non-WEIRD societies (Henrich et al., 2010).

Test: cross-cultural facial expression and self-report studies; meta-analysis of existing cross-cultural emotion data.


P6. Developmental-window dependence of internalization. Internalization of cultural-categorical structures occurs more rapidly and durably during the developmental sensitive periods (0–7 for syntactic/categorical; 12–25 for institutional logics) than after these periods. Adult resocialization retains identifiable residues of prior internalization.


IV: age at exposure.

DV: durability and depth of internalization, measured longitudinally.

Scope: cross-cultural migration and conversion contexts.

Test: longitudinal cohort studies of immigrant populations and religious converts.


P11. Code-switching overload and anomie. When individual exposure to multiple subsystem codes is high and frequency of code-switching exceeds a personal threshold, individuals exhibit measurable increases in anomie.


IV: number of distinct codes encountered per unit time × switching frequency.

DV: standard anomie scales (Srole, 1956; updated versions).

Scope: individuals operating across multiple subsystems professionally or socially.

Test: large-N survey research with media-and-environment exposure measurement.


P15. Asymmetry of Coleman-boat time constants. The macro→micro arc of the Coleman boat (internalization) operates with shorter time constants than the micro→macro arc (aggregation), creating systematic delay in democratic feedback. Specifically, individual disposition shifts in response to institutional change occur within months to years; aggregate behavioral change reaching institutional feedback occurs over years to decades.


IV: source (macro institution) and target (individual or institution).

DV: time constant of measurable change.

Scope: differentiated societies with active media and electoral channels.

Test: longitudinal political-attitude and policy-response time-series analysis.

### 5.3 System-level propositions

P3. Tight-coupling threshold for synchronized crises. When the cross-subsystem coupling matrix Γ has λ_max ≥ τ_c (estimated empirically in the range 0.6–0.8), the probability of synchronized crises propagating across financial, political, and mediatic subsystems within a 12-month window exceeds a baseline rate by ≥40%.


IV: λ_max(Γ).

DV: occurrence of multi-subsystem crisis events.

Scope: globally interconnected modern economies.

Test: longitudinal network analysis of crisis events from 1970 to present, with comparison of pre- and post-tightening periods.


P4. Subsystem colonization signatures. Subsystem colonization is detectable through (i) measurable terminology drift in the colonized subsystem's outputs toward the colonizer's code, (ii) increased personnel transitions across subsystem boundaries in one direction, and (iii) increased regulatory-capture indicators.


IVs: measurable colonizing pressure (resource asymmetry, regulatory access).

DVs: NLP terminology metrics, personnel metrics, capture indices.

Scope: subsystems under sustained asymmetric coupling.

Test: NLP analysis of legislative, regulatory, and curricular texts; biographical-data analysis of senior personnel; institutional-economics regulatory-capture metrics.


P5. Effects of severing the upward aggregation loop. In societies where Loop 2 (upward aggregation) is institutionally suppressed (e.g., authoritarian regimes with no electoral, market-pricing, or scientific feedback channels), measurable divergence between elite expectations and population behavior grows over time, manifested as increasing variance in policy effectiveness and increasing frequency of unanticipated mobilizations.


IV: Loop 2 suppression intensity (operationalized via standard regime-typology measures).

DV: divergence metrics; protest emergence frequency.

Scope: authoritarian and totalitarian regimes.

Test: case studies and time-series of authoritarian regimes; comparative panel analysis.


P7. Coupling speed and volatility. Increased cross-subsystem coupling speed (measured as time-to-information-propagation across a defined channel) correlates positively with systemic volatility (variance in subsystem outputs).


IV: coupling speed (continuous, channel-specific).

DV: subsystem output volatility (continuous).

Scope: post-1980 financialized economies; post-2010 platform-mediated mediatic environments.

Test: financial-network velocity analysis; platform-content propagation studies.


P10. Tight economy–politics coupling: stability vs. capture susceptibility. Tight coupling between economic and political subsystems reduces electoral volatility under stable conditions but increases susceptibility to systemic capture during crises.


IV: economy-politics coupling tightness.

DVs: electoral volatility (stable conditions); regulatory-capture indicators (crisis conditions).

Scope: developed mixed economies.

Test: comparative political-economy analysis across OECD countries 1990–2020.


P14. Buffering reduces contagion. Institutional buffer mechanisms — redundancy, regulatory firewalls, geographic diversification — reduce contagion propagation across coupled subsystems. The reduction is non-linear: small buffer additions to severely tight systems produce disproportionate stability gains.


IV: buffer mechanism presence and capacity.

DV: contagion propagation rates and amplitudes.

Scope: financial, public-health, and informational subsystems.

Test: comparative analysis of crisis impacts pre- and post-regulatory reforms (e.g., Glass-Steagall era vs. post-1999; Basel III impact).

### 5.4 Loop 4 and platform-era propositions

P9. Reflective-autonomy erosion under platform mediation. In choice environments where platform-mediated decision feedback closes Loops 1, 2, and 4 below the threshold of deliberative latency (~3 sec), the share of decisions in which Loop 1 dispositions are reflectively interrogated by System 2 cognition declines measurably; correspondingly, platform predictive accuracy of subsequent user behavior increases.


IV: platform feedback-loop closure speed.

DVs: decision latency; predictive accuracy of platform behavior models.

Scope: platform-mediated decision environments (content selection, e-commerce, political information).

Test: behavioral measurements of platform-mediated choice latency; analysis of platform predictive accuracy over time.


P13. Performative effects of social-scientific theory. Populations trained in specific social-scientific theories (e.g., rational-choice theory in economics) exhibit measurable behavioral shifts toward those theories' predictions in laboratory and field tasks, relative to matched untrained populations.


IV: training in a specific social-scientific theory.

DV: behavior in tasks where the theory makes predictions.

Scope: educational and professional training environments.

Test: cohort comparison of economics students vs. controls (Frank et al., 1993; Marwell and Ames, 1981; updated replications); analysis of option-pricing-theory-trained traders (MacKenzie, 2006).

### 5.5 The falsification test

P16 (Falsification criterion). Under conditions of (a) sustained increase in cross-subsystem coupling (measured by λ_max(Γ) or by direct channel-speed metrics), (b) absence or reduction of buffering mechanisms, and (c) maintenance of subsystem differentiation (no totalitarian collapse), if no increase in synchronization volatility, contagion-event frequency, or crisis-synchronization rate is observed over a 20-year period, the theory is fundamentally falsified.


This is not a vacuous test. The theory's central claim is that tight coupling without buffering produces increased systemic volatility and contagion. If twenty years of demonstrably tighter coupling and reduced buffering yielded no such increase, the CGM as formulated would be empirically wrong and would require either abandonment or substantial revision (e.g., introduction of unspecified compensating mechanisms whose absence in the current theory would be a major lacuna). We invite ongoing measurement against this criterion.


A complete proposition table with full IV/DV operationalizations and test designs is provided in Appendix C.



## 6. Comparison with Rival Theories

A theory's value depends in part on what it can do that established alternatives cannot. We compare the present theory systematically with four traditions: world-systems theory, neo-institutionalism, network/complexity science, and analytical sociology. For each, we identify (a) shared commitments, (b) where the present theory advances upon the rival, and (c) where the rival retains priority.

### 6.1 Wallerstein's world-systems theory

World-systems theory (Wallerstein, 1974, 1980, 1989, 2004) shares with the present theory a commitment to multi-level analysis of large-scale social systems, an emphasis on long-run dynamics, and a refusal to treat societies as bounded units explicable in isolation.


Where the present theory advances. Wallerstein's theory operates with a single dominant logic — capitalist accumulation in the world-economy — that subsumes political, cultural, and military dynamics. While powerful for explaining core-periphery relations, this monocentric architecture struggles to explain intra-core variation: why functionally differentiated subsystems within core states behave under codes that resist reduction to capital accumulation, why scientific or legal autonomy can be defended against economic colonization in some periods and not others, and why political dynamics in core states sometimes produce outcomes contrary to capital interests. The CGM provides a multi-code account in which capitalist logic (the economic subsystem) is one among several, and in which the conditions under which it does or does not colonize others are specifiable.


Where the rival retains priority. World-systems theory's account of long-run global core-periphery dynamics, of historical capitalist transitions across hegemonic powers, and of unequal exchange remains the more developed account of these specific phenomena. The present theory would benefit from incorporating world-systems insights into the cross-border dimensions of subsystem coupling — particularly how the global division of labor structures the asymmetry of economic-subsystem power across societies.

### 6.2 Neo-institutionalism (DiMaggio and Powell; Meyer and Rowan)

Sociological neo-institutionalism (Meyer and Rowan, 1977; DiMaggio and Powell, 1983; DiMaggio, 1997; Powell and DiMaggio, 1991) shares with the present theory an emphasis on how institutional rules and categories shape individual cognition and organizational behavior, on isomorphic pressures across organizational fields, and on the partial decoupling between formal structure and operational reality.


Where the present theory advances. Neo-institutionalism identifies isomorphism (coercive, mimetic, normative) as a process but is less specific about the cross-system dynamics that make some institutional fields more vulnerable to colonization by others. The CGM's formalization of asymmetric structural coupling (§3.4) supplies the missing micro-foundation: institutional fields are isomorphic to the codes of the subsystems whose coupling channels are densest in their environment. The CGM also predicts when isomorphism will break down (under sparse coupling) and when it will accelerate into colonization (under tight coupling without buffering). Neo-institutionalism's "decoupling" between formal and operational reality is recovered, in the present theory, as a buffering mechanism: organizations subject to multiple subsystem codes maintain operational autonomy by formal compliance to one while operating under another.


Where the rival retains priority. Neo-institutionalism's empirical work on organizational fields, on the diffusion of practices, and on the construction of new categories within fields is more developed empirically than the present theory's parallel claims. Future work should integrate the rich empirical neo-institutionalist literature on field dynamics with the cross-subsystem coupling matrix introduced here.

### 6.3 Network and complexity science (Barabási, Centola, Watts)

Network and complexity-science approaches to social systems (Barabási, 2002, 2016; Watts, 2002; Centola, 2018; Easley and Kleinberg, 2010) share with the present theory an emphasis on systemic emergence, on the importance of connection topology, and on the distinction between simple and complex contagion processes.


Where the present theory advances. Network science is, in general, agnostic about the substantive content of the relations it models: a tie is a tie, a node is a node. This agnosticism is methodologically powerful but theoretically thin: it cannot, on its own, explain why some networked phenomena exhibit distinctive logics (legal/illegal, profit/loss) or why coupling channels between distinct logics behave differently from couplings within a single logic. The CGM supplies the substantive content network science abstracts from: nodes are subsystems with codes and programs, edges are coupling channels with substantive operational character. Conversely, the network-science formalization of contagion, threshold dynamics, and small-world topology is the natural mathematical apparatus for the present theory's predictions about λ_max, contagion thresholds (P3), and norm cascades.


Where the rival retains priority. Network science's mathematical sophistication for analyzing topology, for distinguishing complex from simple contagion, and for characterizing scale-free vs. small-world networks is essential machinery the present theory imports rather than develops. Future work should integrate the present theory's substantive coupling matrix with network science's structural-analytic tools.

### 6.4 Analytical sociology (Hedström, Coleman)

Analytical sociology (Coleman, 1990; Hedström, 2005; Hedström and Bearman, 2009) shares with the present theory the commitment to mechanism-based explanation, to multi-level (Coleman-boat) causal architectures, and to formal modeling.


Where the present theory advances. Analytical sociology's commitment to methodological individualism — that all social phenomena ultimately ground in individual action — is in tension with the Luhmannian commitment to subsystems as autonomous loci of operation that cannot be reduced to the actions of their participating individuals. The present theory is more permissive: it preserves the Coleman-boat architecture as a useful tool for analyzing each loop while declining the strong methodological-individualist claim that subsystem operations are nothing-but-aggregated-individual-actions. Subsystems have their own programs, codes, and operations that constrain individual action without being reducible to it. The present theory's CGM thus integrates analytical sociology's methodological apparatus with critical realism's stratified ontology, an integration not generally undertaken in either tradition alone.


Where the rival retains priority. Analytical sociology's careful work on specific mechanisms (network effects, threshold models, opportunity structures) and its insistence on methodological precision provide standards the present theory should aspire to throughout. The discipline imposed by analytical sociology — that one specify mechanisms rather than gesture at "factors" — has guided the present theory's drafting and should continue to discipline its empirical development.

### 6.5 Summary of comparative position

The present theory is not a wholesale replacement for any of these traditions. It is, rather, a framework that integrates their compatible commitments — multi-level analysis (world-systems), institutional codes and categorical effects (neo-institutionalism), network topology and contagion (network science), mechanism-based explanation (analytical sociology) — while refusing the partial reductions each tradition is sometimes tempted toward. Its specific contribution is the CGM: a single mechanism from which the legitimate insights of each tradition can be recovered as special cases, with explicit operational content and falsifiable predictions across the four loops.



## 7. Discussion

### 7.1 Limitations

Several limitations of the present theory should be acknowledged candidly.


Calibration of formal constants. The equation system in §4.3 contains several constants (α, β, η, δ, μ, φ) whose empirical values are not yet established. Without calibration, the system can demonstrate qualitative regime behavior but not precise quantitative prediction. Calibration is itself a research program, requiring coordinated empirical work across multiple subsystems and time scales.


Subsystem inventory. We have treated seven subsystems as canonical (legal, economic, political, scientific, religious, aesthetic, mediatic). This inventory is approximately the Luhmannian list, with some modifications. Other plausible subsystems exist — health, military, education, sport — and the boundary between subsystem and subsystem is not always sharp. The theory's predictions are robust to small changes in the inventory but the formalization assumes a finite set; substantial revision of the inventory would require corresponding revision.


Cross-cultural reach. The theory is most fully developed for differentiated modern societies in the Western European/North American mold. Its claims about non-Western differentiated societies are, at present, theoretical extrapolations rather than empirically validated extensions. Comparative work across diverse modernities (Eisenstadt, 2000) is needed.


Historical causality. The theory specifies mechanisms whose operation produces system-level outcomes given certain configurations. It does not, by itself, explain how the configurations came to be. The historical processes by which subsystems differentiated, by which coupling channels were institutionally constructed, and by which buffering mechanisms were established or removed are themselves objects of historical-sociological inquiry that the theory presupposes.

### 7.2 Scope conditions revisited

§2.4 specified scope conditions. We elaborate three.


Failure mode 1: pre-differentiation. In societies before consolidated functional differentiation, the CGM's premise is violated. The theory predicts nothing useful for such societies; segmentary or stratified models are appropriate.


Failure mode 2: totalitarian or autocratic compression. Where multiple subsystems are simultaneously deprived of operational autonomy by a dominating political-ideological apparatus, the differentiation premise fails. The theory predicts rather specific outcomes for such cases (Loop 2 suppression, Loop 4 distortion or suspension), but these should be considered limiting rather than typical applications.


Failure mode 3: post-shock liminal periods. In the immediate aftermath of catastrophic disruption (war, mass-casualty disaster, civil collapse), subsystem codes may be temporarily suspended and replaced by emergency operational logic. The CGM does not apply during such periods, though it does describe both the normal-period dynamics that preceded them and the dynamics by which systems reconstitute themselves.

### 7.3 Unresolved tensions

Three tensions internal to the theory deserve acknowledgment rather than concealment.


Tension 1: stability of subsystem inventory. The theory treats subsystems as relatively stable. But subsystems can in principle differentiate further (the mediatic subsystem has, arguably, partially differentiated into a distinct algorithmic-attention subsystem in the platform era), or de-differentiate (a colonized subsystem may lose code-distinctiveness). The dynamics by which the inventory itself evolves are not fully formalized in the present theory.


Tension 2: agency at the global level. The theory's macro-level entities — subsystems, coupling matrix — are not agents in the sense individuals are agents. But certain organizations (multinational corporations, transnational regulatory bodies, large platforms) appear to operate at a level intermediate between individual agency and subsystem-level operation. Whether these should be treated as "macro-individuals," as densified institutional bridges, or as a distinct category, is not fully resolved.


Tension 3: normativity. The theory is descriptive-explanatory rather than normative. Yet its predictions about reflective-autonomy erosion under platform mediation (P9) and about subsystem colonization (P4) carry obvious normative resonance: most readers will treat the predicted outcomes as undesirable. The theory does not justify that evaluative response, and its predictions hold whether or not one shares it. Future work integrating the theory with normative political philosophy is possible but is not undertaken here.

### 7.4 Calibration and further research

The next stage of the research program comprises four tasks. (a) Calibration of the formal constants by parallel empirical estimation across multiple datasets and historical periods. (b) Implementation of the COFD-ABM (Appendix B) and validation of its emergent dynamics against historical data. (c) Targeted experimental and observational tests of the sixteen propositions; six of them (P1, P2, P6, P8, P12, P13) are tractable in standard experimental or quasi-experimental designs at modest cost. (d) Comparative cross-cultural testing to determine the theory's robustness across different modernities.



## 8. Conclusion

This paper has sought to do for a five-level descriptive metatheory of the human social system what the literature has long demanded but rarely supplied: replace it with a mechanism-based, falsifiable, formalized theory whose central claims are operationalized, whose predictions are deducible, and whose limits are explicitly stated.


The Core Generative Mechanism is parsimonious. It says: differentiated subsystems coupled selectively and asymmetrically through specifiable channels produce, simultaneously, coordination and tension, both of which feed back to individuals through internalization and to groups through situational logic switching. From this single mechanism, we have recovered (a) why individual cognition is shaped before reflective capacity becomes available; (b) why small groups switch among the four Fiskean relational logics in response to specifiable cues; (c) why subsystems do not merge yet do not isolate; (d) why colonization is possible, predictable, and measurable; (e) why globally synchronized crises emerge above identifiable thresholds of coupling; (f) why surveillance-capitalist platforms erode reflective autonomy as a matter of structural mechanism, not of ill intent; and (g) what would falsify the theory.


The framework also preserves and gives technical content to a set of substantive insights from the theory's original informal formulation that, in less rigorous treatments, can read as merely evocative. The ego is the locus where the four loops meet, organized around survival, recognition, and status, with affective valence on a love/fear approach/avoidance axis (§3.1.1). The aggregate institutional layer functions as a Social Operating System within which ideology and religion serve as the categorical glue allowing millions of unacquainted egos to coordinate beyond Dunbar's limit; population-level affective states are routed through an affect-to-institution translation table ("altruism becomes tax, fear becomes national security"); the legal subsystem replaces personal revenge with formal procedure; money operates as a "religion of trust" sustained by technology and information; political legitimation systematically wraps subsystem outputs in the language of the common good as a structural rather than rhetorical requirement (§3.4.1). The convergent state of the system in the platform era is the predictive anticipation of the ego before reflective thought (§3.6). The canonical closed-orbit trajectory of the system's state space is the Leviathan loop: money → technology → ideology → education → ego → system → money (§3.7). None of these claims is decorative. Each is now formally derivable from the CGM, operationalized in §4, and tied to one or more falsifiable propositions in §5.


The contribution claimed is not the discovery of a new mechanism — most of the components are visible in existing literatures — but their integration into a single derivable framework with computable predictions across scales. The audit that prompted this revision rightly observed that the original framework was a descriptive metatheory rather than a theory in the working sense. We have attempted to repair that, while preserving every substantive insight of the original informal formulation rather than abstracting it away, and we submit the result for the discipline's evaluation.


If the propositions of §5 are tested and largely fail, the CGM is wrong, and the framework should be abandoned. If they are tested and largely succeed, the framework provides a useful integration. Either outcome would advance the discipline more than continued elaboration of descriptive accounts. The point of submitting this version, in the form prescribed by the audit, is precisely to make either outcome possible.



## References

Anderson, B. (1983). Imagined Communities: Reflections on the Origin and Spread of Nationalism. London: Verso.


Archer, M. S. (1995). Realist Social Theory: The Morphogenetic Approach. Cambridge: Cambridge University Press.


Archer, M. S. (2003). Structure, Agency and the Internal Conversation. Cambridge: Cambridge University Press.


Barabási, A.-L. (2002). Linked: The New Science of Networks. Cambridge, MA: Perseus.


Barabási, A.-L. (2016). Network Science. Cambridge: Cambridge University Press.


Barrett, L. F. (2017). How Emotions Are Made: The Secret Life of the Brain. Boston: Houghton Mifflin Harcourt.


Beck, U. (1992). Risk Society: Towards a New Modernity. London: Sage.


Bedau, M. A. (1997). Weak emergence. Philosophical Perspectives, 11, 375–399.


Berger, J., Fisek, M. H., Norman, R. Z., & Zelditch, M. (1977). Status Characteristics and Social Interaction. New York: Elsevier.


Berger, P. L., & Luckmann, T. (1966). The Social Construction of Reality. New York: Doubleday.


Bhaskar, R. (1975). A Realist Theory of Science. Leeds: Leeds Books.


Bhaskar, R. (1979). The Possibility of Naturalism. Brighton: Harvester.


Brown, W. (2015). Undoing the Demos: Neoliberalism's Stealth Revolution. New York: Zone Books.


Bruner, J. (1990). Acts of Meaning. Cambridge, MA: Harvard University Press.


Callon, M. (Ed.) (1998). The Laws of the Markets. Oxford: Blackwell.


Centola, D. (2018). How Behavior Spreads: The Science of Complex Contagions. Princeton: Princeton University Press.


Chalmers, D. J. (2006). Strong and weak emergence. In P. Clayton & P. Davies (Eds.), The Re-emergence of Emergence (pp. 244–256). Oxford: Oxford University Press.


Coleman, J. S. (1990). Foundations of Social Theory. Cambridge, MA: Harvard University Press.


Crutchfield, J. P. (1994). The calculi of emergence. Physica D, 75(1–3), 11–54.


DiMaggio, P. (1997). Culture and cognition. Annual Review of Sociology, 23, 263–287.


DiMaggio, P., & Powell, W. W. (1983). The iron cage revisited. American Sociological Review, 48(2), 147–160.


Dunbar, R. I. M. (1992). Neocortex size as a constraint on group size in primates. Journal of Human Evolution, 22(6), 469–493.


Easley, D., & Kleinberg, J. (2010). Networks, Crowds, and Markets. Cambridge: Cambridge University Press.


Eisenstadt, S. N. (2000). Multiple modernities. Daedalus, 129(1), 1–29.


Ekman, P. (1992). An argument for basic emotions. Cognition and Emotion, 6, 169–200.


Evans, J. S. B. T., & Stanovich, K. E. (2013). Dual-process theories of higher cognition: Advancing the debate. Perspectives on Psychological Science, 8(3), 223–241.


Fiske, A. P. (1991). Structures of Social Life. New York: Free Press.


Fiske, A. P. (1992). The four elementary forms of sociality. Psychological Review, 99(4), 689–723.


Frank, R. H., Gilovich, T., & Regan, D. T. (1993). Does studying economics inhibit cooperation? Journal of Economic Perspectives, 7(2), 159–171.


Geertz, C. (1973). The Interpretation of Cultures. New York: Basic Books.


Giddens, A. (1991). Modernity and Self-Identity. Cambridge: Polity.


Hacking, I. (1995). The looping effects of human kinds. In D. Sperber et al. (Eds.), Causal Cognition (pp. 351–383). Oxford: Clarendon.


Hedström, P. (2005). Dissecting the Social. Cambridge: Cambridge University Press.


Hedström, P., & Bearman, P. (Eds.) (2009). The Oxford Handbook of Analytical Sociology. Oxford: Oxford University Press.


Henrich, J., Heine, S. J., & Norenzayan, A. (2010). The weirdest people in the world? Behavioral and Brain Sciences, 33(2–3), 61–83.


Kahneman, D. (2011). Thinking, Fast and Slow. New York: Farrar, Straus and Giroux.


Kenrick, D. T., Griskevicius, V., Neuberg, S. L., & Schaller, M. (2010). Renovating the pyramid of needs. Perspectives on Psychological Science, 5(3), 292–314.


Lerner, J. S., Li, Y., Valdesolo, P., & Kassam, K. S. (2015). Emotion and decision making. Annual Review of Psychology, 66, 799–823.


Luhmann, N. (1995). Social Systems. Stanford: Stanford University Press.


Luhmann, N. (2012). Theory of Society, Vol. 1. Stanford: Stanford University Press.


MacKenzie, D. (2006). An Engine, Not a Camera. Cambridge, MA: MIT Press.


Marwell, G., & Ames, R. E. (1981). Economists free ride, does anyone else? Journal of Public Economics, 15(3), 295–310.


Maslow, A. H. (1943). A theory of human motivation. Psychological Review, 50(4), 370–396.


Mauss, M. (1925/1990). The Gift. London: Routledge.


Merton, R. K. (1948). The self-fulfilling prophecy. Antioch Review, 8(2), 193–210.


Meyer, J. W., & Rowan, B. (1977). Institutionalized organizations. American Journal of Sociology, 83(2), 340–363.


Plutchik, R. (2001). The nature of emotions. American Scientist, 89(4), 344–350.


Powell, W. W., & DiMaggio, P. J. (Eds.) (1991). The New Institutionalism in Organizational Analysis. Chicago: University of Chicago Press.


Sapolsky, R. M. (2017). Behave. New York: Penguin.


Slaughter, S., & Rhoades, G. (2004). Academic Capitalism and the New Economy. Baltimore: Johns Hopkins University Press.


Srole, L. (1956). Social integration and certain corollaries. American Sociological Review, 21(6), 709–716.


Steinberg, L. (2014). Age of Opportunity: Lessons from the New Science of Adolescence. Boston: Houghton Mifflin Harcourt.


Sunstein, C. R. (2009). Going to Extremes. New York: Oxford University Press.


Tajfel, H., & Turner, J. C. (1979). An integrative theory of intergroup conflict. In W. G. Austin & S. Worchel (Eds.), The Social Psychology of Intergroup Relations (pp. 33–47). Monterey: Brooks/Cole.


Vygotsky, L. S. (1978). Mind in Society. Cambridge, MA: Harvard University Press.


Wallerstein, I. (1974, 1980, 1989, 2011). The Modern World-System, Vols. 1–4. Berkeley: University of California Press.


Wallerstein, I. (2004). World-Systems Analysis: An Introduction. Durham: Duke University Press.


Watts, D. J. (2002). A simple model of global cascades on random networks. PNAS, 99(9), 5766–5771.


Werker, J. F., & Hensch, T. K. (2015). Critical periods in speech perception. Annual Review of Psychology, 66, 173–196.


Zuboff, S. (2019). The Age of Surveillance Capitalism. New York: PublicAffairs.



## Appendix A. Mathematical Formalization

### A.1 The full state-space formulation

Let X_t denote the system state at time t, comprising:


I_{k,i,t}: internalization scores (k = 1, …, K individuals; i = 1, …, 7 subsystems).

S_{g,t}: active relational logic of group g (g = 1, …, G).

u_{g,t}: situational cue vector for group g.

O_{i,t}: output level of subsystem i.

Γ_t: 7×7 cross-subsystem coupling matrix.

B_t: vector of buffering capacities for each coupling channel.

K_t: stock of social-scientific knowledge.


The system evolves under the equations specified in §4.3, here repeated for completeness:


(A.1) I_{k,i,t+1} = I_{k,i,t} + α · w(d_k) · E_{k,i,t} · r_{k,i,t} · (1 + c_{k,t})^{−1} · (I_max,i − I_{k,i,t})


(A.2) P(S_{g,t+1} = S | u_{g,t}) = exp(β · v_S^⊤ u_{g,t}) / Σ_{S'} exp(β · v_{S'}^⊤ u_{g,t})


(A.3) O_{i,t+1} = (1 − δ) O_{i,t} + δ Σ_j γ_{ji,t} O_{j,t} + ε_{i,t}


(A.4) Γ_{t+1} = Γ_t + η · ΔΓ_t − μ · diag(B_t)


(A.5) Programs_{i,t+Δ} = Programs_{i,t} + φ · K_t · ψ_i


(A.6) E_{k,i,t} = function of (channel exposure of k to outputs O_{i,t}; group-level mediation through S_{g(k),t}).


The system is a coupled non-linear difference-equation system. Equilibrium and stability analysis depend on Γ_t. The relevant criterion is the spectral radius (largest absolute eigenvalue) λ_max(Γ_t):


If λ_max(Γ_t) < 1: perturbations damp; the system is stable in the linear approximation.

If λ_max(Γ_t) ≈ 1: the system is at the boundary of stability; small shocks may persist.

If λ_max(Γ_t) > 1 in unbuffered configurations: perturbations amplify; contagion-like dynamics emerge.


The empirically estimated threshold τ_c referenced in P3 corresponds, in the linear approximation, to λ_max(Γ_t) ≈ 1, with downward adjustment to account for non-linearities and buffering: the empirically meaningful τ_c lies in approximately the 0.6–0.8 range pending calibration.

### A.2 Counterfactual analysis: severing loops

The theory permits explicit counterfactual analysis by setting selected coefficients to zero.


Severing Loop 1 (set α = 0): internalization stops. Predicted: increased generational discontinuity in dispositional patterns; subsystems must rely on coercion or material incentive for compliance, since cognitive uptake is absent. Historical instance: rapid revolutionary periods that suspend educational and family transmission.

Severing Loop 2 (set the aggregation function f_i to a flat constant): macro outputs become unresponsive to micro inputs. Predicted: divergence between elite expectation and population behavior; eventual mobilization breakdown. Historical instance: late-Soviet political economy.

Severing Loop 3 (set Γ to the identity matrix): subsystems operate in isolation. Predicted: loss of coordination; each subsystem becomes autarkic; aggregate productivity declines. Historical instance: this is empirically rare; partial cases observed in extreme isolationist regimes.

Severing Loop 4 (set φ = 0): social-scientific knowledge has no effect. Predicted: no performative drift; theories remain external to their objects. This is, in the modern era, never observed cleanly; every functioning state incorporates some social-scientific knowledge into its operations.

### A.3 Computational tractability

The equation system is computationally tractable. For a population of K = 10⁴ agents organized into G = 10² groups operating against I = 7 subsystems, the per-tick computational cost is approximately O(K + G + I²), which is small. Simulation is feasible on standard hardware. Runtime is dominated by the resolution at which exposure events are tracked.



## Appendix B. The COFD-ABM: Agent-Based Model Specification

This appendix provides a specification sufficient for implementation.

### B.1 Agent types

Type I — Individual agents.


State: {biological state b_k, cognitive load c_k, affective state e_k, motivational stack m_k, internalization vector I_k = (I_{k,1}, …, I_{k,7})}.

Actions: respond to exposure (update I_k); make decisions in choice tasks based on current internalization and active group logic.

Group membership: each individual belongs to one or more groups (family, work team, friend network).


Type II — Group agents.


State: {member set M_g, active relational logic S_g, situational cue vector u_g}.

Actions: (a) compute u_g from environment and membership; (b) probabilistically update S_g per equation (A.2); (c) mediate individual decisions according to S_g; (d) reconcile multi-logic activation per status arbitration, narrative reframing, or logic stratification.


Type III — Subsystem agents.


State: {output O_i, code C_i, programs P_i, resource state R_i}.

Actions: (a) receive inputs from coupled subsystems and from individual decisions; (b) apply programs P_i to inputs to produce O_i; (c) propagate O_i to coupled subsystems through Γ; (d) update channels through which exposure E reaches individuals.

### B.2 Environment

The environment includes:


The coupling matrix Γ (initialized empirically from historical estimation; updated per equation A.4).

A resource vector R(t).

An exogenous shock generator producing ε_i(t).

A buffering vector B(t).

### B.3 Time step (one tick)

Subsystems generate outputs O_i(t) given current inputs and program rules.

Outputs propagate through Γ to other subsystems and through channels to individuals (updating exposure E_{k,i}).

Groups update situational cues u_g.

Groups probabilistically update active relational logic S_g.

Individuals update internalization I_{k,i} per equation (A.1).

Individuals make decisions, mediated by their group's S_g, weighted by their I_k.

Decisions aggregate (per channel-specific aggregation functions) into next-period subsystem inputs.

The buffering vector B(t) updates per institutional design rules.

The coupling matrix Γ evolves slowly per equation (A.4).

Loop 4 (slow): periodically (per Δ ticks), the social-scientific subsystem updates K_t and modifies programs P_i per equation (A.5).

### B.4 Calibration parameters

Empirically estimable initial values:


α (learning-rate constant): 0.01–0.10 per tick depending on tick definition; lower for adult learning, higher during sensitive periods.

β (logic-switching inverse temperature): 1–5; higher β corresponds to deterministic responsiveness to cues.

δ (coupling-influence rate): 0.05–0.30; estimable from impulse-response analysis on historical data.

η (coupling-formation rate): slow; 0.001–0.01.

μ (buffering effectiveness): policy-dependent; 0.1–0.5 with effective regulation.

φ (Loop-4 uptake rate): slow; ~0.01.

### B.5 Expected emergent outcomes

Validation criteria for the ABM include the following emergent outcomes (each corresponding to a proposition in §5):


Under sustained increase of η without buffering, λ_max(Γ) rises and crisis-synchronization frequency rises super-linearly (validates P3, P7).

Under sustained asymmetric coupling from one subsystem to another, terminology drift in the colonized subsystem develops (validates P4).

Under platform-equivalent acceleration of Loops 1, 2, and 4, individual decision latency declines and platform-prediction accuracy rises (validates P9).

Under externally imposed resource shock to small groups, MP displaces EM (validates P1).

Under threat plus homogeneity, CS displaces both AR and MP (validates P12).

### B.6 Implementation notes

A reference implementation should use an event-driven simulator rather than a fixed-time-step simulator, because the time scales of the four loops differ by orders of magnitude (Loop 4 is ~10⁴ times slower than Loop 1 on platform-mediated environments). Multi-scale temporal integration is essential. Standard ABM platforms (NetLogo, Mesa, RepastHPC) are adequate for prototype implementation; scaling to populations larger than 10⁵ requires distributed computation.



## Appendix C. Extended Proposition Table

The sixteen propositions of §5 are reproduced here in tabular form with full operational specification.



The propositions span the four loops, the three levels (individual, group, subsystem/global), and the three principal methodological traditions (experimental, computational, comparative-historical). Together they constitute a research program rather than a single empirical study.





