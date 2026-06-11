---
layout: post
comments: true
title: "Engineering an Ending"
tags: economics
---

<style>
.zoom-figure { cursor: zoom-in; }
#fig-overlay {
  display: none;
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.82);
  z-index: 9999;
  align-items: center;
  justify-content: center;
  padding: 1.5rem;
}
#fig-overlay.open { display: flex; }
#fig-overlay svg {
  max-width: min(95vw, 900px);
  max-height: 90vh;
  width: 100%;
  height: auto;
  background: #fafafa;
  border-radius: 4px;
  padding: 1.25rem;
  box-sizing: border-box;
}
#fig-overlay-close {
  position: fixed;
  top: 1rem;
  right: 1.25rem;
  color: #fff;
  font-size: 2rem;
  line-height: 1;
  cursor: pointer;
  background: none;
  border: none;
  padding: 0;
}
</style>

*On equilibrium replacement, orphaned costs, and structural change*

Three strands of twentieth-century social science converge on a shared descriptive insight about how change actually occurs in complex systems, even though they are rarely read together.

# Theoretical Foundations

### 1. Game Theory

In non-cooperative settings, locally stable equilibria persist despite being Pareto-suboptimal because no actor can unilaterally improve their payoff by deviating. Once best-response dynamics have settled, incremental improvement efforts tend to be absorbed back into the equilibrium rather than displacing it; escape generally requires changing the game's structure rather than play within it.[^1] Thomas C. Schelling extended this insight beyond equilibrium analysis to show how commitment, irreversibility, and the strategic removal of one's own options can force discrete outcomes without persuasion.[^2] Power, in this sense, operates by altering the feasible set rather than by improving payoffs within it.

Underlying this persistence is a deeper result. Myerson and Satterthwaite (1983) proved that under private information, no bilateral bargaining mechanism can guarantee efficient trade — some gains from trade *must* go unrealised, regardless of how sophisticated the contracting arrangement.[^3] This upgrades "negative space" from an empirical observation to a structural necessity: coordination costs are not orphaned because nobody noticed them, but because bargaining provably cannot resolve them. The absorber is not fixing a market failure that better negotiation could fix; they are substituting an ownership structure for a bargaining problem that has no bargaining solution.

Lipsey and Lancaster's general theory of the second best (1956) supplies a further formal warrant for the anti-incrementalism stance: in a system with multiple distortions, removing one distortion piecemeal can reduce welfare.[^4] Incremental improvement within a constrained equilibrium is not merely slow — it is directionally unreliable. Only changing the constraint set has predictable effects.

### 2. Institutional Economics

Ronald Coase and later Oliver Williamson argued that organizational forms emerge to minimize transaction and coordination costs.[^5][^6] Activities remain in markets until the costs of contracting, monitoring, or bargaining exceed the costs of hierarchical control, at which point boundaries shift. Structural change therefore appears as discontinuous reorganization of governance regimes.

Grossman, Hart, and Moore's incomplete contracts theory sharpens this: because contracts cannot specify every contingency, whoever holds *residual control rights* captures the surplus in renegotiation, which in turn shapes everyone's ex ante investment.[^7][^8] This is the exact theoretical distinction between Apple's App Intents and Rabbit: Apple holds residual control rights over iOS distribution and can therefore mandate intent exposure; Rabbit held only a contractual hope. "Configuring to absorb costs" is, in GHM terms, acquiring residual control over the assets where unabsorbed costs live. Absorption without the adjacent residual control rights merely subsidises other parties' hold-up.

Holmström's budget-breaker result (1982) formalises the absorber's constitutive role: in team production with joint output, no budget-balanced incentive scheme achieves efficiency.[^9] A principal who stands *outside* the team and absorbs the residual is required. PayPal absorbing fraud risk is a budget-breaker for the merchant–buyer–network team; the LBO sponsor is a budget-breaker for the manager–shareholder team. The absorber must take losses onto their own balance sheet — mediation alone cannot do it.

### 3. Political Economy and Sociology

Albert Hirschman distinguished between voice and exit as mechanisms of response to dissatisfaction, emphasising that systems often metabolize voice indefinitely while remaining vulnerable to exit-like pressures that threaten continuity.[^10] James Scott showed that large administrative systems rely on simplified representations of reality and tend to eliminate actors that introduce persistent illegibility.[^11] From this perspective, change occurs when an arrangement exceeds the system's tolerance for ambiguity — not when arguments about improvement become more compelling.

Read prescriptively, this strand identifies a constraint on the *absorber* rather than only the system: an absorber must remain legible and tolerable to the surrounding institutional environment long enough to reach the scale at which the old equilibrium becomes non-viable. Configurations that exceed regulatory or institutional tolerance too early are eliminated before re-equilibration completes — absorption races against expulsion. This is Schelling's commitment logic returning in empirical form: survival through the vulnerable interval is itself a strategic variable.

Acemoglu and Robinson's political losers hypothesis identifies a further veto: inefficient arrangements persist when change would erode the *power* — not just the rents — of those positioned to block it, and credible compensation deals cannot be struck because promises to redistribute power after it has shifted are not enforceable.[^12] The absorber must compensate, route around, or outlast the political losers. Which is feasible depends on the credibility constraints specific to each case.

---

# Historical Examples

### Containerisation

Malcolm McLean's containerisation did not persuade ports and shipping lines to improve break-bulk handling; it created an end-to-end logistics configuration whose cost and speed advantages rendered the prior system obsolete. McLean internalised coordination across modes of transport — truck, rail, ship — that had previously been managed through fragmented handoffs, theft risk, and manual loading. Ports that maintained break-bulk operations could not match the throughput and cost structure once shippers could move sealed containers seamlessly across the supply chain.

Two features of the case are usually omitted and should not be. Vietnam-era military logistics contracts subsidised containerisation's demonstration phase before commercial economics were proven, and the transition required negotiated — and bitterly contested — mechanisation agreements with longshore unions. Absorption of coordination costs was necessary but not sufficient; it was financed and politically protected through its vulnerable interval. This is Schelling's commitment logic returning in empirical form: the capacity to survive the loss-making interval is itself what makes the commitment credible. The political losers (longshore labour) had to be compensated, not simply outcompeted.

<figure markdown="1">
<svg viewBox="0 0 390 252" xmlns="http://www.w3.org/2000/svg">
  <!-- Title -->
  <text x="195" y="16" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="11" font-weight="700" fill="#1a1a1a">Containerisation: cost and throughput</text>
  <text x="195" y="29" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#555">break-bulk vs. container (c. 1956–1964)</text>
  <!-- Panel 1: Loading cost -->
  <text x="195" y="46" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#666">Loading cost ($/ton)</text>
  <!-- Break-bulk: $5.83 → 270px (full bar width) -->
  <text x="74" y="66" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Break-bulk</text>
  <rect x="80" y="53" width="270" height="20" rx="2" fill="#8b3a2a" opacity="0.78"/>
  <text x="354" y="66" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#8b3a2a">$5.83</text>
  <!-- Container: $0.16 → 270*0.16/5.83 ≈ 8px (minimum visible) -->
  <text x="74" y="94" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Container</text>
  <rect x="80" y="81" width="8" height="20" rx="2" fill="#2a4a6b" opacity="0.85"/>
  <text x="93" y="94" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">$0.16</text>
  <text x="195" y="113" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#888">97% reduction</text>
  <!-- Divider -->
  <line x1="15" y1="123" x2="375" y2="123" stroke="#d4d0c8" stroke-width="1"/>
  <!-- Panel 2: Throughput -->
  <text x="195" y="139" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#666">Throughput (tons/gang-hour)</text>
  <!-- Break-bulk: 1.7 → 270*1.7/30 ≈ 15px -->
  <text x="74" y="159" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Break-bulk</text>
  <rect x="80" y="146" width="15" height="20" rx="2" fill="#8b3a2a" opacity="0.78"/>
  <text x="100" y="159" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#8b3a2a">1.7</text>
  <!-- Container: 30+ → 270px (full bar width) -->
  <text x="74" y="187" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Container</text>
  <rect x="80" y="174" width="270" height="20" rx="2" fill="#2a4a6b" opacity="0.85"/>
  <text x="354" y="187" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">30+</text>
  <text x="195" y="206" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#888">&gt;17× gain</text>
  <!-- Source -->
  <text x="195" y="226" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#aaa" font-style="italic">Source: Levinson, The Box (2006), pp. 187, 230.</text>
  <text x="195" y="238" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#aaa" font-style="italic">NYC docks; wages held constant for cost comparison.</text>
</svg>
<div class="caption-wrapper">
<figcaption>The cost advantage made the old equilibrium non-viable at any scale, not merely competitively inferior. At \$0.16 versus \$5.83 per ton, break-bulk ports could not adjust on price; the mode of handling had to be abandoned entirely.</figcaption>
</div>
</figure>

### Nike

Nike's rise demonstrates that standing in negative space sometimes requires deliberate de-verticalisation. In the 1970s–80s, athletic footwear companies like Adidas were vertically integrated manufacturers. Nike separated design and branding from manufacturing, outsourcing production to Asian contractors while controlling the athlete-to-consumer interface. This absorbed the coordination cost between rapid design iteration and low-cost manufacturing — a gap the vertically integrated model could not bridge.

In Baldwin–Clark and Jacobides terms, Nike deliberately commoditised the manufacturing layer to relocate the bottleneck to the design–brand interface it controlled.[^13] Adidas faced a forced choice: maintain their integrated model (high fixed costs, slow iteration) or concede the strategic insight. The case illustrates that absorption and de-verticalisation are not opposites — both are bottleneck engineering, and the relevant question is always which layer is least contestable.

### PayPal

PayPal absorbed fraud risk and settlement complexity that online merchants and card networks had left orphaned. Merchants couldn't afford sophisticated fraud detection, buyers didn't trust giving card numbers to random websites, and card networks pushed liability onto merchants. PayPal stood in that negative space by internalising fraud costs and dispute resolution — acting as Holmström's budget-breaker for the merchant–buyer–card-network team — forcing a reorganisation of online payments around its network. Once this configuration existed, alternatives that left these coordination costs unabsorbed were dominated for a sufficient mass of transactions.

### LBOs

Early LBO practice aimed at collapsing dispersed ownership structures that allowed managerial drift. By concentrating control and introducing hard budget constraints, LBOs forced organisations into a small number of discrete futures — restructuring, sale, or failure — thereby terminating an otherwise stable but inefficient equilibrium. Importantly, LBO firms achieved this while acquiring companies often substantially larger than themselves. The mechanism was not resource dominance but precision in identifying and absorbing the specific agency costs that dispersed shareholders could not resolve.

The LBO record also marks a boundary of the theory: subsequent evidence suggests many buyouts created returns less by absorbing agency costs than by transferring wealth from bondholders, employees, and tax authorities.[^14] The framework therefore requires a distinction between *absorbing* a coordination cost (resolving it, creating value) and merely *relocating* it onto parties with less bargaining power. Only the former produces durable re-equilibration; the latter invites political reversal and does not generate new negative space in a productive direction.

### Apple App Store

Apple's App Store did not reform software distribution through negotiation with carriers or developers; it internalised distribution, billing, trust enforcement, and sandboxing into a single controlled interface. Developers wanting access to iOS users had one path, on Apple's terms. The coordination costs that carriers and fragmented distribution channels had left unresolved — payment processing, malware prevention, update management — became absorbed into Apple's platform infrastructure, making alternative configurations non-competitive for most use cases.

### Stripe

Stripe extended PayPal's pattern into the modern era by absorbing the coordination complexity of global payments infrastructure — regulatory compliance across jurisdictions, multi-currency settlement, payment method diversity, fraud detection, and tax calculation. Where merchants previously assembled these capabilities from multiple vendors with fragmented integration costs, Stripe internalised them into a unified API. The company's value proposition centres explicitly on eliminating financial complexity: working with regulators, financial institutions, payment networks, and wallets so that businesses running on Stripe do not have to.

Stripe illustrates Teece's complementary assets test clearly: absorption succeeded because it positioned the company at a bottleneck complementary asset — the integration layer — that it controls.[^15] Unlike Webvan, which absorbed grocery logistics but owned no bottleneck, Stripe absorbed compliance complexity *and* became the chokepoint. This is the ex ante profitability test the framework requires.

### Rabbit and Humane — Failure Mode I

Rabbit and Humane attempted to layer AI interfaces atop existing app ecosystems without internalising any coordination problem those apps faced. They required Uber, Spotify, and other services to maintain GUI-compatible interfaces for their benefit, but possessed no mechanism to compel this cooperation — no platform authority like Apple's, no absorption of costs that would make compliance inevitable, no dominance on any axis that mattered to the apps themselves. They operated entirely in narrative space (compelling demos, appealing design language) while lacking constraint-space leverage. The apps could simply refuse or ignore them, and continuation of the existing equilibrium remained viable.

The contrast with Apple's App Intents clarifies the distinction. Apple can execute a similar vision of AI-mediated app interaction because it controls the platform layer and can mandate structured intent exposure as a condition of distribution. Apple absorbed the coordination cost of creating a uniform intent layer across millions of apps and can extract the benefit without requiring individual apps to see value in the change.

### Webvan, Iridium, Better Place — Failure Mode II

A second failure mode is more instructive than Rabbit and Humane's, because it cannot be dismissed as lacking leverage. Webvan absorbed the coordination costs of grocery fulfilment; Iridium absorbed the coordination of truly global telephony; Better Place absorbed the battery-ownership and charging-coordination problem for electric vehicles. In each case the orphaned cost was real, correctly diagnosed, and genuinely absorbed — and the absorber died anyway.

The lesson is that costs are sometimes orphaned for a reason: the value released by resolving them, at prevailing technology and demand, is smaller than the cost of absorption. Webvan absorbed logistics but owned no bottleneck. Iridium's cost structure was destroyed by terrestrial cellular before satellite economics matured. Better Place required simultaneous coordination with automakers, regulators, and consumers at a scale no single actor could sustain.

Diagnostic precision must therefore extend beyond identifying the orphaned cost to *pricing it* — asking whether absorption is subsidised by something (declining technology costs, a captive demand base, state contracts, network tipping dynamics) until the configuration becomes self-funding. Teece's complementary assets test is the ex ante filter: does absorbing this cost position you at a bottleneck you can control? If not, absorption destroys value rather than creating it.

**Figure 2 — Case Map: Absorption Completeness vs. Bottleneck Control**

<figure markdown="1" class="zoom-figure">
<div style="position:relative;">
<svg id="casemap-svg" viewBox="0 0 680 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <marker id="ax" markerWidth="8" markerHeight="6" refX="8" refY="3" orient="auto">
      <polygon points="0 0, 8 3, 0 6" fill="#888"/>
    </marker>
  </defs>
  <line x1="80" y1="340" x2="640" y2="340" stroke="#888" stroke-width="1.5" marker-end="url(#ax)"/>
  <line x1="80" y1="340" x2="80" y2="30" stroke="#888" stroke-width="1.5" marker-end="url(#ax)"/>
  <text x="360" y="378" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="11" fill="#4a4a4a">Absorption completeness (cost actually internalised)</text>
  <text x="22" y="190" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="11" fill="#4a4a4a" transform="rotate(-90,22,190)">Bottleneck control (residual rights held)</text>
  <rect x="80" y="185" width="275" height="155" fill="#fdf3f1" opacity="0.7"/>
  <rect x="355" y="185" width="285" height="155" fill="#f0ede6" opacity="0.5"/>
  <rect x="80" y="30" width="275" height="155" fill="#f0ede6" opacity="0.5"/>
  <rect x="355" y="30" width="285" height="155" fill="#eef4ec" opacity="0.7"/>
  <text x="217" y="270" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#8b3a2a" font-style="italic">Absorbs costs, loses rents</text>
  <text x="497" y="270" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#4a4a4a" font-style="italic">Transition state</text>
  <text x="217" y="112" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#4a4a4a" font-style="italic">Controls chokepoint,</text>
  <text x="217" y="124" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#4a4a4a" font-style="italic">limited re-equilibration</text>
  <text x="497" y="112" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#2a6b3a" font-style="italic">Durable re-equilibration</text>
  <line x1="355" y1="30" x2="355" y2="340" stroke="#d4d0c8" stroke-width="1" stroke-dasharray="4,4"/>
  <line x1="80" y1="185" x2="640" y2="185" stroke="#d4d0c8" stroke-width="1" stroke-dasharray="4,4"/>
  <!-- Interactive dots — data-label and data-note drive the tooltip -->
  <circle class="cm-dot" cx="580" cy="60" r="9" fill="#2a4a6b" opacity="0.85" style="cursor:pointer;"
    data-label="Stripe"
    data-note="Absorbed global payments complexity (compliance, multi-currency, fraud) and holds the integration-layer bottleneck. Classic Teece complementary asset position."/>
  <circle class="cm-dot" cx="540" cy="80" r="9" fill="#2a4a6b" opacity="0.85" style="cursor:pointer;"
    data-label="Apple App Store"
    data-note="Absorbed distribution, billing, trust enforcement, and sandboxing. Holds iOS distribution as a mandatory chokepoint — residual control rights over every app on platform."/>
  <circle class="cm-dot" cx="510" cy="110" r="9" fill="#2a4a6b" opacity="0.85" style="cursor:pointer;"
    data-label="Containerisation"
    data-note="McLean absorbed cross-modal coordination costs (theft, fragmented handoffs, loading). Controlled container standards and integrated port/ship/truck infrastructure."/>
  <circle class="cm-dot" cx="490" cy="140" r="9" fill="#2a4a6b" opacity="0.85" style="cursor:pointer;"
    data-label="PayPal"
    data-note="Absorbed fraud risk and settlement complexity for online merchants. Became the network chokepoint; alternatives that skipped fraud absorption were dominated for most buyers."/>
  <circle class="cm-dot" cx="460" cy="100" r="9" fill="#2a4a6b" opacity="0.85" style="cursor:pointer;"
    data-label="Nike"
    data-note="Absorbed design-to-manufacturing coordination by de-verticalising. Relocated the bottleneck to the brand-athlete interface, which it alone controlled. Baldwin–Clark modularity."/>
  <circle class="cm-dot" cx="400" cy="155" r="9" fill="#2a4a6b" opacity="0.75" style="cursor:pointer;"
    data-label="LBOs (contested)"
    data-note="Early buyouts absorbed agency costs from dispersed ownership. Later evidence suggests many transferred wealth from bondholders/employees rather than resolving coordination problems — hence bottom-right position is contested."/>
  <circle class="cm-dot" cx="390" cy="280" r="9" fill="#8b3a2a" opacity="0.85" style="cursor:pointer;"
    data-label="Webvan"
    data-note="Absorbed grocery fulfilment coordination but owned no bottleneck. Competitors could replicate the logistics model; the value released by absorption was smaller than the cost at prevailing demand density."/>
  <circle class="cm-dot" cx="350" cy="300" r="9" fill="#8b3a2a" opacity="0.85" style="cursor:pointer;"
    data-label="Iridium"
    data-note="Absorbed global telephony coordination (satellite coverage) but terrestrial cellular destroyed its cost structure before satellite economics matured. No chokepoint survived the technology shift."/>
  <circle class="cm-dot" cx="420" cy="295" r="9" fill="#8b3a2a" opacity="0.85" style="cursor:pointer;"
    data-label="Better Place"
    data-note="Absorbed battery-ownership and charging-coordination costs for EVs. Required simultaneous buy-in from automakers, regulators, and consumers — no single bottleneck to anchor."/>
  <circle class="cm-dot" cx="140" cy="295" r="9" fill="#8b3a2a" opacity="0.85" style="cursor:pointer;"
    data-label="Rabbit / Humane"
    data-note="Lacked both absorption and leverage. Required Uber, Spotify, etc. to maintain GUI-compatible interfaces with no mechanism to compel compliance. Operated entirely in narrative space."/>
  <text x="80" y="358" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">Low</text>
  <text x="630" y="358" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">High</text>
  <text x="65" y="344" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">Low</text>
  <text x="65" y="36" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">High</text>
</svg>
<!-- Tooltip -->
<div id="cm-tooltip" style="display:none;position:absolute;background:#fff;border:1px solid #d4d0c8;border-radius:4px;padding:10px 14px;max-width:280px;font-family:Helvetica Neue,Arial,sans-serif;font-size:12px;line-height:1.5;color:#1a1a1a;box-shadow:0 2px 8px rgba(0,0,0,0.12);pointer-events:none;z-index:10;">
  <strong id="cm-tooltip-label"></strong>
  <p id="cm-tooltip-note" style="margin:4px 0 0;color:#4a4a4a;"></p>
</div>
</div>
<script>
(function(){
  var svg = document.getElementById('casemap-svg');
  var tip = document.getElementById('cm-tooltip');
  var tipLabel = document.getElementById('cm-tooltip-label');
  var tipNote = document.getElementById('cm-tooltip-note');
  var dots = svg.querySelectorAll('.cm-dot');
  dots.forEach(function(dot){
    dot.addEventListener('mouseenter', function(e){
      tipLabel.textContent = dot.getAttribute('data-label');
      tipNote.textContent = dot.getAttribute('data-note');
      tip.style.display = 'block';
    });
    dot.addEventListener('mousemove', function(e){
      var rect = svg.parentElement.getBoundingClientRect();
      var x = e.clientX - rect.left + 14;
      var y = e.clientY - rect.top - 10;
      if (x + 300 > rect.width) x = e.clientX - rect.left - 294;
      tip.style.left = x + 'px';
      tip.style.top = y + 'px';
    });
    dot.addEventListener('mouseleave', function(){
      tip.style.display = 'none';
    });
  });
})();
</script>
<div class="caption-wrapper">
<figcaption>Cases in the top-right quadrant achieve durable re-equilibration: costs are absorbed <em>and</em> the absorber holds residual control rights at a bottleneck (Teece, 1986; Grossman–Hart–Moore). Bottom-right cases absorbed real orphaned costs but held no bottleneck. Bottom-left cases (Rabbit, Humane) lacked both. <em>Hover each point for case details.</em></figcaption>
</div>
</figure>

**Figure 3 — The Re-Equilibration Cycle**

<figure markdown="1" class="zoom-figure">
<svg viewBox="0 0 680 300" xmlns="http://www.w3.org/2000/svg" style="width:100%;max-width:680px;display:block;">
  <defs>
    <marker id="cycarr" markerWidth="8" markerHeight="6" refX="8" refY="3" orient="auto">
      <polygon points="0 0, 8 3, 0 6" fill="#2a4a6b"/>
    </marker>
  </defs>
  <path d="M 380 65 Q 530 80 570 130" fill="none" stroke="#2a4a6b" stroke-width="1.8" marker-end="url(#cycarr)"/>
  <path d="M 585 175 Q 590 240 510 255" fill="none" stroke="#2a4a6b" stroke-width="1.8" marker-end="url(#cycarr)"/>
  <path d="M 455 268 Q 340 285 230 265" fill="none" stroke="#2a4a6b" stroke-width="1.8" marker-end="url(#cycarr)"/>
  <path d="M 175 252 Q 100 230 100 175" fill="none" stroke="#2a4a6b" stroke-width="1.8" marker-end="url(#cycarr)"/>
  <path d="M 110 125 Q 150 60 295 52" fill="none" stroke="#2a4a6b" stroke-width="1.8" marker-end="url(#cycarr)"/>
  <ellipse cx="340" cy="48" rx="90" ry="32" fill="#e8eef4" stroke="#2a4a6b" stroke-width="1.5"/>
  <text x="340" y="44" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">1. Orphaned costs</text>
  <text x="340" y="58" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">diffused, unresolved</text>
  <ellipse cx="590" cy="152" rx="80" ry="30" fill="#e8eef4" stroke="#2a4a6b" stroke-width="1.5"/>
  <text x="590" y="148" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">2. Absorber</text>
  <text x="590" y="162" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">takes residual loss</text>
  <ellipse cx="490" cy="263" rx="90" ry="30" fill="#e8eef4" stroke="#2a4a6b" stroke-width="1.5"/>
  <text x="490" y="259" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">3. Re-equilibration</text>
  <text x="490" y="273" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">old config. dominated</text>
  <ellipse cx="195" cy="263" rx="90" ry="30" fill="#fdf3f1" stroke="#8b3a2a" stroke-width="1.5"/>
  <text x="195" y="259" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#8b3a2a">4. Ossification</text>
  <text x="195" y="273" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#8b3a2a">absorption → rent</text>
  <ellipse cx="95" cy="148" rx="80" ry="30" fill="#fdf3f1" stroke="#8b3a2a" stroke-width="1.5"/>
  <text x="95" y="144" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#8b3a2a">5. New negative</text>
  <text x="95" y="158" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#8b3a2a">space created</text>
  <text x="340" y="298" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888" font-style="italic">e.g. App Store: distribution absorbed (stage 3) → 30% toll (stage 4) → antitrust / alternative stores (stage 5 → stage 1)</text>
</svg>
<div class="caption-wrapper">
<figcaption>Every successful absorption creates the conditions for the next one. The rent at stage 4 is the new orphaned cost at stage 1.</figcaption>
</div>
</figure>

# Why Incumbents Don't Simply Copy

The pattern as stated leaves a gap: if absorbing orphaned costs is so advantageous, incumbents should absorb them first, or imitate quickly. Adidas did eventually outsource manufacturing; the question is why the window stayed open long enough for Nike to matter. Three asymmetries do the work.

First, *motivation*: absorbing the orphaned cost typically cannibalises the incumbent's existing margin structure, so the expected value of absorption is lower for the incumbent than for the entrant — Arrow's replacement effect applied to organisational strategy.[^16] Second, *architecture*: the incumbent's organisation is itself an equilibrium — internal coordination, career incentives, and asset bases settled around the old boundary — so imitation requires terminating an internal equilibrium, which is exactly as hard as the theory predicts. Third, *time*: by the moment imitation becomes obviously necessary, the absorber often holds network or scale positions that make late absorption non-equivalent. Adidas adopting the Nike model in 1995 is categorically different from Nike deploying it in 1975.

**Figure 4 — The Incumbent Window**

<!--<figure markdown="1" class="zoom-figure">
<svg viewBox="0 0 700 400" xmlns="http://www.w3.org/2000/svg" style="width:100%;max-width:700px;display:block;">
  <defs>
    <marker id="warr" markerWidth="7" markerHeight="5" refX="7" refY="2.5" orient="auto">
      <polygon points="0 0, 7 2.5, 0 5" fill="#888"/>
    </marker>
    <linearGradient id="absGrad" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#2a4a6b" stop-opacity="0.15"/>
      <stop offset="100%" stop-color="#2a4a6b" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <line x1="60" y1="290" x2="660" y2="290" stroke="#888" stroke-width="1.4" marker-end="url(#warr)"/>
  <line x1="60" y1="290" x2="60" y2="30" stroke="#888" stroke-width="1.4" marker-end="url(#warr)"/>
  <text x="360" y="315" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#555">Time</text>
  <text x="18" y="165" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" fill="#555" transform="rotate(-90,18,165)">Magnitude</text>

  <rect x="190" y="35" width="300" height="255" fill="#fffbe6" opacity="0.7"/>
  <line x1="190" y1="35" x2="190" y2="290" stroke="#c8a000" stroke-width="1" stroke-dasharray="4,3"/>
  <line x1="490" y1="35" x2="490" y2="290" stroke="#c8a000" stroke-width="1" stroke-dasharray="4,3"/>
  <text x="340" y="50" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" font-weight="700" fill="#a07800">Incumbent window</text>
  <text x="340" y="62" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#a07800">gap between threat growth and incumbent motivation</text>

  <path d="M60,275 C100,273 155,265 190,258 C230,248 270,225 320,185 C370,145 420,105 470,84 C510,68 560,62 620,58"
        fill="none" stroke="#2a4a6b" stroke-width="2.2"/>
  <text x="630" y="56" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" font-weight="700" fill="#2a4a6b">Absorber</text>
  <text x="630" y="68" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#2a4a6b">advantage</text>

  <path d="M60,280 C120,280 170,279 230,277 C290,274 370,268 430,255 C470,246 490,230 530,195 C570,160 600,140 640,120"
        fill="none" stroke="#8b3a2a" stroke-width="2.2" stroke-dasharray="7,4"/>
  <text x="645" y="118" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" font-weight="700" fill="#8b3a2a">Incumbent</text>
  <text x="645" y="130" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#8b3a2a">motivation</text>
  <text x="645" y="142" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#8b3a2a">to respond</text>

  <line x1="60" y1="155" x2="490" y2="155" stroke="#555" stroke-width="0.8" stroke-dasharray="3,3"/>
  <text x="495" y="152" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#555">imitation</text>
  <text x="495" y="163" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#555">obviously</text>
  <text x="495" y="174" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#555">necessary</text>

  <circle cx="390" cy="155" r="4" fill="#2a4a6b"/>
  <line x1="390" y1="151" x2="390" y2="110" stroke="#2a4a6b" stroke-width="0.9" marker-end="url(#warr)"/>
  <text x="395" y="108" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#2a4a6b">absorber at scale</text>
  <text x="395" y="119" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#2a4a6b">before incumbent acts</text>

  <rect x="68" y="40" width="110" height="70" rx="3" fill="#f5f5f0" stroke="#d4d0c8" stroke-width="1"/>
  <text x="123" y="55" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" font-weight="700" fill="#555">Judo dynamic</text>
  <text x="123" y="67" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#4a4a4a">Staying small keeps</text>
  <text x="123" y="78" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#4a4a4a">fight-or-ignore calc</text>
  <text x="123" y="89" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#4a4a4a">in absorber's favour</text>
  <text x="123" y="102" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#8b3a2a">optimal: grow slowly</text>
  <line x1="178" y1="75" x2="200" y2="240" stroke="#888" stroke-width="0.8" marker-end="url(#warr)"/>

  <line x1="195" y1="290" x2="195" y2="295" stroke="#c8a000" stroke-width="1"/>
  <text x="195" y="304" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#a07800">Nike</text>
  <text x="195" y="314" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#a07800">enters</text>

  <line x1="540" y1="290" x2="540" y2="295" stroke="#8b3a2a" stroke-width="1"/>
  <text x="540" y="304" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#8b3a2a">Adidas</text>
  <text x="540" y="314" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#8b3a2a">finally outsources</text>
  <line x1="195" y1="322" x2="540" y2="322" stroke="#a07800" stroke-width="1"/>
  <line x1="195" y1="318" x2="195" y2="326" stroke="#a07800" stroke-width="1"/>
  <line x1="540" y1="318" x2="540" y2="326" stroke="#a07800" stroke-width="1"/>
  <text x="367" y="336" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#a07800">Nike/Adidas window (~20 yrs): outsourcing = dismantling org identity</text>

  <text x="340" y="350" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8" fill="#555" font-style="italic">Containerisation window was shorter: incumbents could switch modes, but military contracts and union agreements compressed the interval.</text>

  <text x="55" y="294" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">Low</text>
  <text x="55" y="40" text-anchor="end" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#888">High</text>
</svg>
<div class="caption-wrapper">
<figcaption>The incumbent window is the gap between two closing processes: the absorber's advantage compounding and the incumbent's motivation to respond rising. Arrow's replacement effect keeps the red curve flat early — imitation cannibalises the incumbent's own margin, so the expected value of response is low while the absorber is still small. The window closes when imitation becomes obviously necessary, but by then the absorber often holds scale or network positions that make late imitation non-equivalent. Window duration varies by how much imitation requires the incumbent to terminate their <em>own</em> internal equilibrium — Adidas's window stayed open longest because outsourcing manufacturing meant dismantling their organisational identity.</figcaption>
</div>
</figure>
-->

Gelman and Salop's judo economics adds a fourth asymmetry: an entrant's credible commitment to staying small can deter incumbent retaliation during the absorption window, because the incumbent's expected gain from fighting exceeds the expected loss only if the entrant threatens to be large.[^17] Sutton's endogenous sunk costs explain the durability after tipping: once absorption succeeds, escalating sunk investment in the absorbed function makes concentration self-reinforcing.[^18]

The strategy is therefore not merely absorbing the right cost, but absorbing it where these asymmetries protect the interval during which the old equilibrium's non-viability becomes apparent to all participants.

# The Operational Mechanism: Segal's Divide-and-Conquer

The framework's cases share an operational pattern that Segal's contracting-with-externalities analysis formalises.[^19] An absorber facing many parties whose payoffs depend on each other's participation can profitably tip a system from one equilibrium to another by exploiting the externalities among them — including via sequenced, discriminatory offers that make each party's acceptance individually rational even when collective resistance would succeed.

This explains why early participants in new platforms typically receive subsidised terms: McLean gave ports preferential rates; Apple gave early iOS developers the full 70% revenue split before the store had scale; Stripe gave startups free integration support. Each defection from the old equilibrium raises the cost of staying, making the next defection easier to secure. The coalition that "should" defend the old equilibrium fails to form because sequential individual rationality undermines collective action. This is the operational layer between diagnostic precision and re-equilibration: it is how the absorber flips the system rather than simply waiting for it to tip.

**Figure 4a — Why Simultaneous Offers Allow Coalition Resistance**

<figure markdown="1">
<svg viewBox="0 0 380 280" xmlns="http://www.w3.org/2000/svg" style="width:100%;max-width:420px;display:block;margin:0 auto;">
  <!-- Title -->
  <text x="190" y="18" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="11" font-weight="700" fill="#1a1a1a">Simultaneous offers</text>
  <text x="190" y="31" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#666">Coalition resistance viable — focal point exists</text>

  <!-- Matrix border -->
  <rect x="30" y="48" width="320" height="170" rx="3" fill="#fafafa" stroke="#d4d0c8" stroke-width="1"/>

  <!-- Column headers -->
  <text x="215" y="65" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#555" font-style="italic">Others hold out</text>
  <text x="320" y="65" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#555" font-style="italic">Others accept</text>
  <line x1="145" y1="68" x2="350" y2="68" stroke="#d4d0c8" stroke-width="0.8"/>
  <line x1="268" y1="48" x2="268" y2="218" stroke="#d4d0c8" stroke-width="0.8"/>

  <!-- Row headers -->
  <text x="87" y="108" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#555" font-style="italic">A holds out</text>
  <text x="87" y="175" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#555" font-style="italic">A accepts</text>
  <line x1="30" y1="138" x2="350" y2="138" stroke="#d4d0c8" stroke-width="0.8"/>
  <line x1="145" y1="48" x2="145" y2="218" stroke="#d4d0c8" stroke-width="0.8"/>

  <!-- Cell TL: A holds out / Others hold out -->
  <rect x="146" y="69" width="121" height="68" fill="#eef4ec" rx="1"/>
  <text x="206" y="96" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="14" font-weight="700" fill="#2a6b3a">+8</text>
  <text x="206" y="111" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#2a6b3a">old eq. holds</text>
  <text x="206" y="123" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#2a6b3a">coalition wins</text>
  <rect x="146" y="69" width="121" height="68" fill="none" stroke="#2a6b3a" stroke-width="1.8" rx="1" stroke-dasharray="4,2"/>
  <text x="206" y="80" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#2a6b3a">← focal point</text>

  <!-- Cell TR: A holds out / Others accept -->
  <rect x="269" y="69" width="80" height="68" fill="#fdf3f1" rx="1"/>
  <text x="309" y="96" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="14" font-weight="700" fill="#8b3a2a">−4</text>
  <text x="309" y="111" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#8b3a2a">A isolated,</text>
  <text x="309" y="123" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#8b3a2a">non-pivotal</text>

  <!-- Cell BL: A accepts / Others hold out -->
  <rect x="146" y="139" width="121" height="68" fill="#f5f5f0" rx="1"/>
  <text x="206" y="166" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="14" font-weight="700" fill="#555">+3</text>
  <text x="206" y="181" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#555">early-mover</text>
  <text x="206" y="193" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#555">subsidy</text>

  <!-- Cell BR: A accepts / Others accept -->
  <rect x="269" y="139" width="80" height="68" fill="#e8eef4" rx="1"/>
  <text x="309" y="166" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="14" font-weight="700" fill="#2a4a6b">+5</text>
  <text x="309" y="181" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#2a4a6b">new eq.</text>
  <text x="309" y="193" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#2a4a6b">stable</text>

  <!-- Annotation -->
  <text x="190" y="235" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#555">Resistance pays if ≥ k others also hold out.</text>
  <text x="190" y="247" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#555">Simultaneous offers let parties coordinate on top-left.</text>
  <text x="190" y="268" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#888" font-style="italic">Payoffs illustrative; structure from Segal (1999)</text>
</svg>
<div class="caption-wrapper">
<figcaption>When offers arrive simultaneously, each party can reason about collective action. The top-left cell is the focal point: if you expect others to hold out, holding out yields +8. The coalition that should defend the old equilibrium can form.</figcaption>
</div>
</figure>

**Figure 4b — How Sequential Offers Break Coalition Resistance**

<figure markdown="1">
<svg viewBox="0 0 380 310" xmlns="http://www.w3.org/2000/svg" style="width:100%;max-width:420px;display:block;margin:0 auto;">
  <defs>
    <marker id="sarr2" markerWidth="7" markerHeight="5" refX="7" refY="2.5" orient="auto">
      <polygon points="0 0, 7 2.5, 0 5" fill="#555"/>
    </marker>
  </defs>
  <!-- Title -->
  <text x="190" y="18" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="11" font-weight="700" fill="#1a1a1a">Sequential offers</text>
  <text x="190" y="31" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9.5" fill="#666">Each party faces a fait accompli — coalition never forms</text>

  <!-- Party 1 -->
  <rect x="90" y="44" width="200" height="60" rx="3" fill="#e8eef4" stroke="#2a4a6b" stroke-width="1.3"/>
  <text x="190" y="63" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">Party 1 — offered first</text>
  <text x="190" y="77" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Sees: 0 prior acceptances</text>
  <text x="190" y="91" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#2a6b3a">Full subsidy offered. Accepts.</text>
  <text x="190" y="101" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#888" font-style="italic">e.g. McLean preferential port rate</text>

  <!-- Arrow 1→2 -->
  <line x1="190" y1="104" x2="190" y2="128" stroke="#555" stroke-width="1.2" marker-end="url(#sarr2)"/>
  <text x="200" y="121" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#888">1 accepted ↓</text>

  <!-- Party 2 -->
  <rect x="90" y="130" width="200" height="60" rx="3" fill="#edf0f8" stroke="#2a4a6b" stroke-width="1.3"/>
  <text x="190" y="149" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#2a4a6b">Party 2 — offered second</text>
  <text x="190" y="163" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Sees: 1 prior acceptance</text>
  <text x="190" y="177" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#2a6b3a">Holding out now costly. Accepts.</text>
  <text x="190" y="187" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#888" font-style="italic">e.g. Apple 70% split, early devs</text>

  <!-- Arrow 2→n -->
  <line x1="190" y1="190" x2="190" y2="214" stroke="#555" stroke-width="1.2" marker-end="url(#sarr2)"/>
  <text x="200" y="207" font-family="Helvetica Neue,Arial,sans-serif" font-size="8.5" fill="#888">1+2 accepted ↓</text>

  <!-- Party n -->
  <rect x="90" y="216" width="200" height="60" rx="3" fill="#f5f5f0" stroke="#888" stroke-width="1"/>
  <text x="190" y="235" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="10" font-weight="700" fill="#555">Party n — offered last</text>
  <text x="190" y="249" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Sees: fait accompli</text>
  <text x="190" y="263" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#8b3a2a">Resistance individually irrational.</text>
  <text x="190" y="273" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="7.5" fill="#888" font-style="italic">coalition never forms</text>

  <!-- Key insight -->
  <rect x="30" y="287" width="320" height="18" rx="2" fill="#f0ede6" stroke="#d4d0c8" stroke-width="0.8"/>
  <text x="190" y="300" text-anchor="middle" font-family="Helvetica Neue,Arial,sans-serif" font-size="9" fill="#4a4a4a">Each acceptance raises the cost of holding out for the next party.</text>
</svg>
<div class="caption-wrapper">
<figcaption>Sequential offers convert the same coordination game into a chain of individual decisions. Each party's pivotality falls as prior acceptances accumulate; resistance becomes individually irrational even when collective resistance would have succeeded. Early subsidies are not generosity — they are a sequencing device.</figcaption>
</div>
</figure>

# Conclusion

Across these cases, the same pattern recurs. Stable situations persist because coordination costs, decision authority, or risk are diffused such that no actor is compelled to resolve underlying inefficiencies. Structural change arises when an actor stands in the negative space where these costs are orphaned and configures themselves to absorb those specific costs in a way that makes continuation of the prior equilibrium non-viable. The prior arrangement ceases to reproduce itself.

What unifies the game-theoretic, institutional, sociological, and historical accounts is a shift in analytical focus away from improvement within equilibria toward the conditions under which equilibria are replaced altogether. The sophistication lies not in deploying superior resources or pursuing vertical integration as a general strategy, but in diagnostic precision: identifying exactly which coordination costs the current equilibrium leaves unabsorbed, then configuring to absorb specifically those costs — whether through integration, disaggregation, or novel organisational forms — such that alternatives become dominated.

The new equilibrium is not an ending. Absorbed coordination costs tend to ossify into toll positions: the absorber becomes the incumbent, the absorption becomes a rent, and the rent becomes a new orphaned cost borne diffusely by participants who individually cannot resolve it. Apple's App Store, having absorbed distribution, billing, and trust enforcement, is now itself the target of regulatory and competitive attempts at forced re-equilibration. The theory is therefore cyclical rather than terminal: every successful absorption creates the negative space for the next one.

Two scope conditions bound the claim. First, this is a theory of engineered transitions, not of all change: equilibria also collapse from exogenous shocks, demographic drift, and technological obsolescence with no strategic absorber present. Second, absorption need not be performed by a single firm — standards bodies and open protocols (TCP/IP, container dimensions themselves, ISO standards) represent distributed absorption, where a coalition internalises a coordination cost no member could carry alone. What is invariant is not the organisational form of the absorber but the mechanism: someone, or some configuration, must come to stand where the costs were orphaned, in a way the old arrangement cannot survive.

> Complex systems relax into constraints. Change the constraints that bind behaviour, and the system re-equilibrates. Leave constraints unchanged, and no amount of persuasion or incremental effort produces structural transformation — because incremental improvement within a multiply-distorted system has no guaranteed direction (Lipsey–Lancaster), and because bargaining over the resulting inefficiency has no guaranteed solution (Myerson–Satterthwaite).

---

[^1]: Nash, J. F. (1951). [Non-cooperative games.](https://www.jstor.org/stable/1969529) *Annals of Mathematics*, 54(2), 286–295.

[^2]: Schelling, T. C. (1960). *The Strategy of Conflict*. Harvard University Press.

[^3]: If a buyer's value $$v_b$$ and a seller's cost $$c_s$$ are private information drawn from overlapping distributions, there is no mechanism that is simultaneously (i) incentive-compatible, (ii) individually rational, and (iii) budget-balanced, that guarantees trade whenever $$v_b > c_s$$. Even when a deal is mutually beneficial, bilateral bargaining under private information will sometimes fail to produce it. An absorber who internalises the residual entirely substitutes ownership for a bargaining problem that has no bargaining solution. See Myerson, R. B., & Satterthwaite, M. A. (1983). [Efficient mechanisms for bilateral trading.](https://doi.org/10.1016/0022-0531(83)90048-0) *Journal of Economic Theory*, 29(2), 265–281.

[^4]: In a system with $$n$$ first-best Pareto conditions, if one condition is violated and cannot be restored, the constrained optimum generally requires violating some of the remaining $$n-1$$ conditions too. Partial reform — removing distortion $$A$$ while distortion $$B$$ persists — is not guaranteed to improve welfare and may reduce it. The direction of the welfare change depends on the specific second-order cross-effects, which are not in general knowable in advance. See Lipsey, R. G., & Lancaster, K. (1956). [The general theory of second best.](https://doi.org/10.2307/2296233) *Review of Economic Studies*, 24(1), 11–32.

[^5]: Coase, R. H. (1937). [The nature of the firm.](https://doi.org/10.1111/j.1468-0335.1937.tb00002.x) *Economica*, 4(16), 386–405.

[^6]: Williamson, O. E. (1985). *The Economic Institutions of Capitalism*. Free Press.

[^7]: Grossman, S. J., & Hart, O. D. (1986). [The costs and benefits of ownership: A theory of vertical and lateral integration.](https://doi.org/10.1086/261404) *Journal of Political Economy*, 94(4), 691–719.

[^8]: Contracts are always incomplete: some contingencies cannot be specified, verified, or enforced. When a gap arises and the parties must renegotiate, whoever holds *residual control rights* — formal authority over decisions not covered by the contract — captures a disproportionate share of the surplus. This shapes investment incentives ex ante: a party who anticipates being held up in renegotiation underinvests in relationship-specific assets. Ownership matters because it is the institutional form for holding residual control. Applied here: "configuring to absorb costs" is acquiring residual control over the assets where unabsorbed costs live. See Hart, O., & Moore, J. (1990). [Property rights and the nature of the firm.](https://doi.org/10.1086/261729)  *Journal of Political Economy*, 98(6), 1119–1158.

[^9]: In team production, suppose $$n$$ agents each choose effort $$e_i$$, joint output is $$q(e_1, \ldots, e_n)$$, and each agent must receive at least their outside option. If incentive schemes must be budget-balanced — the sum of payments equals output — then no scheme achieves first-best effort from every agent simultaneously. Each agent free-rides, since their marginal contribution is diluted across the team. Holmström's solution is a *budget-breaker*: a principal who stands outside the team, collects output, pays each agent a scheme contingent on total output, and absorbs the residual (positive or negative). With a budget-breaker present, first-best is achievable because the constraint $$\sum s_i(q) = q$$ is dropped — the principal can run a deficit or surplus. Holmström, B. (1982). [Moral hazard in teams.](https://doi.org/10.2307/3003320) *Bell Journal of Economics*, 13(2), 324–340.

[^10]: Hirschman, A. O. (1970). *Exit, Voice, and Loyalty*. Harvard University Press.

[^11]: Scott, J. C. (1998). *Seeing Like a State*. Yale University Press.

[^12]: Acemoglu, D., & Robinson, J. A. (2000). [Why did the West extend the franchise?](https://doi.org/10.1162/003355300554836) *Quarterly Journal of Economics*, 115(4), 1167–1199. See also: Acemoglu, D., & Robinson, J. A. (2006). *Economic Origins of Dictatorship and Democracy*. Cambridge University Press.

[^13]: Baldwin, C. Y., & Clark, K. B. (2000). *Design Rules: The Power of Modularity*. MIT Press. Jacobides, M. G., Knudsen, T., & Augier, M. (2006). [Benefiting from innovation.](https://doi.org/10.1016/j.respol.2006.09.005) *Research Policy*, 35(8), 1200–1221.

[^14]: Kaplan, S. N., & Strömberg, P. (2009). [Leveraged buyouts and private equity.](https://doi.org/10.1257/jep.23.1.121) *Journal of Economic Perspectives*, 23(1), 121–146. For the wealth-transfer critique, see Shleifer, A., & Summers, L. H. (1988). [Breach of trust in hostile takeovers.](https://www.nber.org/papers/w2342) In A. Auerbach (Ed.), *Corporate Takeovers: Causes and Consequences*. University of Chicago Press.

[^15]: The returns from innovation often do not accrue to the innovator, but to whoever controls the *complementary assets* required to commercialise it: manufacturing, distribution, after-sales service, regulatory relationships. If those assets are tightly held and not easily replicated, their owners can hold up the innovator at the commercialisation stage and capture most of the surplus. The innovator wins only when the complementary assets are either generic (freely available) or owned by the innovator themselves. Applied here: an absorber who clears an orphaned cost but does not control the bottleneck complementary assets (the layer through which the new configuration must pass) will find that the rents from their absorption are captured by whoever does control that layer. See Teece, D. J. (1986). [Profiting from technological innovation.](https://doi.org/10.1016/0048-7333(86)90027-2) *Research Policy*, 15(6), 285–305.

[^16]: Arrow, K. J. (1962). [Economic welfare and the allocation of resources for invention.](https://www.nber.org/chapters/c2144) In R. Nelson (Ed.), *The Rate and Direction of Inventive Activity*. Princeton University Press.

[^17]: A small entrant can profitably deter an incumbent's price response by *credibly committing to stay small*. If the entrant caps its capacity at $$k$$ units, then the incumbent's profit from matching the entrant's low price across its entire customer base is $$\pi(\text{match}) = (p_e - c) \cdot (D(p_e) - k)$$, while ignoring the entrant yields $$\pi(\text{ignore}) = (p_I - c) \cdot (D(p_I) - k)$$. For small enough $$k$$, the incumbent prefers to cede the $$k$$ customers rather than cut price for everyone. Stripe's early strategy was precisely judo: by targeting developers and startups that the incumbent acquirers (Chase, Citibank) had no interest in serving, Stripe grew into the market without triggering a price war it could not survive. See Gelman, J. R., & Salop, S. C. (1983). [Judo economics: Capacity limitation and coupon competition.](https://doi.org/10.2307/3003535) *Bell Journal of Economics*, 14(2), 315–325.

[^18]: Sutton, J. (1991). *Sunk Costs and Market Structure*. MIT Press.

<div id="fig-overlay" role="dialog" aria-modal="true">
  <button id="fig-overlay-close" aria-label="Close">&times;</button>
</div>

<script>
(function(){
  var overlay = document.getElementById('fig-overlay');
  var closeBtn = document.getElementById('fig-overlay-close');
  var cloned = null;

  document.querySelectorAll('.zoom-figure').forEach(function(fig){
    fig.addEventListener('click', function(e){
      if (e.target.closest('.cm-dot')) return;
      var svg = fig.querySelector('svg');
      if (!svg) return;
      if (cloned) cloned.remove();
      cloned = svg.cloneNode(true);
      cloned.removeAttribute('id');
      cloned.style.cssText = '';
      overlay.appendChild(cloned);
      overlay.classList.add('open');
      document.body.style.overflow = 'hidden';
    });
  });

  function close(){
    overlay.classList.remove('open');
    if (cloned) { cloned.remove(); cloned = null; }
    document.body.style.overflow = '';
  }

  closeBtn.addEventListener('click', close);
  overlay.addEventListener('click', function(e){ if (e.target === overlay) close(); });
  document.addEventListener('keydown', function(e){ if (e.key === 'Escape') close(); });
})();
</script>

[^19]: Segal's contracting-with-externalities result explains why the coalition defending an old equilibrium often fails to form even when it is collectively rational to do so. When a principal offers contracts to multiple agents and those contracts impose externalities on non-signatories, the agents face a prisoners' dilemma: each agent prefers to sign if others defect (since holding out alone leaves them worse off), so sequential individual rationality unravels collective resistance. The principal can exploit this by offering contracts one at a time. Segal and Whinston's naked exclusion paper extends the logic to exclusionary dealing: an incumbent can sign up buyers to exclusive deals at terms that are individually attractive but collectively disadvantage a more efficient entrant. In the absorber context, this is the mechanism behind sequential coalition-flipping — McLean offering ports preferential rates, Apple giving early developers 70% before the store had scale. Each early adoption raises the cost of staying with the old equilibrium for the next party in line, making defection from the old equilibrium sequentially dominant even if collective resistance would have been viable. See Segal, I. (1999). [Contracting with externalities.](https://doi.org/10.1162/003355399556016) *Quarterly Journal of Economics*, 114(2), 337–388.  See also Segal, I., & Whinston, M. D. (2000). [Naked exclusion.](https://doi.org/10.1257/aer.90.1.296) *American Economic Review*, 90(1), 296–309.
