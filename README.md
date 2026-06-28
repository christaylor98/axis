# Axis

Axis is a philosophy, a paradigm, an idea — a bet that a few simple principles, applied where they usually aren't, can build something that matters.

Nothing here is guaranteed. Until there's evidence, nothing is assumed true.

A few north stars orient the work — by no means the best or only ones:

- **Semantics are load-bearing.** Meaning is the crux of the systems below — the lens for finding direction in a never-ending sea of possibilities, and for deciding better.
- **UNKNOWN is a first-class state.** A simple idea doing outsized work: it turns open systems closed, and shuts the long tail of gaps that plague security loops of every shape and size.
- **Immutability.** Not new — applied harder. The route to systems that are reliable, predictable, and auditable by construction.
- **First principles.** Strip every layer to what's load-bearing. If it isn't, drop it.
- **Built for AI.** This began as a language designed specifically for AI to use. The shape has moved on; the ethos hasn't.

As much as it's AI-forward, it's equally about *governing* AI: keeping it auditable and transparent, and — where accuracy is non-negotiable — removing it from the operational loop altogether. Immutable ledgers so nothing can be altered after the fact. Data security embedded down to the language and compilation level. Transparency by construction, not bolted on.

None of this is new or revolutionary. It's building on what we already know and pushing it into places it isn't normally applied.

I hope it inspires you, maybe informs you. I hope you attack every idea here ruthlessly — and that we push the boundaries of human knowledge forward and find something of real use.

## The thesis

**Meaning is the primitive.** Most systems treat meaning as something you recover after the fact — by parsing, by inference, by convention. Axis declares it up front and makes it the canonical form.

Three strata — every design decision is just routing a fact to its owning stratum, with one epistemic state, **UNKNOWN**, cutting across all three:

```
 ┌─ the three strata ───────────────────────────────────────┐
    CORE IR    meaning      the canonical, content-addressed form
    REGISTRY   definition   the closed set of what can be called
    LEDGER     event        what happened, append-only
 └───────────────────────────────────────────────────────────┘
    UNKNOWN  spans all three. A fact that can't be decided —
    a call not in the registry, an input matching no rule — is
    named, not guessed and not hidden: that is what closes the
    gaps the other three would otherwise leave open.
```

One cognitive move applied everywhere: strip to the irreducible core, drop the assumptions that don't earn their place, rebuild from what's actually true.

# Outline

Axis is a loose collection of projects based around the ideas above. Currently it's composed of the following:

```
 Axis — a method, not a pile.  One lens (meaning),
 one engine (structural import across domains), many arms:

   ├── axStack    the compute stack
   └── biology    the lens, pointed at the genome
```

Tiers:  🟢 **Built** (runs today)  ·  🔵 **Building** (active, partial)  ·  🟡 **Designed** (specified, no code)  ·  ⚪ **Sketched** (on the palette). *(Colour is a scan aid; the word is authoritative.)*

## axStack — the compute stack

```
 build path:  axlang + bridge  →  axAI  →  axHost / axOS  →  axDisplay  →  First Drop

 the stack    (top = surface · bottom = foundation)

   ┌ surface    [Designed]  axDisplay
   │ run        [Designed]  axHost / axOS
   │ resources  [Sketched]  axStorage · axCompute · axSatellite
   │ generate   [Building]  axAI / Mechanical AI
   └ foundation [Built]     axlang + bridge + axVerity

     alongside  [Building]  axSemantica · axPlanner · Chronicle   (control & knowledge)
     on top     [mixed]     axAporia · ax-workflow · AI Factory   (applications)
```

**First Drop** is the near-term proof — the stack booting and showing a live Chronicle through its own surface.

**Core**
- 🟢 [axlang / Semantic Calculus](https://github.com/christaylor98/axis-lang-lab) — the language; a closed callable space where an undeclared call cannot exist. **Built**
- 🟢 [bridge](https://github.com/christaylor98/axis-codegen-bridge-rs) — the sole effect boundary; ejects Core IR to native Rust. **Built**
- 🔵 axVerity — immutable content-addressed store; hash is identity; the immutable-ledger backbone behind the auditing theme. **Building**
- 🟢 axRegistry — the canonical registry; ground truth for what can be called. **Built**
- 🔵 axAI / Mechanical AI — mechanical code-gen from the IR; the lever for taking AI *out* of operational loops. **Building**

**Runtime & resources**
- 🟡 axHost / axOS — the same codebase on Linux as an on-ramp; the boundary pushed down over time. **Designed**
- ⚪ axStorage — distributed, encrypted semantic fabric; storage as a location-independent layer. **Sketched**
- ⚪ axCompute — shared compute plane; pure functions migrate to where the data and capacity are. **Sketched**
- ⚪ axSatellite — ambient connectivity fabric; makes axStorage and axCompute genuinely global; location becomes irrelevant. **Sketched**
- 🟡 axDisplay — the surface layer; minimal bridge, no business logic. **Designed**

**Control & knowledge**
- 🔵 axSemantica — the intent graph and control loop the build itself runs on. **Building**
- 🔵 axPlanner — the planning loop; markdown plan + LLM as runtime; compute-for-decisions. **Building**
- 🔵 Chronicle — associative knowledge store; persistence across sessions. **Building**

**Applications & governance**
- 🟡 axAporia — autonomous-vehicle controller; never acts during UNKNOWN. **Designed**
- 🔵 [ax-workflow](https://github.com/christaylor98/axis-workflow-demo) — semantic workflow; UNKNOWN as a governed state, policy clauses as code. **Building**
- 🔵 [AI Factory](https://github.com/christaylor98/ai-factory) — governance-first AI execution; auditable gates, immutable ledger; fraud-detection PoC. **Building**

## The biology arm

The same lens, pointed at the genome — evidence it generalises past computing.

- 🔵 Contextual Commitment Theory — cell state as context-dependent commitment; within- vs between-sample coherence as the load-bearing measurement. **Building**
- 🔵 bio pipeline — the genomic analysis pipeline behind CCT. **Building**

## Anticipated, not yet specified

Named so they're on the palette, not claimed: sovereign comms (axComms), semantic event loops, log compression.
