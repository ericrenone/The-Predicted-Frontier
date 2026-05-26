# The Predicted Frontier: Hubert Dreyfus, Absorbed Coping, and the Phenomenological Account of Why Machine Intelligence Has the Shape It Has

> "I predicted that AI would not achieve general intelligence because intelligence requires understanding, and understanding requires being in the world. The AI community was not interested. They called my paper 'Alchemy and Artificial Intelligence.' The title was intended to wound."
> — Hubert Dreyfus, in interview, circa 2010

> "The expert does not solve problems. He does not deliberate. He does not even act deliberately in the usual sense of the word. He just does what normally works and, naturally, it normally works."
> — Hubert L. Dreyfus & Stuart E. Dreyfus, *Mind over Machine*, 1986

> "In Alchemy and AI and What Computers Can't Do, Dreyfus identified four philosophical assumptions, at least one of which he deems necessary for AI to succeed. In each case, the assumption is taken by workers in AI as an axiom, guaranteeing results, whereas it is, in fact, one hypothesis among others, to be tested by the success of such work."
> — Dreyfus's own account, as documented

> "Without involvement and presence, we cannot acquire skills."
> — Hubert Dreyfus, *On the Internet*, 2001

> "Intelligence is skill-acquisition efficiency on novel tasks."
> — François Chollet, *On the Measure of Intelligence*, 2019

---

## A Structural Gap and What Fills It

The companion READMEs — *The Budapest Transmission* and *The Bifurcated Century* — establish the philosophical and economic foundations of what machines cannot hold. Polanyi names tacit knowledge. Hayek identifies its economic consequences. Wittgenstein demonstrates that the rules constituting a language-game presuppose a pre-theoretical form of life. Arendt establishes the irreducibility of action. Gödel proves, from within mathematics, that formal systems contain truths they cannot prove. The intellectual edifice is formidable.

What neither README names is the figure who brought this entire apparatus to bear directly, specifically, and in real time against the AI research program — who read the classified internal reports at RAND, who tracked the specific promises of Minsky, McCarthy, Newell, and Simon, who named their failures before they occurred, who predicted the precise *shape* of what Kapoor et al. (2026) now call the jagged frontier, and who spent the next fifty years watching the AI community alternately ignore him, declare him refuted, and eventually — with the publication of open-world evaluation results — confirm every structural prediction he had made.

Hubert Dreyfus (1929–2017) is the biggest analytical gap in the existing framework. His absence is not peripheral. It is the gap between having a philosophical account of machine limits and having a *predictive* account — an account that specified in advance what AI systems would accomplish, what they would fail to accomplish, and exactly why the failure pattern would take the form it takes.

This README traces the complete Dreyfus lineage: the philosophical sources from which he drew, the arguments he constructed from those sources, the engineering confirmation those arguments received, the three cycles of declared refutation and actual vindication, and the connection — never yet made explicit in the AI literature — between his five-stage skill acquisition model and the mechanism that Ide (2026) is now formalizing as the intergenerational transmission trap.

---

## I. The RAND Position: Reading the Classified Files

In the early 1960s, Hubert Dreyfus was a young philosopher at MIT who had completed his doctoral dissertation at Harvard on Husserl's phenomenology. He was not, initially, interested in artificial intelligence. The connection was forced on him by circumstance: he was engaged as a consultant by the RAND Corporation and given access to the internal technical reports that Minsky, McCarthy, Newell, and Simon were circulating before publication.

What Dreyfus read in those reports alarmed him — not because the claims were modest but because they were maximal, and because he could see, from the phenomenological framework he had developed, exactly where the program would fail. Newell and Simon's General Problem Solver (1957) claimed to model human problem-solving by reducing it to symbol manipulation over explicit representations. McCarthy's programs assumed that intelligence consists in the formal manipulation of logical expressions. The entire enterprise was built on an assumption that Dreyfus recognized, from his reading of Heidegger and Merleau-Ponty, as philosophically untenable: that the behavior of intelligent beings can be decomposed into rule-governed operations on context-free symbolic representations.

Dreyfus wrote "Alchemy and Artificial Intelligence" in 1965 as a RAND working paper — the title deliberate and pointed: alchemy was the program that medieval practitioners pursued with complete sincerity, that had a sophisticated internal logic, and that was constitutively misconceived about the nature of matter. RAND was reluctant to publish it. The AI community's response, when the paper circulated, was contempt: Marvin Minsky dismissed him; Seymour Papert argued publicly that an MIT checkers program would defeat Dreyfus within a year. (Dreyfus played, won, and was thereafter excluded from the rematches.)

What was dismissed in 1965 was a precise, structured argument derived from two decades of European phenomenological philosophy and bearing directly on the theoretical foundations of the AI program. The argument was not "AI will never achieve anything." It was something more specific: AI systems, operating on the assumptions that governed their design, would achieve strong performance within closed, formally specified domains and would fail systematically at the boundaries of those domains — at the point where human performance draws on a background of embodied, worldly engagement that formal specification cannot capture. This is what the jagged frontier looks like. Dreyfus described it in 1965, before any modern AI benchmark existed.

---

## II. The Philosophical Sources: Heidegger's Being-in-the-World

Dreyfus drew explicitly on two philosophical sources that the existing READMEs have not fully analyzed in their connection to the AI problem. The first is Martin Heidegger's *Being and Time* (1927). The second is Maurice Merleau-Ponty's *Phenomenology of Perception* (1945). Together, they provide the positive account — the description of what human knowing actually is — that grounds Dreyfus's negative argument about what machines cannot do.

Heidegger's central contribution is the analysis of *Dasein* — the human way of being — as fundamentally *being-in-the-world*: not a mind that receives information about an external world and then acts on it, but a being whose existence is constitutively a mode of engaged, purposeful, situated inhabiting of a world that is always already structured by its practices, projects, and concerns. This framing reverses the Cartesian picture on which all classical AI depends: there is no mind on one side and a world of objects on the other. There is only the engaged existence of beings for whom the world shows up as a space of possibilities and resistances defined by what they care about.

The distinction that Dreyfus found most directly applicable to AI is Heidegger's distinction between *Zuhandenheit* (readiness-to-hand) and *Vorhandenheit* (presence-at-hand). Equipment, in the normal course of skilled use, is *ready-to-hand*: it recedes into the background, becomes transparent, and the agent's attention is directed through it at the task rather than at the tool. The skilled carpenter does not attend to the hammer while hammering well; the hammer is an extension of the action, not an object of contemplation. It is only when the hammer breaks, or becomes unfamiliar, or fails in its function, that it becomes *present-at-hand*: an object of explicit attention, something to be examined and described. The breakdown from readiness-to-hand to presence-at-hand is the moment at which the skilled practitioner is forced to adopt the stance of the observer — and this is the only stance available to AI systems operating on explicit representations.

Dreyfus's argument from this analysis is structurally decisive: AI systems always operate in the *presence-at-hand* mode. They have explicit representations of everything. Nothing becomes transparent in the way that equipment becomes transparent for a skilled agent. The AI system always treats the world as an array of objects with describable properties, to be manipulated according to explicit rules. This is not a contingent limitation of current architectures. It is a constitutive feature of any system whose operation is defined by the manipulation of explicit symbolic representations. The readiness-to-hand is not a more complex form of presence-at-hand that more computational power could achieve. It is a different mode of engagement — one that requires being a kind of entity that has equipment in the first place, that has projects in which that equipment is deployed, and that exists in a world structured by those projects and their interconnections.

Heidegger's second contribution is the concept of *background*: the vast, inarticulate, pre-reflective understanding of a shared world that makes any specific understanding possible. Before I can understand the meaning of a hammer, I must already understand what it is to build things, what it is to drive nails, what it is to intend a structure — and this understanding is not itself made up of more explicit representations but is the ground on which explicit representations can get purchase at all. The background, for Heidegger, is not a very large explicit belief set. It is a mode of being — the mode of being-in-the-world — that cannot be assembled from any finite collection of explicit propositions. Dreyfus's central argument is that this background is what AI systems cannot hold, not because it is too large, but because it has the wrong *form*: it is not propositional, not representable, not the kind of thing that can be stored and retrieved.

---

## III. The Philosophical Sources: Merleau-Ponty's Body Schema

The second philosophical source is Maurice Merleau-Ponty's *Phenomenology of Perception* (1945) — published the same year as von Neumann's First Draft of a Report on the EDVAC, the year in which the formal machine and its philosophical critique arrived simultaneously. Merleau-Ponty's contribution is the account of embodied cognition that specifies the *biological* form of the background that Heidegger identified.

Merleau-Ponty's central argument is that the body is not an object that the mind controls but the medium through which we are present to the world. The *body schema* — the body's tacit, pre-reflective map of its motor capacities and their relation to the environment — is the ground of all intentional engagement. I do not first represent my arm's position and then calculate how to reach for a cup. My body orients toward the cup in a unified motor act that is directed at the cup as something to be grasped, without any intermediate representation of body parts and their trajectories. The body's knowledge is a practical knowledge — a *motor intentionality* — that is not possessed by a mind but is enacted by a body organized by its history of skillful engagement with its environment.

The implications for machine intelligence are more specific than Heidegger's analysis alone provides. Merleau-Ponty gives two examples that Dreyfus found clinching. First, the blind person's cane: a skilled blind person does not represent the cane as an object between herself and the world, registering its properties and calculating their significance for navigation. The cane becomes an extension of the body schema — a new organ of perception, a way of feeling the world's surfaces and obstacles — such that the experienced blind person attends not to the cane but *through* it to the world. The cane's integration into the body schema is the body acquiring a new way of being in the world, not a mind acquiring a new tool for processing information. No representation mediates this. The body changes.

Second, the typist. A skilled typist who is asked where the letter "M" is on the keyboard often cannot answer without moving her hands — the knowledge is in the fingers, not in any explicit representation. The body knows things that the mind does not know in the form of propositions. This is not, for Merleau-Ponty, a deficient form of knowledge awaiting articulation. It is the primary form of knowing, the form on which all explicit knowledge rests. The typist's propositional knowledge that "M" is near the right side of the bottom row — if she can access this at all — is a secondary achievement, an abstraction from the motor knowledge that constitutes her skill. To say that the motor knowledge is merely an efficient route to propositional knowledge is to get the order of explanation backwards.

Dreyfus's connection of Merleau-Ponty to the AI critique is direct: *motor intentionality* is the form in which tacit knowing is constituted. It is not pre-verbal knowledge waiting to be articulated. It is a different logical type of cognitive achievement — one that requires a body that has been changed by its history of engagement with the world, and that could not be replicated by any system that merely processes descriptions of skilled behavior.

---

## IV. The Four Assumptions and Their Systematic Refutation

In "Alchemy and Artificial Intelligence" (1965) and *What Computers Can't Do* (1972), Dreyfus identified four philosophical assumptions on which the AI program depended — assumptions that were treated as axioms by AI researchers but that the phenomenological tradition had already subjected to decisive criticism.

**The biological assumption**: that the brain is a digital device — that it processes discrete elements, much like a digital computer. This assumption was necessary for any claim that computers could replicate mental processes, because if the brain operates on fundamentally different principles, the analogy breaks down before it begins. Merleau-Ponty's neuroscience — which Dreyfus supplemented with the later work of Walter Freeman on chaotic neural dynamics and Karl Pribram on holographic brain organization — showed that the brain does not operate as a serial processor of discrete symbols. It operates as a massively parallel, dynamical system whose behavior cannot be decomposed into discrete computational steps without loss of the properties that generate its cognitive achievements. This assumption fails biologically.

**The psychological assumption**: that the mind operates by manipulating context-free symbols according to rules. This is the assumption that Heidegger's analysis of the background refutes philosophically: the rules that govern any domain of human activity presuppose a background understanding that cannot itself be captured in rules, because the rules must be applied, and their application requires a kind of understanding that is not itself rule-following. Dreyfus called this the *regress problem for rules*: if every rule application requires further rules specifying how to apply the first rule, the system of rules never closes. Human practice closes this regress not through more rules but through the background understanding of a being-in-the-world, who grasps the situation as calling for a particular kind of response without consulting a rule for that recognition. This assumption fails philosophically.

**The epistemological assumption**: that all genuine knowledge can be formalized — that every form of knowing can, in principle, be expressed as a set of explicit propositions or rules. This is the assumption that Dreyfus, drawing on Polanyi (and developing a parallel argument from phenomenological sources), identifies as false: the tacit dimension of knowing — what Heidegger calls the background, what Merleau-Ponty calls the body schema — is constitutively not propositional. It cannot be formalized without being destroyed. This assumption fails epistemologically.

**The ontological assumption**: that reality consists of context-independent elements with determinate, formally describable properties. This assumption is necessary for any system that operates by matching explicit descriptions to explicit models of the world: the world must be, in principle, fully describable in the terms that the formal system can process. Heidegger's phenomenological analysis shows that the world as it shows up for human beings is not an array of context-independent elements but a space of significance organized by projects, practices, and concerns. The same physical configuration of objects constitutes a "kitchen" in one context and a "workshop" in another, depending on the practices and projects of the beings who inhabit it. No context-independent description can capture this — because the significance is not in the objects but in the form of engagement that constitutes a context in the first place. This assumption fails ontologically.

The four assumptions fail independently, at four different levels of analysis. Dreyfus's argument was not that AI systems would never achieve *anything* — he was careful to acknowledge impressive accomplishments within closed, formally specified domains. His argument was that any system depending on all four assumptions would fail to achieve the kind of general, context-sensitive, background-dependent cognition that human beings exercise in ordinary life and that any account of human intelligence must accommodate.

---

## V. The Five-Stage Model: The Developmental Theory of What Automation Destroys

The most direct contribution of the Dreyfus lineage to the AI-transition debate of 2025–2026 is the five-stage skill acquisition model developed in *Mind over Machine* (1986), co-authored with his brother Stuart Dreyfus, an operations researcher at Berkeley who had applied the model empirically across multiple domains including chess, nursing, flying, mathematics, and military command.

The five stages trace a developmental trajectory from rule-following novice to intuitive expert, and the crucial structural insight is that the transition from the lower stages to the upper stages involves not an accumulation of more rules or more information, but a *dissolution* of the rule-following mode entirely.

**Stage 1: Novice.** The novice is given explicit, context-free rules that specify what to do in terms of objectively identifiable features of the situation. The beginning chess player learns that losing a piece is bad and controls the center. The beginning driver learns: when the speedometer reads 35mph in a 30mph zone, decelerate. The rules are context-free because the novice cannot yet see the context — cannot yet recognize what makes a situation the kind of situation that calls for an exception to the rule. The novice processes the situation as a collection of explicitly specified features and applies the rules mechanically.

**Stage 2: Advanced Beginner.** Through practical experience, the advanced beginner begins to recognize *aspects* of situations that are not defined by explicit features — patterns that emerge from the overall configuration rather than any single objectively specifiable element. The driving student begins to feel when the engine sounds strained. The chess player begins to recognize a "bad bishop" as a structural configuration rather than a count of material. These aspects are context-dependent and cannot be captured in context-free rules; they are the beginning of the background understanding developing.

**Stage 3: Competent.** The competent performer can no longer manage the complexity of the situation by simple rule-following. Too many potentially relevant features present themselves. The competent performer selects a *plan* or *organizing perspective* that makes certain features salient and others irrelevant, and acts from within that perspective. Crucially, the competent performer feels *responsible* for this choice in a way the novice does not — the choice is theirs, not the rule's. Failure is painful. This emotional investment, Dreyfus argues, is not incidental but functional: it is what drives the learning that produces the next stages.

**Stage 4: Proficient.** With more experience, the perspective is no longer consciously chosen but *perceived*: the situation shows up as demanding a particular organizing response. The proficient performer does not decide to treat the situation as of type X — the situation appears as of type X, and the appropriate response suggests itself. Deliberation still occurs at the level of what to do within the perceived situation, but the situation-perception is no longer effortful.

**Stage 5: Expert.** At the level of genuine expertise, both the situation-perception and the responsive action are non-deliberative. The expert does not perceive a situation and then decide how to respond. The situation and the response are perceived together, as a unified practical gestalt. The chess grandmaster does not see a board position and then search for a good move — she sees a good move, and the board as requiring it, in a single act of perception. The surgeon does not analyze the tissue and then decide how to cut — the cut presents itself as called for. Asked to explain what she did and why, the expert must reconstruct an account that was not present in the doing: the account is a secondary artifact, produced for the benefit of novices, that does not correspond to the cognitive process it purports to describe. This is why experts often give bad instruction: instruction requires articulating what expertise does not do — apply rules.

The connection to the AI-transition debate is now exact. Entry-level professional work — the work that AI systems are now absorbing — is Stages 1 and 2. The novice and advanced beginner operate closest to the rule-following mode that formal systems can replicate. They apply explicit procedures to recognizable categories of cases and receive feedback that is comprehensible within the explicit framework of their rules. This is precisely the domain of AI competence.

But Stages 1 and 2 are not merely economically dispensable labor. They are the *necessary developmental conditions* for Stages 3, 4, and 5. The competent performer's emotional stake, the proficient performer's situation-perception, and the expert's intuitive grasp are not skills that can be injected at a later stage once the entry-level work is done by machines. They are the *outcome* of having traversed Stages 1 and 2 under conditions of genuine engagement, failure, feedback, and the slow accumulation of experiential residue that does not survive abstraction from the practice in which it is constituted.

Dreyfus argued this in 1986. Ide (2026) is now formalizing the economic consequence: when entry-level functions are automated, the developmental trajectory is interrupted not at its end but at its beginning. What is lost is not the work done by novices and advanced beginners — that work, in its explicit, rule-following form, is precisely what machines can do. What is lost is the generation of future experts. The intergenerational transmission trap is the macroeconomic surface of a microeducational mechanism that Dreyfus identified from phenomenological premises forty years ago.

---

## VI. The First-Step Fallacy: Dreyfus's Structural Diagnosis of AI Hype

Dreyfus identified a recurring pattern in AI research that he called the "first-step fallacy": the systematic extrapolation from initial success in a narrow domain to confident predictions of general intelligence. His last published paper, produced near the end of his life, documented this pattern across the entire history of AI — from Newell and Simon's prediction in 1958 that a machine would be the world chess champion within ten years (it took forty), to the 1960s predictions that machine translation would be solved within five years (it was not solved for fifty, and the "solution" — statistical translation — works within a fundamentally different paradigm), to the 1980s predictions of expert systems achieving general medical diagnosis.

The structural logic of the first-step fallacy is this: when an AI system achieves impressive performance within a domain, researchers observe the magnitude of the achievement and project that the same rate of progress will continue until general intelligence is reached. What they do not observe — because it requires a philosophical argument to see it — is the *categorical* difference between the achieved performance and the general cognitive capability they extrapolate toward. Performance within a closed, formally specified domain is not a point on a continuous scale toward general intelligence. It is achievement within a *different category* of cognitive task — a task whose tractability depends precisely on its closure, its formal specification, and its independence from the background understanding that general cognition requires.

This analysis is the philosophical ground of what benchmark researchers are now encountering empirically: AI systems saturate closed benchmarks at scale, but this saturation is not evidence of progress toward open-world capability. It is evidence of the precise boundary that Dreyfus drew in 1965. The first-step fallacy is the institutional expression of the epistemological confusion: treating performance on closed-domain tasks as evidence of progress toward open-world capability misidentifies what has been achieved, because it does not distinguish between the domain of the formally tractable and the domain that requires the background understanding of a being-in-the-world.

The ARC-AGI benchmark, introduced by François Chollet in "On the Measure of Intelligence" (2019), is the most rigorous empirical instantiation of Dreyfus's critique. Chollet's explicit design principle is the distinction between *skill* — performance on specific tasks, which can be "bought" by training data — and *intelligence* — the efficiency of acquiring new skills from minimal experience. The benchmark was designed specifically to resist pattern-matching on training data, to require the kind of flexible generalization that Dreyfus argued machines cannot achieve: the recognition that a situation is a *new kind of thing* requiring a *new kind of response*, rather than the application of a learned pattern to a familiar category. The persistent gap between frontier AI performance on ARC-AGI (which remained well below human-level through multiple generations of systems, including the best reasoning models of 2024–2025) and human performance — humans solve roughly 80% of tasks that AI systems, even with high compute, solve at a fraction of that rate — is the empirical measurement of the boundary Dreyfus drew philosophically.

Chollet did not cite Dreyfus. But his definition of intelligence — skill-acquisition efficiency on novel tasks, the ability to adapt to new problems whose creators did not anticipate — is a formal rendering of what Dreyfus's account of Stage 5 expertise predicts will be machine-resistant: the capacity to recognize what kind of thing one is facing when that kind of thing has not been encountered before. ARC-AGI-3 (2025), extending the challenge to continuous skill-acquisition tasks in novel game environments, makes the Dreyfus connection more explicit: it tests precisely the ability to constitute a new understanding of a new domain, which is what Dreyfus's analysis of Stages 4 and 5 identifies as constitutively dependent on the background understanding of an embodied, world-engaged being.

---

## VII. The Winograd Conversion: When a Founder of AI Read Dreyfus

The most consequential reception of Dreyfus's work within the AI community itself occurred when Terry Winograd — one of the field's founders, developer of the SHRDLU program (1970), which was then among the most impressive demonstrations of natural language understanding by machine — read *What Computers Can't Do* and was persuaded.

Winograd's SHRDLU could accept natural language commands about a simulated blocks world and respond intelligently within that world. The system was heralded as a breakthrough, and Winograd was celebrated as a pioneer. But Winograd came to understand, through his encounter with Dreyfus's argument, what SHRDLU's success demonstrated: not that machine understanding of natural language was within reach, but that within a severely restricted, formally closed domain — a world reduced to a small number of objects with explicit properties and a small number of possible relations — machine performance could look like understanding while depending on none of the background understanding that human natural language comprehension requires. The system was "brittle": brilliant within its world, helpless the moment the world changed or the inputs referred to anything outside the formal specification.

Winograd moved to Stanford, pivoted from classical AI to a new kind of design philosophy, met Fernando Flores — a Chilean philosopher who had been Minister of Finance under Allende and had encountered Heidegger in prison — and co-authored *Understanding Computers and Cognition: A New Foundation for Design* (1986). The book argued, drawing explicitly on Heidegger, Maturana, and Dreyfus, that the assumption underlying classical AI — that intelligence consists in the manipulation of formal representations — was philosophically untenable, and that a new foundation for computing design must take seriously the background of human practice that all computing tools are embedded in and cannot themselves replace.

The genealogy that follows is remarkable. Winograd, having written *Understanding Computers and Cognition*, moved to Stanford, where one of his graduate students was Larry Page. Page, supervised by Winograd in the late 1990s while Winograd was doing research on digital libraries, co-founded Google. The search engine architecture that Page and Sergey Brin developed — PageRank, the ranking of web documents by their link structure rather than by explicit metadata — is, in a philosophically significant sense, a design that takes Winograd's post-Dreyfus insight seriously: rather than trying to explicitly represent relevance, it uses the structure of human behavior (linking, citing) as a proxy for the human background understanding that determines relevance. It is not a representation of relevance but an aggregation of the behavioral residue of relevance-judgments made by embodied, world-engaged humans. This is the opposite of the classical AI program that Dreyfus criticized, and it works.

The Dreyfus–Winograd–Page connection is the most direct demonstration that the phenomenological critique of AI has practical engineering consequences — that taking seriously what machines cannot do changes what one builds, and that building in ways that aggregate human judgment rather than replace it produces systems of extraordinary power within a domain that is, crucially, different from the domain of background-dependent human cognition.

---

## VIII. The Engineering Confirmation: Rodney Brooks and Intelligence Without Representation

Dreyfus's argument was philosophical. Its engineering confirmation came from within robotics, independently, through a route that did not cite Dreyfus but converged on his conclusions.

Rodney Brooks, at MIT, began building mobile robots in the late 1980s on the principle that had been implicit in Dreyfus's critique: that intelligent behavior does not require an explicit internal representation of the world. Brooks's "subsumption architecture" (1986) replaced the central-representation-and-planning paradigm of classical AI robotics with a layered architecture of reactive behaviors that interface directly to the world through perception and action. Each layer operates independently, perceiving the world and responding to it without constructing an explicit model or planning a course of action. The robot navigates an office environment not by building a map of it and planning paths through the map but by perceiving obstacles and responding to them in real time, through a hierarchy of behavioral responses that are tuned by their history of engagement with the actual environment.

Brooks's 1991 paper "Intelligence without Representation" reported that behavior-based robots outperformed representation-based robots at tasks in unstructured, real-world environments. The lesson was Dreyfusian: when intelligence is grounded in direct environmental engagement rather than mediated by explicit representations, it handles the variability and unpredictability of the real world better, not worse. The explicit representation, far from enhancing intelligence, introduces a fragility — the brittleness that Winograd had observed in SHRDLU — that ground-level engagement avoids. Brooks's observation was precise: "When we examine very simple level intelligence we find that explicit representations and models of the world simply get in the way. It turns out to be better to use the world as its own model."

This is Heidegger's distinction between readiness-to-hand and presence-at-hand, expressed in engineering terms: the robot that uses the world as its own model is operating in the readiness-to-hand mode, engaging with the environment directly rather than through a formal representation of it. The robot that builds an explicit model and plans against the model is operating in the presence-at-hand mode — and pays the price in brittleness, failure under unpredicted conditions, and the inability to cope with the ambiguity and context-dependence of the real world.

Brooks did not cite Dreyfus in the 1991 paper. The convergence is independent — a roboticist arriving, from engineering experience, at the same structural conclusions that a philosopher had reached from phenomenological premises twenty-five years earlier. This independence makes the convergence epistemologically significant: the claim that explicit representation introduces fragility rather than enhancing intelligence was not an idiosyncrasy of Dreyfus's philosophical framework. It was a structural truth about the relationship between formal systems and real-world engagement that independently careful inquiry reached from two different directions.

---

## IX. The Three Cycles of Declared Refutation and Actual Vindication

Dreyfus's argument was declared refuted three times across sixty years. Each declaration missed the point, and the subsequent development of AI confirmed it. The pattern is itself philosophically instructive: it is the first-step fallacy operating on his critics, who observed AI achievements within closed domains and concluded that the categorical argument had been answered.

**Cycle 1: Chess (1957–1997).** Dreyfus argued that chess, as a formally specified game with well-defined rules and a clear evaluation function, was precisely the kind of domain where AI would succeed — and that success at chess would therefore demonstrate nothing about general intelligence, because chess is not an open-world task requiring background understanding. He was ridiculed when AI programs failed to beat grandmasters in the 1960s and 1970s. He was declared comprehensively refuted when Deep Blue defeated Kasparov in 1997. But Dreyfus's point had never been that chess was beyond AI — he had predicted that AI would succeed at chess on the grounds that chess is a formally tractable domain. The refutation proved the point. Deep Blue's success showed exactly what Dreyfus had argued: that sufficient computational power, applied to a formally closed domain with explicit rules and a clear success criterion, can surpass human performance. It showed nothing about general intelligence. The critics who declared him refuted by Deep Blue had not understood the argument.

**Cycle 2: Connectionism (1980s–1990s).** When connectionist neural networks (back-propagation, multi-layer perceptrons) achieved successes that symbolic AI had failed to achieve — pattern recognition, speech processing, handwritten character recognition — the AI community declared that the Dreyfusian critique of symbolic representation had been circumvented. Connectionist networks do not manipulate explicit symbols; they learn distributed representations from data. This seemed to answer the objection about context-free symbolic manipulation. Dreyfus welcomed the shift away from symbolic AI as moving in the right direction but argued that connectionism still failed on the background problem: connectionist networks learn from training data, and their performance is bounded by what that data contains. They do not bring to a new situation the background understanding of a being-in-the-world — they apply a learned pattern to a new instance of a familiar distribution. They fail when the test distribution is genuinely novel, when the task requires understanding *what kind of thing* one is facing rather than *which familiar pattern* it resembles. This is the out-of-distribution failure that every generation of neural networks, including transformers, exhibits at the boundaries of its training domain.

**Cycle 3: Deep Learning and Large Language Models (2012–2024).** The transformer architecture, applied at scale, produced achievements that seemed finally decisive: superhuman performance at image recognition, protein folding, competitive mathematics, code generation, and sophisticated natural language production. The AI community, and most of the public, concluded that the Dreyfusian critique had been answered: intelligence could be achieved by pattern matching at scale. The counter-evidence accumulated quietly — in open-domain evaluation results, in the persistent failure of large language models on tasks requiring genuine novelty, in the ARC-AGI benchmark scores that remained well below human-level despite extraordinary compute — until the publication of open-world evaluations (Kapoor et al., 2026) made the structure of the failure visible as the jagged frontier. Dreyfus's categorical distinction between closed-domain performance and open-world capability was confirmed, again, by empirical results. The third cycle of declared refutation resolved, as the first two had, as confirmation.

---

## X. "On the Internet" as the Unread Prophecy of AI Tutoring

In 2001, four years before YouTube, fourteen years before AI tutoring systems attracted serious investment, and twenty-four years before the AI-driven disruption of professional education became a policy debate, Dreyfus published *On the Internet* — the most directly applicable work in his entire corpus for the AI-transition scenario the companion READMEs describe.

Dreyfus's argument in *On the Internet* was not merely that online learning is less effective than in-person learning. It was that online learning — and, by structural extension, any mediated learning that removes the learner from embodied, at-risk, co-present engagement with a skilled practitioner — cannot produce genuine expertise. It can produce Stage 3 competence at most. The reason is the same reason that machines cannot hold tacit knowledge: the development from competent to proficient to expert requires the kind of engagement that only embodied presence, genuine risk, and the apprenticeship relation provide.

Four structural conditions for expertise development, which Dreyfus identified in *On the Internet*, are destroyed by both online learning and AI-mediated entry-level work:

*Embodied relevance*: The ability to distinguish relevant from irrelevant in a complex situation is grounded in the shape and movement of the practitioner's body in a physical environment. When the learner is physically present in the environment of practice — the hospital ward, the courtroom, the laboratory, the trading floor — the environment organizes their attention in ways that no informational representation can replicate. The body's responses to the situation — what feels urgent, what seems to recede, what demands attention — are the beginning of the practical sense that expertise requires. These responses are not available to a learner interacting with representations of the environment.

*The risk of embarrassment*: Dreyfus argued, following Heidegger's analysis of authentic existence, that genuine commitment to a practice requires that one's failures be felt as failures. Online learning, and AI-mediated work, reduce the social stakes of performance in ways that eliminate the emotional investment that drives development beyond Stage 3. The surgical resident who makes an error in the presence of the attending surgeon experiences that error in a way that drives learning. The trainee who makes an error in a simulated or AI-mediated environment does not experience the same force. The emotional dimension of skill acquisition is not incidental to its effectiveness; it is constitutive of the transition from competent to proficient.

*The master's embodied demonstration*: The novice who watches a master perform acquires something that no description of the performance can convey. The master's manner, timing, presence, and the quality of their engagement with the material — what Dreyfus calls their "attunement" to the domain — is transmitted through co-presence and imitation in ways that are systematically unavailable from any mediated or represented account of the same performance. This is the mechanism by which Stage 5 expertise is transmitted across generations; it is the mechanism that AI-driven entry-level automation eliminates not directly but by eliminating the conditions for the apprenticeship relation in which it occurs.

*Ultimate commitment*: Dreyfus draws on Kierkegaard to argue that genuine engagement with a practice requires a form of unconditional commitment — a willingness to stake one's identity on one's choices — that the mediated, risk-reduced environment of online or AI-assisted work does not elicit. The student who knows they can always step back, revise, or disengage has not made the commitment that the developmental trajectory requires. The loss of commitment is not a motivational deficiency; it is a structural consequence of the elimination of genuine risk from the learning environment.

These four conditions — embodied relevance, the risk of embarrassment, the master's embodied demonstration, and ultimate commitment — are precisely what entry-level professional work provides that AI-mediated work cannot. Dreyfus argued this in the context of internet learning in 2001. Its application to the AI-transition debate is direct: the argument is not that AI-produced outputs are worse than human outputs, but that AI-mediated practice destroys the conditions under which the next generation of humans who could produce outputs requiring Stage 5 expertise will develop. This is the "training for obsolescence" argument of Peterson (2025), the intergenerational transmission trap of Ide (2026), and the skill formation concern of Shen and Tamkin (2026) — all derived, independently, from the same structural claim that Dreyfus stated in 2001 and whose roots extend to *Mind over Machine* in 1986 and "Alchemy and Artificial Intelligence" in 1965.

---

## XI. The Undrawn Connection: Dreyfus and Polanyi

The two most comprehensive philosophical accounts of what machine intelligence cannot hold — Dreyfus's absorbed coping and Polanyi's tacit knowing — were developed independently, in parallel, from different starting points, and have never been fully connected in the literature.

Dreyfus drew on Heidegger and Merleau-Ponty. Polanyi drew on Gestalt psychology, the philosophy of science, and his own practice as a research chemist. They were working in adjacent decades: Polanyi's *Personal Knowledge* appeared in 1958, four years before Dreyfus began writing "Alchemy and Artificial Intelligence." Their primary intellectual circles — Polanyi's Manchester and Chicago, Dreyfus's MIT and Berkeley — did not significantly overlap. There is no evidence of direct dialogue.

Yet the structural coincidence of their arguments is exact — and more precise than a simple shared conclusion. Both identify the *same logical structure* of tacit knowing: the integration of subsidiary clues into a focal achievement, in which the subsidiary clues are attended *from* rather than *to*. For Polanyi, the skilled diagnostician attends from the patient's symptoms (subsidiary) to the diagnosis (focal), and the knowing that constitutes diagnosis cannot survive making the symptoms themselves the focal object of attention. For Dreyfus, the expert chess player attends from the board configuration (subsidiary, ready-to-hand) to the good move (focal), and the knowing cannot survive converting the board configuration into an explicit object of analysis. The structure is identical: subsidiary awareness integrated into focal achievement through the practitioner's body and history.

Both argue that this structure is lost when one attempts full articulation: Polanyi's "by attending to them as we would when examining each clue in itself, we would lose sight of the face"; Dreyfus's "the expert who is asked to give reasons for his action is in the position of the centipede asked which leg it moves first — the question can only disrupt what was working fine before it was asked." Both identify the same target: the assumption that all genuine knowledge can be made explicit without loss — the assumption that underlies both classical AI (for Dreyfus) and the received positivist account of science (for Polanyi).

The convergence matters for the framework because it establishes, from two independent lineages, the same structural claim about what machine intelligence cannot hold. Polanyi demonstrates it from the philosophy of science and the practice of research chemistry. Dreyfus demonstrates it from Heidegger's phenomenology and the empirical record of AI's failure pattern. Neither argues from the other. Both arrive at the same bedrock.

---

## XII. What the Dreyfus Lineage Adds to the Framework

The companion READMEs establish the philosophical and economic foundations of the claim that machine intelligence has constitutive limits. The Dreyfus lineage adds four things that those foundations lack.

**Predictive precision**: Dreyfus did not merely argue that machines could not achieve general intelligence. He specified the *form* that AI failure would take: strong performance within closed, formally specified domains; systematic failure at the boundary between those domains and the open-world tasks that require background understanding. This is not a qualitative claim about ultimate limits. It is a structural prediction about the shape of the capability profile — which is exactly the shape the jagged frontier has.

**A developmental theory of the transmission mechanism**: The five-stage model provides the most rigorous account of *why* AI-driven entry-level automation destroys the intergenerational transmission of expertise. It is not enough to say that tacit knowledge is transmitted through communities of practice. One needs to know which parts of practice carry the transmission, and the five-stage model identifies them: the early stages, where the learner operates closest to explicit rule-following, are the stages where the background understanding is first constituted — where the practitioner begins acquiring the experiential residue that eventually produces Stage 5. Automating those stages eliminates the starting condition of the entire developmental trajectory.

**A theory of mediated learning's limits**: "On the Internet" (2001) provides the most direct analysis of why AI-mediated learning cannot replace apprenticeship. Its four conditions — embodied relevance, the risk of embarrassment, the master's embodied demonstration, and ultimate commitment — specify exactly what is lost when the learning environment is mediated by technology in ways that reduce the embodied, at-risk quality of engagement. This analysis applies directly to AI tutoring systems, AI-assisted entry-level work, and any substitution of machine mediation for practitioner-to-practitioner transmission.

**A reception history that is itself analytically informative**: The three cycles of declared refutation and actual vindication are not merely biographical interest. They reveal the first-step fallacy in action across sixty years of AI development — the systematic misidentification of closed-domain achievement as evidence of progress toward open-world capability. Each cycle of "Dreyfus has been refuted" was followed by a cycle of "the capabilities we claimed have not generalized." The reception history is a real-time demonstration of the epistemological confusion that the framework diagnoses.

---

## References

Brooks, R. A. (1986). A robust layered control system for a mobile robot. *IEEE Journal on Robotics and Automation*, 2(1), 14–23.

Brooks, R. A. (1991). Intelligence without representation. *Artificial Intelligence*, 47(1–3), 139–159.

Chollet, F. (2019). On the measure of intelligence. *arXiv:1911.01547*.

Dreyfus, H. L. (1965). *Alchemy and artificial intelligence*. RAND Corporation Paper P-3244.

Dreyfus, H. L. (1972). *What computers can't do: A critique of artificial reason*. Harper & Row.

Dreyfus, H. L. (1979). *What computers can't do: The limits of artificial intelligence* (Rev. ed.). Harper & Row.

Dreyfus, H. L. (1991). *Being-in-the-world: A commentary on Heidegger's Being and Time, Division I*. MIT Press.

Dreyfus, H. L. (1992). *What computers still can't do: A critique of artificial reason*. MIT Press.

Dreyfus, H. L. (2001). *On the Internet*. Routledge.

Dreyfus, H. L. (2012). A history of first step fallacies. *Minds and Machines*, 22(2), 87–99.

Dreyfus, H. L., & Dreyfus, S. E. (1986). *Mind over machine: The power of human intuition and expertise in the era of the computer*. Free Press.

Dreyfus, S. E. (1981). *Formal models vs. human situational understanding: Inherent limitations on the modeling of business expertise*. Office of Naval Research, USAF-AFSC-TR-81-5062.

Dreyfus, S. E., & Dreyfus, H. L. (1980). *A five-stage model of the mental activities involved in directed skill acquisition*. University of California, Berkeley, Operations Research Center (USAF Contract F49620-79-C-0063).

Heidegger, M. (1962). *Being and time* (J. Macquarrie & E. Robinson, Trans.). Harper & Row. (Original work published 1927)

Ide, E. (2026). Automation, AI, and the intergenerational transmission of knowledge. IESE Business School / CEPR Discussion Paper 20940. arXiv:2507.16078. [R&R, *American Economic Review*]

Kapoor, S., Kirgis, P., Schwartz, A., Rabanser, S., Allaire, J. J., Bommasani, R., … Narayanan, A. (2026). Open-world evaluations for measuring frontier AI capabilities. arXiv:2605.20520.

Merleau-Ponty, M. (1962). *Phenomenology of perception* (C. Smith, Trans.). Routledge & Kegan Paul. (Original work published 1945)

Peterson, A. J. (2025). Training for obsolescence? The AI-driven education trap. University of Poitiers. arXiv:2508.19625.

Polanyi, M. (1958). *Personal knowledge: Towards a post-critical philosophy*. University of Chicago Press.

Polanyi, M. (1966). *The tacit dimension*. Doubleday.

Schuering, B., & Schmid, T. (2024). What can computers do now? Dreyfus revisited for the third wave of artificial intelligence. *Proceedings of the AAAI Symposium Series*, 3(1), 248–252.

Shen, J. H., & Tamkin, A. (2026). How AI impacts skill formation. Anthropic Fellows Program. arXiv:2601.20245.

Ward, D. (2018). What's lacking in online learning? Dreyfus, Merleau-Ponty and bodily affective understanding. *Journal of Philosophy of Education*, 52(4), 645–659.

Winograd, T., & Flores, F. (1986). *Understanding computers and cognition: A new foundation for design*. Ablex.

---

*Fifth companion to: README_uncovered.md, README_lineage.md, README_bifurcated.md, and README_parallel_arrivals.md — the Attentional Arbitrage framework*
