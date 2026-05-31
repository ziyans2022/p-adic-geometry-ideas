-----

## name: p-adic-geometry-ideas
description: >
Use this skill to generate and analyze open problems, research directions, and
conjectures in p-adic geometry and arithmetic geometry. Activate whenever the
user mentions any of: perfectoid spaces, p-adic Hodge theory, prismatic cohomology,
prismatic F-gauges, Breuil–Kisin modules, (φ,Γ)-modules, rigid analytic geometry,
adic spaces, Berkovich spaces, p-adic Langlands, Fargues–Fontaine curve, diamonds,
v-sheaves, syntomic cohomology, p-adic representations, Galois representations,
period rings (B_dR, B_cris, B_st), local Shimura varieties, eigenvarieties,
p-divisible groups, Dieudonné theory, overconvergent F-isocrystals,
non-archimedean geometry, p-adic Simpson correspondence, non-abelian p-adic Hodge
theory, Higgs bundles rigid analytic, v-bundles, Hodge–Tate stack, Sen operator,
Cartier–Witt stack, smoothoid spaces, diamantine Picard, p-adic Corlette–Simpson,
AGT correspondence, or Faltings Simpson. Also activate for vague prompts such as:
“what should I work on”, “find me a research problem”, “what’s open in [area]”,
“suggest a direction”, “what are good problems for a postdoc”, “what’s hot right now
in arithmetic geometry”, “help me brainstorm a paper topic”, or any question about
feasibility or scope of a research project in these areas.

# P-adic Geometry: Open Problems & Research Idea Generator

**Audience**: Postdoc / early-career researcher with broad expertise across p-adic geometry.  
**Goal**: Produce structured, mathematically precise open problem analyses and research directions.  
**References**: See `references/key_papers.md` for literature and `references/arxiv_guide.md` for search strategy.

-----

## Output Format

For each problem, always use this structure:

### [Problem Title]

**Sub-area**: (e.g. Prismatic cohomology, p-adic Langlands, …)  
**Difficulty**: ★☆☆ Accessible / ★★☆ Substantial / ★★★ Major open problem  
**Time horizon**: Short-term (1–2 yr) / Medium-term (3–5 yr) / Long-term (5+ yr)

**Background**: 2–4 sentences of precise mathematical context. State relevant theorems with precise hypotheses; use correct notation (e.g. distinguish B_dR from B_cris, F-gauge from F-crystal, adic space from Berkovich space).

**Current state**: Who has done what, and exactly where does the gap lie. Name specific papers and results. Be explicit: “X is proved; Y is not known; Z is folklore but unwritten.”

**The problem**: A sharp formulation — ideally a precise conjecture, a missing functor with expected properties, or an explicit diagram that should commute. Use mathematical notation where it clarifies.

**Why it’s interesting**: Broader significance — what does a solution unlock, which other problems does it unblock (reference problem IDs).

**Entry point — first concrete step**: Not a vague reading suggestion, but a specific lemma to prove, a special case to verify, or a computation to do. State it as an actionable task.

**Prerequisites**: List 2–3 papers to read before starting, with a one-line description of what each contributes.

**Depends on** / **Unlocks**: Explicit dependency graph entries (reference other problem IDs).

-----

## Sub-area Reference Map

### Perfectoid Spaces & Diamonds

Key figures: Scholze, Kedlaya, Bhatt, Weinstein, Hansen  
Core tools: Tilting equivalence, pro-étale site, diamonds, v-sheaves, Banach–Colmez spaces  
Hot frontiers: Stacky extensions, 6-functor formalism, geometry of L-parameter stacks

### p-adic Hodge Theory

Key figures: Fontaine, Berger, Colmez, Kisin, Brinon, Caraiani  
Core tools: Period rings (B_dR, B_cris, B_st), (φ,Γ)-modules, Wach modules, Breuil–Kisin–Fargues modules  
Hot frontiers: Relative theory over non-perfect bases, integral p-adic Hodge theory, prismatic comparisons

### Prismatic Cohomology

Key figures: Bhatt–Scholze, Bhatt–Lurie, Drinfeld, Anschütz–Le Bras  
Core tools: Prisms, (φ,δ)-rings, Nygaard filtration, F-crystals, prismatic F-gauges, q-de Rham  
Hot frontiers: Motivic aspects, stacky prismatic cohomology, semi-stable prisms, syntomic cohomology

### Rigid Analytic Geometry

Key figures: Tate, Raynaud, Berkovich, Huber, de Jong, Kedlaya, Liu  
Core tools: Adic spaces, Berkovich spaces, formal models, alterations, solid modules  
Hot frontiers: 6-functor formalism (Mann), non-archimedean RH correspondence, solid geometry

### p-adic Langlands Program

Key figures: Colmez, Breuil, Emerton, Fargues–Scholze, Hellmann, Zhu, Paškūnas  
Core tools: (φ,Γ)-modules, completed cohomology, FF-curve, local Shimura varieties, Shtuka spaces  
Hot frontiers: GL_n beyond GL_2(Q_p), categorical Langlands, coherent sheaves on L-parameter stacks

### p-adic Simpson Correspondence

Key figures: Faltings, Abbes–Gros–Tsuji, Heuer, Anschütz–Le Bras, Min–Wang, Heuer–Xu  
Core tools: Higgs bundles, pro-étale vector bundles, v-bundles, Hodge–Tate stack, Cartier–Witt stack, Sen theory, smoothoid spaces  
Hot frontiers: Non-abelian (G-bundle) Simpson in higher dimensions, derived Simpson functor essential image, non-proper case, integral theory via prismatic methods

-----

## Idea Generation Protocol

1. **Clarify scope** if needed: sub-area, project length (paper vs. program), background constraints.
1. **Generate 3–5 problems** with variety:
- ≥1 ★☆☆ accessible (paper within 1–2 years)
- ≥1 ★★☆ substantial (research program)
- ≥1 cross-sub-area (e.g. prismatic + Langlands, perfectoid + motivic)
1. **Cross-reference**: After listing, note which problems interact and could form a coherent program.
1. **Dependency map**: Draw explicit arrows between the selected problems (e.g. “PR4 → X8 → L7”).
1. **arXiv pointer**: Direct the user to `references/arxiv_guide.md` for current search strategy.

-----

## Open Problems Bank

Each entry follows: **ID** | Difficulty | one-line summary | then full structured description.
For full Output Format expansion of any entry, follow the template above.

-----

### Perfectoid Spaces & Diamonds (P)

-----

**P1** ★☆☆ — Pro-étale comparison for non-smooth rigid spaces

**Current state**: Scholze (2013) proved the pro-étale comparison theorem $H^**{\text{proét}}(X, \hat{\mathbb{Z}}*\ell) \cong H^**{\text{ét}}(X, \mathbb{Z}*\ell)$ for smooth rigid spaces $X$ over a perfectoid field. The non-smooth case is open; de Jong’s alterations give a resolution strategy but the descent argument has not been written down.

**The problem**: Let $X$ be a qcqs rigid analytic space over $\text{Spa}(C, C^+)$, $C$ algebraically closed perfectoid. Using de Jong’s alterations $\tilde{X} \to X$ with $\tilde{X}$ smooth, prove that $R\Gamma_{\text{proét}}(X, \hat{\mathbb{Z}}_\ell)$ satisfies cohomological descent along the alteration, and deduce the comparison with étale cohomology.

**Entry point — first concrete step**: Verify descent for the structure sheaf $\hat{\mathcal{O}}_X$ along a single alteration in the case $X = \text{Spa}(A)$ with $A$ having a single ordinary double point. This reduces to an explicit calculation with almost mathematics.

**Prerequisites**: Scholze’s pro-étale paper (2013); de Jong’s alterations paper (1996); Gabber–Ramero “Almost Ring Theory” Ch. 5.

**Depends on**: — | **Unlocks**: P2 (the non-representable morphism case in 6-functors needs P1 as input), R3

-----

**P2** ★★☆ — Complete 6-functor formalism for diamonds

**Current state**: Hansen (thesis, 2020) constructed $f_!$ and $f^!$ for compactifiable morphisms of diamonds. The gap is non-compactifiable and non-representable morphisms (e.g., the map $\text{Spd}(\mathbb{Z}_p) \to *$), and the full projection formula and base change in this generality. Hansen–Scholze have announced further work but it is not yet public.

**The problem**: Construct a full 6-functor formalism ${f^*, f_*, f_!, f^!, \otimes^L, R\mathcal{H}om}$ for étale sheaves on the category of small v-stacks, satisfying: (i) proper base change, (ii) projection formula, (iii) Verdier duality relative to a dualizing complex. Verify the formalism for $\mathbb{B}^1_{\text{FF}} \to \text{Spd}(\mathbb{Q}_p)$.

**Entry point — first concrete step**: Construct $f_!$ for the map $f: \mathcal{M}_\infty \to \text{Spd}(\mathbb{Q}*p)$ where $\mathcal{M}*\infty$ is the Lubin–Tate tower at infinite level; verify the Künneth formula in this case.

**Prerequisites**: Hansen’s thesis; Scholze–Weinstein “Berkeley Lectures” Ch. 22–23; Mann’s thesis (2022) for the p-adic analogue.

**Depends on**: P1 | **Unlocks**: P4, X2, L2

-----

**P3** ★★☆ — Geometry of Banach–Colmez spaces for general de Rham representations

**Current state**: Fargues–Fontaine constructed Banach–Colmez spaces $\mathcal{H}^i(V)$ as “spaces of $H^i$” for a de Rham $(\varphi, \Gamma)$-module $V$ over the FF-curve $X_{FF}$. For $V$ de Rham with distinct Hodge–Tate weights, $\mathcal{H}^0(V)$ is understood (it is a successive extension of $\mathbb{B}^1$’s). For non-de Rham $V$ or repeated HT weights, the geometry is not described.

**The problem**: For a semi-stable representation $V$ with monodromy $N \neq 0$, describe the Banach–Colmez space $\mathcal{H}^0(V)$ as a diamond; specifically, identify the reduced subspace and the formal completion along the special fiber. Conjecture: $\mathcal{H}^0(V)$ is an extension of a unipotent group diamond by a product of $\mathbb{B}^1$’s, with $N$ encoding the extension class.

**Entry point — first concrete step**: Work out the case $V = B_{\text{st}}^{\varphi=p, N\neq 0}$ (the non-crystalline rank-2 semi-stable representation). Write down the explicit transition matrices in the Fargues–Fontaine description and identify the geometric fiber.

**Prerequisites**: Fargues–Fontaine “Courbe” (2018) Ch. 8; Colmez “Espaces de Banach” (2002); Scholze–Weinstein Ch. 11.

**Depends on**: — | **Unlocks**: P4, L6, X3

-----

**P4** ★★★ — Perverse sheaves on diamonds with a good t-structure

**Current state**: On $\ell$-adic sheaves over schemes, the perverse t-structure is well-established (BBD 1982). For diamonds, Hansen–Scholze have $\ell$-adic sheaf categories but no t-structure with good properties (e.g. noetherian heart, stability under $f_*$ for proper $f$) has been constructed. The obstruction is the lack of a dimension theory for general v-stacks.

**The problem**: Construct a perverse t-structure on $D(X_{\text{proét}}, \mathbb{Z}*\ell)$ for a locally spatial diamond $X$ of finite $\ell$-cohomological dimension. Verify: (i) the heart is noetherian when $X$ is spatial; (ii) $IC_Z(\mathbb{Z}*\ell)$ exists for any locally closed spatial sub-diamond $Z \hookrightarrow X$; (iii) $f_*$ is t-exact for proper $f$.

**Entry point — first concrete step**: Define the perverse truncation functors ${}^p\tau_{\leq 0}$ on $D(\text{Spd}(C), \mathbb{Z}_\ell)$ for $C$ algebraically closed perfectoid, and verify this gives the correct answer on locally constant sheaves.

**Prerequisites**: BBD “Faisceaux Pervers” (1982) Ch. 1–2; Hansen “Towards a 6-functor formalism” (2020); Scholze–Weinstein Ch. 24.

**Depends on**: P2 | **Unlocks**: R12, L2

-----

**P5** ★☆☆ — Coherent cohomology of L-parameter stacks for tori

**Current state**: For a torus $T$ over $\mathbb{Q}*p$, the L-parameter stack $Z^1(W*{\mathbb{Q}*p}, \hat{T})/\hat{T}$ is relatively explicit — $\hat{T}$ is also a torus, so the stack is a quotient of a smooth variety. But the coherent cohomology $H^*(Z^1(W*{\mathbb{Q}_p}, \hat{T})/\hat{T}, \mathcal{O})$ has not been computed, and its relation to smooth representations of $T(\mathbb{Q}_p)$ has not been verified directly.

**The problem**: For $T = \mathbb{G}_m$ (so $\hat{T} = \mathbb{G}*m$, and $Z^1(W*{\mathbb{Q}_p}, \mathbb{G}_m)/\mathbb{G}_m$ classifies characters), compute $\text{Ext}^*$ between line bundles on this stack and match the result with extensions between smooth characters of $\mathbb{Q}_p^\times$ via local class field theory.

**Entry point — first concrete step**: Write down the functor of points of $Z^1(W_{\mathbb{Q}_p}, \mathbb{G}_m)/\mathbb{G}_m$ as an adic space explicitly; identify the connected components as eigenvariety-style spaces.

**Prerequisites**: Fargues–Scholze “Geometrization” (2021) Ch. I; Emerton–Gee–Hellmann survey (2022) §3.

**Depends on**: — | **Unlocks**: L5, L11

-----

**P6** ★★☆ — Stratified homotopy theory for diamonds

**Current state**: Barwick–Glasman–Haine developed a theory of exodromy equivalences: for a stratified scheme $(X, S)$, locally constant sheaves on the strata are equivalent to representations of a “profinite stratified fundamental groupoid.” This works for schemes and their étale sites. No analogue exists for diamonds or v-stacks, despite the fact that many natural diamonds (e.g., $\text{Spd}(\mathbb{Z}_p)$) have natural stratifications.

**The problem**: For a locally spatial diamond $X$ with a finite stratification by locally closed sub-diamonds $X = \bigsqcup_i X_i$, construct an exodromy equivalence $\text{Loc}(X) \simeq \text{Fun}(\Pi_1^{\text{strat}}(X), \text{Vect})$ where $\Pi_1^{\text{strat}}(X)$ is an appropriate stratified condensed groupoid. Verify for $X = \text{Spd}(\mathbb{Z}_p)$ with its generic/special fiber stratification.

**Entry point — first concrete step**: Compute $\Pi_1^{\text{strat}}(\text{Spd}(\mathbb{Z}_p))$ explicitly: the generic fiber stratum is $\text{Spd}(\mathbb{Q}*p)$ with $\pi_1 = G*{\mathbb{Q}_p}$, the special fiber is $\text{Spd}(\mathbb{F}_p)$ with $\pi_1 = \hat{\mathbb{Z}}$, and the specialization map should be the cyclotomic character. Check this matches the known description of local systems on $\text{Spd}(\mathbb{Z}_p)$.

**Prerequisites**: Barwick–Glasman–Haine “Exodromy” (2020); Scholze–Weinstein Ch. 15–17.

**Depends on**: P2 | **Unlocks**: P9, R9

-----

**P7** ★☆☆ — Tilting for perfectoid algebras over ramified bases

**Current state**: Scholze–Weinstein prove tilting $(-)^\flat$ as an equivalence between perfectoid algebras over $\text{Spa}(C, C^+)$ (algebraically closed) and their characteristic-$p$ tilts. Over a ramified base $\text{Spa}(K, \mathcal{O}_K)$ with $K/\mathbb{Q}_p$ totally ramified of degree $e$, the tilting functor exists but the equivalence breaks: the tilt depends on the choice of uniformizer up to non-canonical isomorphism. The precise functoriality in the ramification data has not been worked out.

**The problem**: For a totally ramified extension $K/\mathbb{Q}_p$ with uniformizer $\pi$ satisfying an Eisenstein polynomial $E(u) = 0$, describe the category of perfectoid $\mathcal{O}_K$-algebras in terms of characteristic-$p$ data. Specifically: formulate the correct “ramified tilt” functor $(-)^{\flat, \pi}$ and prove it is an equivalence onto an explicit subcategory of perfectoid $\mathcal{O}_K^\flat$-algebras equipped with a “Frobenius-twisted $E$-structure.”

**Entry point — first concrete step**: Work out the case $K = \mathbb{Q}_p(\zeta_p)$ (cyclotomic extension, $e = p-1$), where the Frobenius twist of $E(u) = \Phi_p(u+1)$ has an explicit form. Verify that the Witt vector construction recovers $\mathcal{O}_K$ from $\mathcal{O}_K^\flat$.

**Prerequisites**: Scholze–Weinstein Ch. 6–7; Kisin–Ren “Galois representations and Lubin–Tate extensions” (2015).

**Depends on**: — | **Unlocks**: H1, PR4

-----

**P8** ★★☆ — Schematic points of Spd(Z_p) and their prismatic meaning

**Current state**: The diamond $\text{Spd}(\mathbb{Z}_p)$ has two obvious “points”: the generic point $\text{Spd}(\mathbb{Q}_p)$ and the special point $\text{Spd}(\mathbb{F}_p)$. But as a diamond, it has many more points (corresponding to untilts of perfectoid fields in characteristic $p$). Bhatt–Scholze show that the prismatic site of $\mathbb{Z}_p$ is closely related to $\text{Spd}(\mathbb{Z}_p)$, but the precise dictionary between “points of $\text{Spd}(\mathbb{Z}_p)$” and “prisms over $\mathbb{Z}_p$” has not been made into a theorem.

**The problem**: Prove an equivalence between: (i) the full subcategory of “bounded prisms $(A, I)$ with $A/I$ a perfectoid ring” in the absolute prismatic site $(\mathbb{Z}*p)*\Delta$, and (ii) the category of morphisms $\text{Spd}(R, R^+) \to \text{Spd}(\mathbb{Z}_p)$ for $(R, R^+)$ a perfectoid Huber pair. Make the equivalence functorial in maps of prisms.

**Entry point — first concrete step**: Work out the dictionary explicitly for the Breuil–Kisin prism $(\mathbb{Z}_p[[u]], (E(u)))$ and identify the corresponding point of $\text{Spd}(\mathbb{Z}_p)$ — it should be the “Lubin–Tate point” corresponding to the formal group of $\mathbb{Q}_p$.

**Prerequisites**: Bhatt–Scholze “Prisms and Prismatic Cohomology” (2022) §2–3; Scholze–Weinstein §18.

**Depends on**: — | **Unlocks**: PR1, X1

-----

**P9** ★★★ — D-modules on diamonds / adic spaces

**Current state**: Ardakov–Wadsley developed a theory of $\hat{\mathcal{D}}$-modules on smooth rigid analytic spaces (completed PD-differential operators). This theory is purely characteristic-0 and rigid-analytic. On the diamond/v-stack side, there is no analogue. Such a theory would be essential for a non-archimedean version of the geometric Langlands program, but even the definition of “differential operator” on a diamond is unclear (the pro-étale site has no tangent sheaf).

**The problem**: Define a category of “solid $\hat{\mathcal{D}}$-modules” on a smooth adic space $X$ over $\text{Spa}(\mathbb{Q}_p, \mathbb{Z}_p)$ in the framework of solid quasi-coherent sheaves (Clausen–Scholze), and prove it agrees with Ardakov–Wadsley’s $\hat{\mathcal{D}}$-modules for Stein spaces. As a test case, recover the $\hat{\mathcal{D}}$-module associated to a de Rham local system (Liu–Zhu).

**Entry point — first concrete step**: In Clausen–Scholze “Analytic Stacks,” identify the solid structure sheaf $\mathcal{O}^{\text{solid}}_X$ on a smooth adic space and compute $\mathcal{E}xt^i(\mathcal{O}_X, \mathcal{O}_X)$ — the answer should encode the cotangent complex. Check this against Ardakov’s computation for the open unit disk.

**Prerequisites**: Ardakov–Wadsley “On irreducible representations of compact p-adic analytic groups” (2013); Clausen–Scholze “Analytic Stacks” lecture notes (2023); Liu–Zhu “Rigidity” (2017).

**Depends on**: P2, R4 | **Unlocks**: L9

-----

**P10** ★☆☆ — v-cohomology of local Shimura varieties for Sp_4 and U(3)

**Current state**: Fargues–Scholze compute the cohomology of local Shimura varieties for $GL_n$ as a bimodule for $GL_n(F) \times W_F$ and extract the local Langlands correspondence. For classical groups $Sp_4$ and $U(3)$, the local Shimura varieties are known (they are related to spinor/unitary Rapoport–Zink spaces), but their v-cohomology in the Fargues–Scholze framework has not been computed.

**The problem**: For $G = Sp_4$ and the minuscule cocharacter $\mu = (1,1,0,0)$, compute $H^**c(\mathcal{M}*{Sp_4, \mu, \infty}, \overline{\mathbb{Q}}_\ell)$ as a $Sp_4(\mathbb{Q}*p) \times W*{\mathbb{Q}_p}$-module, and identify which L-parameters appear (expected: generic parameters for $GSp_4$, consistent with the classical LLC for $Sp_4$).

**Entry point — first concrete step**: Using the Hodge–Tate period map $\pi_{HT}: \mathcal{M}*{Sp_4, \mu, \infty} \to \mathcal{F}\ell*{Sp_4, \mu}$, compute the cohomology of the flag variety $\mathcal{F}\ell_{Sp_4, \mu}$ as an $Sp_4(\mathbb{Q}_p)$-representation — this is classical Bruhat decomposition and gives the leading term.

**Prerequisites**: Fargues–Scholze “Geometrization” Ch. VII; Rapoport–Viehmann “Towards a theory of local Shimura varieties” (2014); Kaletha–Weinstein “On the Kottwitz conjecture for local Shimura varieties” (2023).

**Depends on**: P2 | **Unlocks**: L4, X7

-----

### p-adic Hodge Theory (H)

-----

**H1** ★★☆ — Relative p-adic Hodge theory over non-perfect residue fields

**Current state**: Kedlaya–Liu (2015, 2016) developed relative p-adic Hodge theory for smooth families $f: X \to S$ of rigid spaces when $S = \text{Spa}(A, A^+)$ with $A$ a Tate algebra over $\mathbb{Q}_p$ (perfect residue field $\mathbb{F}_p$). The case when $S$ has non-perfect residue field — e.g., $S = \text{Spa}(\mathbb{Q}*p{t^{1/p^\infty}})$ or families over function field bases — is not covered. The obstruction is that the “relative period ring” $B*{\text{dR}}(A)$ requires $A$ to be perfectoid.

**The problem**: For a smooth proper morphism $f: X \to S$ with $S = \text{Spa}(A, A^+)$ where $A$ is an arbitrary reduced Tate $\mathbb{Q}*p$-algebra, construct a relative $(\varphi, \Gamma)$-module $\mathbb{D}(R^n f** \mathbb{Z}_p)$ over the relative Robba ring $\mathcal{R}_A$. Specifically: (i) define $\mathcal{R}_A$ for non-perfect $A$ using Kedlaya’s ramification-theoretic approach; (ii) prove the overconvergence of the associated isocrystal.

**Entry point — first concrete step**: Define $B_{\text{dR}}^+(A)$ for $A = \mathbb{Q}*p\langle t \rangle$ (Tate algebra in one variable) by taking the completed PD-envelope of $W(A^\flat) \to A$; compute $B*{\text{dR}}^+(A)/(t)$ and verify it equals $A$.

**Prerequisites**: Kedlaya–Liu Vol. I (2015) §5; Brinon “Représentations p-adiques dans le cas relatif” (2008); Scholze “p-adic Hodge theory for rigid spaces” (2013).

**Depends on**: P7 | **Unlocks**: H3, H8, X3

-----

**H2** ★★☆ — Breuil–Kisin–Fargues modules for semi-stable representations in families

**Current state**: Kisin (2006) classified crystalline $G_K$-representations via Breuil–Kisin modules (finite free modules over $\mathfrak{S} = W(k)[[u]]$ with a Frobenius $\varphi$). Bhatt–Morrow–Scholze (2018) introduced Breuil–Kisin–Fargues modules to handle the integral story uniformly. For semi-stable representations with non-trivial monodromy $N$, the BKF-module picture is understood for individual representations (Brinon–Trihan), but the case of a family $\mathcal{V}$ of semi-stable representations over a base $S$ — where $N$ varies — has no clean formulation.

**The problem**: For a smooth proper family $f: \mathcal{X} \to S$ with semi-stable reduction, construct a relative BKF-module $\mathbb{M}(R^n f_* \mathbb{Z}_p)$ over the relative Breuil–Kisin ring $\mathfrak{S}*S$ equipped with: (i) a Frobenius $\varphi$; (ii) a monodromy operator $N: \mathbb{M} \to \mathbb{M}$ satisfying $N\varphi = p\varphi N$; (iii) a comparison isomorphism with the relative $B*{\text{st}}$-cohomology.

**Entry point — first concrete step**: For the universal semi-stable elliptic curve over the Tate curve parameter $q \in \text{Spa}(\mathbb{Z}_p[[q]])$, write down the BKF-module explicitly and identify how $N$ varies as a function of $q$. The monodromy should vanish when $q \to 0$ (multiplicative reduction degenerates to good reduction).

**Prerequisites**: BMS “Integral p-adic Hodge Theory” (2018) §4–5; Kisin “Crystalline representations” (2006); Brinon–Trihan “Représentations semi-stables” (2008).

**Depends on**: H1 | **Unlocks**: PR3, X1, X6

-----

**H3** ★★☆ — Prismatic comparison for rigid cohomology

**Current state**: Berthelot conjectured that rigid cohomology $H^*_{\text{rig}}(X/K)$ for a variety $X/\mathbb{F}_q$ should be computable via a comparison with de Rham cohomology of a lift. Le Bras–Vezzani (2023) proved a comparison $H^**{\text{rig}}(X/K) \cong H^**{\text{dR}}(\hat{X}/W(k)[1/p])$ for a smooth proper lift $\hat{X}$, using pro-étale methods. The prismatic perspective — which would give integral control via $H^*_\Delta(X/\mathbb{F}_q)$ — is missing.

**The problem**: For $X/\mathbb{F}*p$ smooth proper, construct an isomorphism $H^**{\text{rig}}(X/\mathbb{Q}*p) \cong H^**\Delta(X/\mathbb{Z}_p)[1/p]$ where the right side is the prismatic cohomology of $X$ viewed as an $\mathbb{F}_p$-scheme (using the Frobenius prism $(\mathbb{Z}_p, (p))$). Show this is compatible with Frobenius on both sides and with the Berthelot–Ogus comparison.

**Entry point — first concrete step**: Verify the isomorphism for $X = \mathbb{P}^1_{\mathbb{F}*p}$: compute $H^**\Delta(\mathbb{P}^1_{\mathbb{F}_p}/\mathbb{Z}_p)$ directly using the covering by two affines, and check it gives $\mathbb{Z}_p \oplus \mathbb{Z}_p(-1)$ with the correct Frobenius action.

**Prerequisites**: Bhatt–Scholze “Prisms” (2022) §5–6; Le Bras–Vezzani “de Rham comparison” (2023); Berthelot “Cohomologie rigide I” (1986).

**Depends on**: H1 | **Unlocks**: PR1, X4

-----

**H4** ★☆☆ — Wach modules for symmetric power representations of G_{Q_p}

**Current state**: Berger–Li–Zhu computed the Wach module $\mathbb{N}(V)$ for $V = \text{Sym}^k(V_p(E))$ when $E$ is a good-ordinary elliptic curve, showing $\mathbb{N}(V)$ is free over $\mathbb{Z}_p[[u]][\varphi]$ of rank $k+1$. For supersingular $E$, the Wach module description is more subtle (involves the extended Robba ring); Berger–Breuil gave a partial answer for $k \leq p-2$. The range $k \geq p-1$ is open.

**The problem**: For $E/\mathbb{Q}_p$ supersingular and $k \geq p-1$, explicitly compute the Wach module (or Breuil–Kisin module, or Breuil module) of $\text{Sym}^k(T_p(E))$. State the answer in terms of $\varphi$-matrix with entries in $\mathbb{Z}_p[[u]]$, and verify it matches Colmez’s functor output for the corresponding GL_2-representation.

**Entry point — first concrete step**: For $k = p-1$ and $E$ with $a_p = 0$, use the Fontaine–Laffaille functor to compute $\text{Sym}^{p-1}(T_p(E))$ modulo $p$ as a filtered $\varphi$-module; this gives the leading term of the Wach module.

**Prerequisites**: Berger–Breuil “Sur quelques représentations” (2010); Berger–Li–Zhu (2004); Colmez “Représentations de GL_2(Q_p)” (2010).

**Depends on**: — | **Unlocks**: H5, L1

-----

**H5** ★★☆ — Integral p-adic Hodge theory for wild ramification

**Current state**: Kisin’s theory classifies $G_K$-stable $\mathbb{Z}_p$-lattices in crystalline representations via Breuil–Kisin modules over $\mathfrak{S} = W(k)[[u]]$, $E(u)$ an Eisenstein polynomial. This requires the residue field of $K$ to be perfect. For a wildly ramified extension $L/K$ (where the residue field of $L$ is purely inseparable over that of $K$), the Breuil–Kisin ring $\mathfrak{S}_L$ is not well-defined in the usual sense.

**The problem**: For a totally wildly ramified extension $L/\mathbb{Q}_p$ of degree $p$, define a category of “wild Breuil–Kisin modules” that classifies $G_L$-stable $\mathbb{Z}*p$-lattices in crystalline $G_L$-representations. The expected answer: replace $\mathfrak{S}$ by a ramified Witt ring $W*{\mathcal{O}*K}(\mathcal{O}*{L^\flat})$ as suggested by the prismatic perspective.

**Entry point — first concrete step**: For $L = \mathbb{Q}_p(\pi)$ where $\pi^p = p$, write down the relevant prism $(A, I)$ with $A = W(\mathbb{F}_p[[u^{1/p^\infty}]])$, $I = (E(u))$, and compute the associated Breuil–Kisin ring; verify it has the correct properties modulo $p$.

**Prerequisites**: Kisin “Crystalline representations” (2006); BMS (2018) §4; Caruso “Représentations semi-stables” (2008).

**Depends on**: P7, H1 | **Unlocks**: H6, PR4

-----

**H6** ★★★ — Crystalline comparison for non-proper smooth varieties

**Current state**: The crystalline comparison $H^n_{\text{ét}}(X_{\bar{K}}, \mathbb{Q}*p) \cong D*{\text{cris}}(H^n_{\text{ét}}) \otimes B_{\text{cris}}$ is proved for smooth proper $X/K$ (Faltings, Tsuji, Nizioł). For non-proper $X$, Colmez–Nizioł proved a “local” version using log geometry and syntomic complexes, but the global version — an actual comparison isomorphism compatible with the Poincaré duality pairing — remains unproved in the non-proper case.

**The problem**: For $X/K$ smooth (not necessarily proper), with smooth compactification $\bar{X}$ having normal crossing boundary $D = \bar{X} \setminus X$, prove: $H^n_{\text{ét}, c}(X_{\bar{K}}, \mathbb{Q}*p) \otimes B*{\text{st}} \cong D_{\text{st}}(H^n_{\text{ét},c}(X_{\bar K})) \otimes B_{\text{st}}$ compatibly with $\varphi$, $N$, and Galois action.

**Entry point — first concrete step**: Prove the comparison for $X = \mathbb{A}^1_K$ (affine line). In this case $H^2_c = \mathbb{Q}*p(-1)$ and the comparison reduces to showing $B*{\text{st}}(-1)^{G_K} = K_0$ — which is classical — but the compatibility with the boundary exact sequence $H^*_c(\mathbb{A}^1) \to H^*(\mathbb{P}^1) \to H^*(\infty)$ should be verified in the syntomic language.

**Prerequisites**: Colmez–Nizioł “Syntomic complexes” (2017); Tsuji “p-adic étale cohomology” (1999); Beilinson “p-adic periods and derived de Rham cohomology” (2012).

**Depends on**: H5 | **Unlocks**: R3, X5

-----

**H7** ★☆☆ — Künneth formula for (φ,Γ)-modules over the Robba ring

**Current state**: The Robba ring $\mathcal{R}*K$ is a Bézout domain (every finitely generated ideal is principal), hence $(\varphi, \Gamma)$-modules over it have good homological properties. The tensor product of two $(\varphi, \Gamma)$-modules $M \otimes*{\mathcal{R}} N$ corresponds to the tensor product of the corresponding $G_K$-representations, but the derived Künneth formula — relating $\text{Tor}_i^{\mathcal{R}}(M, N)$ to cohomological operations on representations — has not been written down.

**The problem**: For $(\varphi, \Gamma)$-modules $M, N$ over $\mathcal{R}_K$, prove: $\text{Tor}_i^{\mathcal{R}_K}(M, N) = 0$ for $i \geq 2$, and identify $\text{Tor}_1^{\mathcal{R}*K}(M, N)$ in terms of Galois cohomology of the corresponding representations via Herr’s complex. Derive a Künneth spectral sequence for $H^*(\Gamma, M \otimes*\varphi N)$.

**Entry point — first concrete step**: Compute $\text{Tor}*1^{\mathcal{R}}(\mathcal{R}(\chi*{\text{cyc}}), \mathcal{R}(\chi_{\text{cyc}}^{-1}))$ where $\chi_{\text{cyc}}$ is the cyclotomic character, by explicit resolution using the fact that $\mathcal{R}$ is Bézout.

**Prerequisites**: Berger “Introduction to $(\varphi, \Gamma)$-modules” (2004); Herr “Sur la cohomologie galoisienne” (1998); Kedlaya “Slope filtrations revisited” (2006).

**Depends on**: — | **Unlocks**: H8, R1

-----

**H8** ★★☆ — p-adic Hodge theory for overconvergent F-isocrystals

**Current state**: Kedlaya–Liu showed that an overconvergent $F$-isocrystal on $X/\mathbb{F}_q$ gives rise to a $(\varphi, \nabla)$-module over the Robba ring of $X$. Berger showed that de Rham $(\varphi, \Gamma)$-modules (i.e. those arising from p-adic Galois representations) carry a natural connection. The bridge between these two stories — a functor from overconvergent $F$-isocrystals to $(\varphi, \Gamma)$-modules with connection — is missing in general.

**The problem**: For a smooth curve $C/\mathbb{F}_p$ and a point $x \in C(\mathbb{F}*p)$ with residue disk $D_x \subset C^{\text{rig}}$, construct a functor $\mathcal{F} \mapsto \mathbb{D}(\mathcal{F})$ from overconvergent $F$-isocrystals on $C$ to $(\varphi, \Gamma)$-modules over $\mathcal{R}*{K(x)}$ (where $K(x) = W(\mathbb{F}_p)[1/p]$), and show it is compatible with the local monodromy theorem.

**Entry point — first concrete step**: For $C = \mathbb{A}^1_{\mathbb{F}*p}$ and the rank-1 isocrystal $\mathcal{L}*\psi$ associated to an additive character $\psi$, compute the associated $(\varphi, \Gamma)$-module explicitly at $x = 0$; it should be the Wach module of a character of $G_{\mathbb{Q}_p}$.

**Prerequisites**: Kedlaya–Liu Vol. II (2016) §7; Berger “Equations différentielles p-adiques” (2002); Marmora “Facteurs epsilon p-adiques” (2004).

**Depends on**: H1, H7 | **Unlocks**: X3

-----

### Prismatic Cohomology (PR)

-----

**PR1** ★★★ — Prismatic analogue of the motivic cohomology spectrum

**Current state**: Bhatt–Lurie (2022) constructed the prismatization $X_\Delta$ of a p-adic formal scheme $X$ and showed that $R\Gamma_\Delta(X, \mathcal{O})$ recovers prismatic cohomology. Elmanto–Morrow defined a motivic cohomology spectrum $\mathbb{Z}(n)$ for $\mathbb{F}*p$-schemes using $A^1$-homotopy theory. Bhatt–Lurie have announced a prismatic refinement, but the connection to Voevodsky’s motivic cohomology $H^**{\mathcal{M}}(-, \mathbb{Z}(n))$ in mixed characteristic is not yet a theorem.

**The problem**: Construct a spectrum $\mathbb{Z}*\Delta(n)$ in the $\infty$-category of sheaves on $(\text{Sch}/\mathbb{Z}*p)^{\text{op}}*{\text{proét}}$ such that: (i) $\mathbb{Z}*\Delta(n) \otimes \mathbb{F}*p \simeq \mathbb{Z}(n)*{\mathbb{F}*p}$ (Elmanto–Morrow); (ii) $\mathbb{Z}*\Delta(n)[1/p] \simeq \mathbb{Q}*p(n)$ (Tate twist in $D(X*{\text{proét}})$); (iii) for smooth proper $X/\mathbb{Z}*p$, $H^{2n}*\Delta(X, \mathbb{Z}_\Delta(n)) \cong \text{CH}^n(X)$ (cycle class map).

**Entry point — first concrete step**: Define $\mathbb{Z}_\Delta(1)$ by hand: for a smooth $\mathbb{Z}*p$-algebra $A$, set $\mathbb{Z}*\Delta(1)(A) := \text{fib}(\mathbb{G}*m(A*\Delta) \to \mathbb{G}*m(A/p))$ where $A*\Delta$ is the prismatization; verify this recovers $\widehat{\mathbb{G}}_m$ (the p-adic completion of $\mathbb{G}_m$) and compare with the syntomic $\mathbb{Z}_p(1)$.

**Prerequisites**: Bhatt–Lurie “Absolute Prismatic Cohomology” (2022); Elmanto–Morrow (2021); Antieau–Mathew–Morrow–Nikolaus “Beilinson fiber square” (2022).

**Depends on**: P8, PR9 | **Unlocks**: X2, X5

-----

**PR2** ★★☆ — Prismatic cohomology for algebraic stacks

**Current state**: Bhatt–Scholze define the prismatic site $(X/A)*\Delta$ for a p-adic formal scheme $X$. For a smooth Deligne–Mumford stack $\mathcal{X}$, one can formally imitate the construction, but: (i) the comparison with de Rham cohomology of $\mathcal{X}$ requires the cotangent complex $\mathbb{L}*{\mathcal{X}/\mathbb{Z}_p}$ to be concentrated in degree 0 (smooth), failing for non-representable morphisms; (ii) the Hodge–Tate comparison for stacks with non-trivial stabilizers involves the character theory of the stabilizer groups.

**The problem**: For $\mathcal{X} = [\text{Spec}(A)/G]$ a classifying stack with $G$ a finite flat group scheme over $\mathbb{Z}*p$, compute $H^**\Delta(\mathcal{X}/\mathbb{Z}*p, \mathcal{O}*\Delta)$ and compare with group cohomology $H^*(G, A)$. Formulate the prismatic Künneth formula for the product $\mathcal{X} \times BG$.

**Entry point — first concrete step**: For $\mathcal{X} = B\mu_p = [\text{Spec}(\mathbb{Z}*p)/\mu_p]$, compute $H^**\Delta(B\mu_p, \mathcal{O}_\Delta)$ using the Čech nerve of the cover $\text{Spec}(\mathbb{Z}_p) \to B\mu_p$; compare with $H^*(B\mu_p, \mathbb{Z}_p) = \mathbb{Z}_p[c_1]/(pc_1)$ (Chern class of the tautological line bundle).

**Prerequisites**: Bhatt–Scholze (2022) §4; Lurie “Spectral Algebraic Geometry” Ch. 6 (stacks and cotangent complex); Simpson “Homotopy theory of higher stacks” (1998).

**Depends on**: PR11 | **Unlocks**: PR1, X2

-----

**PR3** ★★☆ — Prismatic F-gauges in the semi-stable case

**Current state**: Bhatt–Scholze (2023) prove: {crystalline $G_K$-representations} $\simeq$ {prismatic $F$-gauges on $\text{Spf}(\mathcal{O}_K)$}. The semi-stable case requires a log structure: Kato’s log prisms $(A, I, M)$ where $M$ is a monoid encoding the boundary. Bhatt–Scholze mention this extension but do not carry it out; the key difficulty is that the Nygaard filtration must be replaced by a “log Nygaard filtration” whose definition is unclear.

**The problem**: Define the category of “log prismatic $F$-gauges” on $\text{Spf}(\mathcal{O}_K)$ with the log structure given by $\mathbb{N} \to \mathcal{O}_K, 1 \mapsto \varpi$ (uniformizer). Prove an equivalence: {semi-stable $G_K$-representations with $N$-filtration} $\simeq$ {log prismatic $F$-gauges}. The monodromy operator $N$ should appear as the “residue of the log connection” on the gauge.

**Entry point — first concrete step**: For the log prism $(\mathbb{A}*{\text{inf}}, \ker\theta, \mathbb{N} \xrightarrow{1 \mapsto [\tilde{p}]} \mathbb{A}*{\text{inf}})$, compute the log-prismatic cohomology of $\text{Spf}(\mathcal{O}*K)$ with the standard log structure, and identify the resulting $(\varphi, N)$-module; it should equal $D*{\text{st}}(\mathbb{Q}_p(1)) = \mathbb{Q}_p \cdot t$ with $\varphi(t) = pt$ and $N(t) = 1$.

**Prerequisites**: Bhatt–Scholze (2023) §5; Kato “Logarithmic structures” (1989); Hyodo–Kato “Semi-stable reduction and crystalline cohomology” (1994).

**Depends on**: H2 | **Unlocks**: PR4, H5, X1

-----

**PR4** ★★☆ — Prismatic Dieudonné theory over very ramified bases

**Current state**: Anschütz–Le Bras (2023) classify p-divisible groups over $\mathcal{O}_K$ (for $K/\mathbb{Q}_p$ finite) in terms of prismatic $F$-crystals over $({\mathcal{O}*K})*\Delta$. Their proof uses the structure of the prismatic site of $\mathcal{O}_K$, which is well-understood only when $e(K/\mathbb{Q}_p) \leq p-1$ (the tamely ramified case). For wildly ramified $K$ (i.e., $e \geq p$), the prismatic site has extra complexity (the Breuil–Kisin prism is not the “final” prism), and the classification is not known.

**The problem**: For $K/\mathbb{Q}_p$ totally wildly ramified with $e(K/\mathbb{Q}_p) = p$ (simplest wild case), classify p-divisible groups over $\mathcal{O}_K$ in terms of “wild prismatic $F$-crystals” — modules over the wild Breuil–Kisin ring defined in H5. Show the resulting category is equivalent to the category of Kisin modules with descent data of Breuil–Kisin–Fargues.

**Entry point — first concrete step**: For $K = \mathbb{Q}*p(\pi)$, $\pi^p = p$, classify p-divisible groups of height 1 (i.e., $\mu*{p^\infty}$ and $\mathbb{Q}_p/\mathbb{Z}_p$ and their deformations) in terms of the wild Breuil–Kisin ring; these are rank-1 objects so the problem reduces to explicit module theory.

**Prerequisites**: Anschütz–Le Bras (2023); Lau “Frames and formal groups” (2010); Kisin “Crystalline representations” (2006).

**Depends on**: PR3, H5 | **Unlocks**: X8, L7

-----

**PR5** ★☆☆ — Prismatic cohomology of toric and nodal singularities

**Current state**: Bhatt–Scholze compute $H^*_\Delta(\mathbb{Z}_p, \mathbb{Z}_p)$ and smooth projective varieties. For the ordinary double point $R = \mathbb{Z}_p[x,y]/(xy - p)$ (special fiber: two lines crossing) and toric singularities $R = \mathbb{Z}_p[S]$ for a toric monoid $S$, no explicit computation has appeared. These are the simplest non-smooth cases.

**The problem**: Compute $H^**\Delta(\text{Spf}(R), \mathcal{O}*\Delta)$ for: (i) $R = \mathbb{Z}_p\langle x,y \rangle/(xy-p)$ (ordinary double point); (ii) $R = \mathbb{Z}_p[u,v,w]/(uv - w^2)$ (A_1 singularity). For (i), identify the Nygaard filtration and the resulting $(\varphi, N)$-module; confirm it matches $H^*_{\text{st}}$ of the associated semistable scheme.

**Entry point — first concrete step**: For $R = \mathbb{Z}*p\langle x,y \rangle/(xy-p)$, find an explicit cover by prisms: use both the Breuil–Kisin prism $(W(k)[[u]], (E(u)))$ mapping to $R$ via $u \mapsto x$ (branch 1) and $u \mapsto y$ (branch 2). Write the Čech complex for this cover and compute $H^0*\Delta$.

**Prerequisites**: Bhatt–Scholze (2022) §7; Bhatt “Cohen–Gabber theorem via prismatic cohomology” (2020); Ogus “Lectures on Logarithmic Algebraic Geometry” (2018).

**Depends on**: — | **Unlocks**: PR3, PR2, X4

-----

**PR6** ★★☆ — Drinfeld’s q-de Rham complex and prismatic cohomology

**Current state**: Scholze (2017) defined a “q-deformation” of the de Rham complex $q\Omega^*_A$ for a smooth $\mathbb{Z}[q]$-algebra $A$, with $q\Omega^**A|*{q=1} = \Omega^**A$. Drinfeld’s prismatization $X*\Delta$ gives a geometric interpretation. Bhatt–Scholze mention that $H^**\Delta(X, \mathcal{O}*\Delta)|*{q=p} = H^**{\text{cris}}(X)$ but the intermediate values of $q$ (between 1 and $p$) are not given a cohomological interpretation.

**The problem**: For $q = \zeta_{p^n}$ (a primitive $p^n$-th root of unity), identify $H^**\Delta(X, \mathcal{O}*\Delta)|*{q = \zeta*{p^n}}$ with a natural cohomology theory for $X \otimes_{\mathbb{Z}*p} \mathbb{Z}*p[\zeta*{p^n}]$ (e.g., relative de Rham cohomology, or a “twisted” crystalline cohomology). Conjecture: it equals the Nygaard-filtered de Rham cohomology of $X*{\mathbb{Z}*p[\zeta*{p^n}]}$ twisted by the $n$-th Adams operation.

**Entry point — first concrete step**: For $X = \mathbb{G}_m = \text{Spec}(\mathbb{Z}*p[t, t^{-1}])$, compute $q\Omega^**{\mathbb{Z}_p[t]}$ explicitly (the q-differential is $d_q(t^n) = [n]_q t^{n-1} dt$); evaluate at $q = \zeta_p$ and identify the cohomology groups.

**Prerequisites**: Scholze “Canonical q-deformations” (2017); Drinfeld “Prismatization” (2020); Bhatt–Lurie “Absolute Prismatic Cohomology” §3.

**Depends on**: PR5 | **Unlocks**: PR7, X4

-----

### Rigid Analytic Geometry (R)

-----

**R1** ★★☆ — Kedlaya–Liu relative (φ,Γ)-modules over Berkovich spaces with boundary

**Current state**: Kedlaya–Liu construct relative $(\varphi, \Gamma)$-modules for smooth proper families over affinoid bases (compact, no boundary). For non-compact bases — e.g., $S = \mathbb{B}^1$ (open disk), or a Stein space with boundary — the “boundary behavior” of the $(\varphi, \Gamma)$-module is not controlled. This is the relative analogue of the “irregular singularity” problem.

**The problem**: For a smooth proper family $f: X \to S$ over $S = \mathbb{B}^1_{\mathbb{Q}*p}$ (open unit disk), equip the relative $(\varphi, \Gamma)$-module $\mathbb{D}(R^n f** \mathbb{Z}_p)$ over the Robba ring $\mathcal{R}_S$ with a “boundary condition” at $|t| = 1$: a filtration by sub-$(\varphi, \Gamma)$-modules controlling the growth rate. Show this filtration is preserved by the Galois action and satisfies a “monodromy-weight” condition.

**Entry point — first concrete step**: For the Legendre family of elliptic curves $y^2 = x(x-1)(x-\lambda)$, $\lambda \in \mathbb{B}^1 \setminus {0, 1}$, compute the Robba ring module $\mathbb{D}(R^1 f_* \mathbb{Z}_p)$ explicitly near $\lambda = 0$ and identify the boundary behavior as $\lambda \to 0$ (the fiber degenerates to a nodal curve, so monodromy should be unipotent).

**Prerequisites**: Kedlaya–Liu Vol. II (2016) §3; Berger “Equations différentielles p-adiques” (2002); Andreatta–Iovita–Kim (2015) for families over disks.

**Depends on**: H7 | **Unlocks**: R2, H8

-----

**R2** ★★☆ — Non-archimedean Riemann–Hilbert correspondence in families

**Current state**: Liu–Zhu (2017) proved a Riemann–Hilbert correspondence for p-adic local systems on a smooth rigid space $X$: $\text{LocSys}_{\mathbb{Z}_p}(X) \simeq \text{MIC}^{\text{HT}}(X)$ (de Rham local systems with Hodge–Tate structure). Shimizu extended this to families. However, both results require $X$ to be smooth. For non-smooth $X$, or for families $f: X \to S$ where $S$ is not smooth, the RH correspondence is unknown.

**The problem**: For $f: X \to S$ a smooth morphism of smooth rigid spaces, and $\mathbb{L}$ a relative $\mathbb{Z}*p$-local system on $X$ (relative over $S$), construct a “relative de Rham local system” $\mathbb{D}*{\text{dR}}(\mathbb{L})$ on $X/S$ equipped with a relative connection $\nabla: \mathbb{D}*{\text{dR}}(\mathbb{L}) \to \mathbb{D}*{\text{dR}}(\mathbb{L}) \otimes \Omega^1_{X/S}$, and prove $\mathbb{L} \mapsto \mathbb{D}_{\text{dR}}(\mathbb{L})$ is fully faithful.

**Entry point — first concrete step**: Verify the relative RH correspondence for the tautological local system on the relative Drinfeld upper half-plane $\Omega^2 \to \text{Spa}(\mathbb{Q}_p)$ — the relative $(\varphi, \Gamma)$-module is known (it is the standard representation of $GL_2$), and the associated de Rham bundle is the Hodge bundle $\omega$ of the universal elliptic curve.

**Prerequisites**: Liu–Zhu (2017); Shimizu “Constancy of generalized Hodge–Tate weights” (2018); Scholze “p-adic Hodge for rigid spaces” §7.

**Depends on**: R1 | **Unlocks**: P9, R5

-----

**R4** ★☆☆ — Mann’s 6-functor formalism for non-locally finite type maps

**Current state**: Mann (2022) constructed a 6-functor formalism for $\mathbb{Z}_\ell$-sheaves on adic spaces of locally finite type (lft) over $\text{Spa}(\mathbb{Q}_p, \mathbb{Z}_p)$. Maps of adic spaces that are not lft (e.g., the structure map $\text{Spa}(\mathbb{Q}_p^\wedge) \to \text{Spa}(\mathbb{Q}_p)$ for a completed algebraic closure) are not covered.

**The problem**: Extend Mann’s formalism to cover all qcqs maps of analytic adic spaces, including non-lft maps and maps between perfectoid spaces. The key step is constructing $f_!$ for a non-lft map by a “limit over compactifications” argument, and proving that the resulting functor satisfies proper base change.

**Entry point — first concrete step**: Define $f_!$ for the map $f: \text{Spa}(C) \to \text{Spa}(\mathbb{Q}*p)$ where $C/\mathbb{Q}*p$ is algebraically closed perfectoid, using the fact that $f$ is the limit of finite morphisms; show $f*! \mathbb{Z}*\ell = C_c(\text{Gal}(\bar{\mathbb{Q}}_p/\mathbb{Q}*p), \mathbb{Z}*\ell)$.

**Prerequisites**: Mann “A p-adic 6-functor formalism” (2022); Clausen–Scholze “Analytic Stacks” §4; Huber “Étale Cohomology” Ch. 2.

**Depends on**: — | **Unlocks**: P2, P9, R9

-----

### p-adic Langlands Program (L)

-----

**L1** ★★★ — Local p-adic Langlands for GL_n(F), F/Q_p finite

**Current state**: For $G = GL_2(\mathbb{Q}_p)$: Colmez (2010) constructed a functor $V \mapsto \Pi(V)$ from 2-dimensional $(\varphi, \Gamma)$-modules to $GL_2(\mathbb{Q}_p)$-Banach representations; Paškūnas (2013) proved it is an equivalence on blocks. For $GL_2(F)$, $F \neq \mathbb{Q}_p$: Breuil–Mézard have partial results. For $GL_n$, $n \geq 3$: only the “generic” case is understood (Breuil–Hellmann–Schraen 2019 for trianguline representations). A full correspondence is not known for any $n \geq 3$.

**The problem**: For $n = 3$, $F = \mathbb{Q}*p$, construct a functor $\Pi: {3\text{-dim’l } (\varphi,\Gamma)\text{-modules over }\mathcal{R}*{\mathbb{Q}_p}} \to {GL_3(\mathbb{Q}*p)\text{-Banach representations}}$ satisfying: (i) $\Pi(V)$ is non-zero iff $V$ is “p-adic Hodge theoretically reasonable”; (ii) $\Pi(V)$ is admissible; (iii) $\Pi(V)|*{B(\mathbb{Q}_p)} \cong (\text{Jacquet module of } V)$ compatibly with filtration. State the expected answer in terms of the Orlik–Strauch construction.

**Entry point — first concrete step**: For $V$ crystalline of Hodge–Tate weights $(0, 1, 2)$ and distinct Frobenius eigenvalues, the expected $\Pi(V)$ is the locally algebraic representation $\text{Sym}^1 \otimes \text{Sym}^1 \boxtimes \chi$ twisted by a locally algebraic character. Construct this representation explicitly and verify it has the correct $(\varphi,\Gamma)$-module.

**Prerequisites**: Colmez “Représentations de $GL_2(\mathbb{Q}_p)$” (2010); Paškūnas (2013); Breuil–Hellmann–Schraen “Smoothness and classicality” (2019).

**Depends on**: H4 | **Unlocks**: L2, L7, L9

-----

**L5** ★☆☆ — Coherent sheaves on the GL_2 L-parameter stack

**Current state**: Fargues–Scholze (2021) construct the stack $Z^1(W_{\mathbb{Q}*p}, GL_2)/GL_2$ of L-parameters and conjecture $\text{Coh}(Z^1(W*{\mathbb{Q}*p}, GL_2)/GL_2) \simeq \text{Rep}*{\text{sm}}(GL_2(\mathbb{Q}*p))$. Paškūnas classified $\text{Rep}*{\text{sm}}(GL_2(\mathbb{Q}*p))$ into blocks. On the stack side, the connected components of $Z^1(W*{\mathbb{Q}_p}, GL_2)/GL_2$ are indexed by Weil–Deligne representations, but the coherent sheaves on each component have not been explicitly identified.

**The problem**: For the irreducible principal series block (corresponding to an unramified Weil–Deligne representation $\text{rec}(\pi_0)$ with $\pi_0 = \text{Ind}*{B}^{GL_2}(\chi_1 \otimes \chi_2)$ unramified), describe $\text{Coh}(Z^1*{\text{rec}(\pi_0)}/GL_2)$ explicitly as a $\mathbb{G}_m$-equivariant coherent sheaf on $\mathbb{A}^1$ (the Hecke eigenvalue). Match with Paškūnas’s block description: the block is equivalent to $\text{mod-}\mathcal{H}$ where $\mathcal{H}$ is the Hecke algebra.

**Entry point — first concrete step**: The unramified component of $Z^1(W_{\mathbb{Q}*p}, GL_2)/GL_2$ is isomorphic to $[\mathbb{A}^2*{\text{symm}}/GL_2] = \text{Spec}(\mathbb{Z}_p[s, t])$ where $s = \text{tr}$ and $t = \det$. Compute $H^0$ and $H^1$ of the tautological rank-2 sheaf on this stack and identify them with the Hecke algebra $\mathcal{H}(GL_2(\mathbb{Q}_p), GL_2(\mathbb{Z}_p))$.

**Prerequisites**: Fargues–Scholze “Geometrization” Ch. I–II; Paškūnas (2013); Emerton–Gee–Hellmann (2022) §5.

**Depends on**: P5 | **Unlocks**: L6, L11

-----

**L7** ★★☆ — Breuil–Mézard conjecture for GL_n, n ≥ 3

**Current state**: The Breuil–Mézard conjecture (2002) for $GL_2(\mathbb{Q}*p)$ predicts that the Hilbert–Samuel multiplicity of a local Galois deformation ring $R*{\bar{V}, \tau}$ (deforming $\bar{V}$ with “Hodge type” $\tau$) equals a sum of multiplicities of Serre weights, weighted by modular representation theory of $GL_2(\mathbb{F}_p)$. This was proved by Kisin (2009) and extended by Emerton–Gee (2023) to $GL_n$ for some cases, but the full $GL_n$ conjecture remains open for $n \geq 3$.

**The problem**: For $\bar{V}: G_{\mathbb{Q}*p} \to GL_3(\mathbb{F}*p)$ generic (in the sense of Herzig), prove: $e(R*{\bar{V}, \tau}) = \sum*{\sigma \in W(\tau)} m(\bar{V}, \sigma)$ where $W(\tau)$ is the set of Serre weights for the inertial type $\tau$, and $m(\bar{V}, \sigma)$ are the multiplicities predicted by the weight part of Serre’s conjecture for $GL_3$.

**Entry point — first concrete step**: Verify the formula for $\bar{V}$ the direct sum of three distinct characters $\chi_1 \oplus \chi_2 \oplus \chi_3$ (reducible, split case). In this case $R_{\bar{V}, \tau}$ is a complete intersection (Kisin’s $R = T$ theorem applies), and the multiplicity formula should reduce to a combinatorial identity in the Weyl group of $GL_3$.

**Prerequisites**: Emerton–Gee “A geometric perspective on the Breuil–Mézard conjecture” (2023); Herzig “The weight in a Serre-type conjecture for tame n-dimensional Galois representations” (2009); PR4 (prismatic methods for deformation rings).

**Depends on**: PR4, L1 | **Unlocks**: L10

-----

**L10** ★★★ — Local–global compatibility for categorical p-adic Langlands

**Current state**: Emerton proved local–global compatibility for the classical (non-categorical) p-adic Langlands: the local $GL_2(\mathbb{Q}*p)$-representation appearing in completed cohomology at a prime $p$ is determined by the local Galois representation. The categorical version — relating the spectral action of $\text{Perf}(Z^1(W*{\mathbb{Q}_p}, \hat{G})/\hat{G})$ on local representations to the global Hecke algebra action on completed cohomology — has not been formulated precisely, let alone proved.

**The problem**: For a definite quaternion algebra $D/\mathbb{Q}$ split at $p$, formulate a precise “categorical local–global compatibility”: an equivalence of categories $\tilde{H}^0(\mathcal{X}_D, \mathbb{Z}*p) \simeq \text{IndCoh}(Z^1(W*{\mathbb{Q}*p}, GL_2)/GL_2)^{T*{\text{global}}}$ where the right side is the global Hecke eigenspace and the equivalence is $\text{Perf}(Z^1/GL_2)$-linear.

**Entry point — first concrete step**: For a single Hecke eigensystem $\lambda: \mathbb{T} \to \mathcal{O}*E$ (classical eigenform of weight $k$, level $N$ prime to $p$), verify that the corresponding coherent sheaf $\mathcal{F}*\lambda$ on $Z^1(W_{\mathbb{Q}*p}, GL_2)/GL_2$ (supported on the L-parameter $\text{rec}(f_p)$) has $\text{Hom}(\mathcal{F}*\lambda, -) \cong \Pi_\lambda(-)$ where $\Pi_\lambda$ is Colmez’s representation.

**Prerequisites**: Emerton “Local–global compatibility in the p-adic Langlands program” (2011); Fargues–Scholze Ch. X; Hellmann (2023).

**Depends on**: L7, P4 | **Unlocks**: X5, X6

-----

### Cross-area Problems (X)

-----

**X1** ★★☆ — Prismatic shtukas and Langlands parameters

**Current state**: Bhatt–Scholze identify crystalline $G_K$-representations with “prismatic shtukas” (BKF-modules with Frobenius). Fargues–Scholze use “shtukas” on the FF-curve to parametrize L-parameters. The two notions of “shtuka” are not directly compared; the bridge would require identifying a “prismatic Langlands parameter” as a shtuka on the prismatization of the FF-curve.

**The problem**: Construct a functor from prismatic $F$-gauges on $\text{Spf}(\mathcal{O}*K)$ to “Weil-parameter shtukas” on $X*{FF}$, extending the known functor ${\text{crystalline reps}} \to {\text{BdR shtukas}}$ (Fargues–Scholze Ch. II). Identify the essential image as “shtukas with crystalline modification.”

**Entry point — first concrete step**: For a crystalline representation $V$ of $G_K$ with HT weights in $[0, 1]$ (i.e., a p-divisible group), trace through both constructions: (1) Anschütz–Le Bras give a prismatic $F$-crystal; (2) Fargues–Scholze give a shtuka on $X_{FF}$ with one leg. Verify the two constructions are compatible via the Berthelot–Ogus comparison.

**Prerequisites**: Bhatt–Scholze (2023); Fargues–Scholze “Geometrization” Ch. II; Anschütz–Le Bras (2023).

**Depends on**: PR3, P8 | **Unlocks**: L7, X8

-----

**X4** ★☆☆ — Explicit comparison: prismatic vs. rigid cohomology

**Current state**: For $X/\mathbb{F}*p$ smooth proper, both $H^**\Delta(X, \mathcal{O}*\Delta)$ (prismatic) and $H^**{\text{rig}}(X/\mathbb{Q}_p)$ (rigid) are defined and known to be isomorphic after inverting $p$ (by H3, partially). But for explicit varieties (projective spaces, elliptic curves, Fermat hypersurfaces), the prismatic calculation has not been done from scratch, and the comparison isomorphism has not been written out at the cochain level.

**The problem**: For $X = E_a: y^2 = x^3 - x + a$ (Weierstrass elliptic curve over $\mathbb{F}*p$), compute $H^1*\Delta(E_a/\mathbb{Z}*p, \mathcal{O}*\Delta)$ directly via the Čech complex on the prismatic site, and verify it equals $H^1_{\text{rig}}(E_a/\mathbb{Q}_p) = \mathbb{Q}_p^2$ with the correct Frobenius eigenvalues ($\alpha, p/\alpha$ where $\alpha$ is a root of $T^2 - a_p T + p$).

**Entry point — first concrete step**: Cover $E_a$ by the two standard affine patches $U_1 = {y \neq \infty}$ and $U_2 = {x \neq \infty}$; find explicit prisms for each patch (use the Witt vector prism for $U_i$ after choosing a lift); compute the Čech 1-cocycle.

**Prerequisites**: Bhatt–Scholze (2022) §7–8; Kedlaya “Finiteness of rigid cohomology” (2006); Monsky–Washnitzer (1968) for comparison.

**Depends on**: PR5, H3 | **Unlocks**: PR1, X5

-----

**X8** ★★☆ — Prismatic Dieudonné theory and the Barsotti–Tate stack

**Current state**: Anschütz–Le Bras (2023) classify p-divisible groups over $\mathcal{O}_K$ via prismatic $F$-crystals. The Emerton–Gee stack $\mathcal{X}_2$ parametrizes 2-dimensional $(\varphi, \Gamma)$-modules; its Barsotti–Tate locus $\mathcal{X}^{BT}_2$ is a closed substack. The relation between prismatic Dieudonné modules (which classify the p-divisible group) and the Barsotti–Tate locus in $\mathcal{X}^{BT}_2$ (which classifies the Galois representation) has not been made into a precise functor.

**The problem**: Construct an isomorphism of stacks $\mathcal{M}^{\text{pris}}_{BT, 2} \xrightarrow{\sim} \mathcal{X}^{BT}_2$ where the left side is the moduli stack of “height-2 prismatic $F$-crystals of type BT” (defined via Anschütz–Le Bras) and $\mathcal{X}^{BT}_2$ is the Emerton–Gee Barsotti–Tate stack. Show the isomorphism is compatible with the Breuil–Kisin period map.

**Entry point — first concrete step**: For $p$-divisible groups of height 2 and dimension 1 over $\mathcal{O}_{\bar{\mathbb{Q}}_p}$ (i.e., formal $\mathcal{O}_F$-modules), write the Anschütz–Le Bras classification explicitly; identify each isomorphism class with a point of $\mathcal{X}^{BT}*2(\mathcal{O}*{\bar{\mathbb{Q}}_p})$ via the Colmez–Fontaine theorem.

**Prerequisites**: Anschütz–Le Bras (2023); Emerton–Gee “Moduli stacks of $(\varphi,\hat{G})$-modules” (2023); Kisin “Potentially semi-stable deformation rings” (2008).

**Depends on**: PR4, X1 | **Unlocks**: L7, L10

-----

### p-adic Simpson Correspondence (S)

-----

**S1** ★☆☆ — Essential image of the Simpson correspondence in rank > 1

**Current state**: Heuer (2022, Compos. Math.) fully described the essential image for rank 1: a pro-étale line bundle corresponds to a continuous character $\pi_1^{\text{ét}}(X) \to K^\times$ if and only if the underlying line bundle is topologically torsion in $\text{Pic}(X)$, not merely having vanishing Chern class (contrary to the classical complex analogy). For rank $n \geq 2$, no analogous characterization of the essential image is known; Faltings (2005) and AGT (2016) only handle “small” representations (close to trivial).

**The problem**: For a smooth proper curve $X/\mathbb{C}_p$ and $n = 2$, characterize the essential image of the p-adic Simpson functor ${\text{continuous } \pi_1^{\text{ét}}(X) \to GL_2(\mathbb{C}*p)} \to {\text{Higgs bundles on } X}$. Conjecture (Heuer): the image consists of Higgs bundles $(E, \theta)$ where $E$ is “v-topologically torsion” in an appropriate sense in the moduli stack $\text{Bun}*{GL_2}(X_v)$, generalizing the rank-1 condition.

**Entry point — first concrete step**: For $X$ an elliptic curve over $\mathbb{C}_p$, classify rank-2 Higgs bundles $(E, \theta)$ with $\theta = 0$ (flat bundles) that arise from crystalline representations of $\pi_1(X)$; these should correspond to rank-2 vector bundles on the formal group of $X$. Verify that “topologically torsion” in this case means $E$ is a successive extension of topologically torsion line bundles.

**Prerequisites**: Heuer “A geometric p-adic Simpson correspondence in rank one” (Compos. Math. 2024); AGT book Ch. II; Heuer–Xu arXiv:2402.01365.

**Depends on**: — | **Unlocks**: S2, S4

-----

**S2** ★★☆ — p-adic Simpson correspondence for non-proper rigid spaces

**Current state**: Heuer (arXiv:2307.01303, 2023) proved the p-adic Simpson correspondence — an equivalence $\text{Vect}(X_{\text{proét}}) \simeq \text{Higgs}(X)$ — for smooth **proper** rigid spaces over a complete algebraically closed extension of $\mathbb{Q}_p$. The properness is used crucially to ensure convergence of the Higgs field (which is a global section of $\mathcal{E}nd(E) \otimes \Omega^1_X$). For non-proper $X$ (e.g., open rigid disks, Drinfeld’s upper half-plane), the correspondence is not known and Higgs fields may have poles.

**The problem**: For $X = \Omega^2$ (Drinfeld’s upper half-plane over $\mathbb{Q}_p$), formulate and prove a p-adic Simpson correspondence with “growth conditions” at the boundary: an equivalence between pro-étale vector bundles with controlled growth and Higgs bundles with at most logarithmic poles along the boundary divisor of a compactification $\bar{X}$.

**Entry point — first concrete step**: Study rank-1 objects: classify pro-étale $\mathcal{O}^+$-line bundles on $\Omega^2$ by computing $H^1(\Omega^2_{\text{proét}}, \mathcal{O}^+)$. Compare with logarithmic Higgs line bundles (i.e., $\Omega^1_{\Omega^2}(\log \partial)$-valued forms) to formulate the correct boundary condition.

**Prerequisites**: Heuer arXiv:2307.01303; Heuer “Moduli spaces in p-adic non-abelian Hodge theory” arXiv:2207.13819; Liu–Zhu “Rigidity and a Riemann–Hilbert correspondence” (2017).

**Depends on**: S1, R2 | **Unlocks**: S5, R3

-----

**S3** ★★☆ — Derived p-adic Simpson functor and its essential image

**Current state**: Anschütz–Heuer–Le Bras (Crelle 2025, arXiv:2302.12747) constructed a derived p-adic Simpson functor: a fully faithful embedding $\text{Perf}(X_{\text{HT}})^{\text{isog}} \hookrightarrow \text{Perf}(X_{v})$ where $X_{\text{HT}}$ is the Hodge–Tate stack of $X$. The functor is only fully faithful (not essentially surjective), and the essential image — which v-perfect complexes arise from the Hodge–Tate stack — is not characterized.

**The problem**: Characterize the essential image of $\text{Perf}(X_{\text{HT}})^{\text{isog}} \hookrightarrow \text{Perf}(X_v)$. Conjecture: it consists of those v-perfect complexes $\mathcal{F}$ whose Sen operator $\Theta_{\mathcal{F}}: \mathcal{F} \to \mathcal{F} \otimes \mathcal{O}_X$ is nilpotent (in a derived sense). Prove this for $X$ a smooth proper curve.

**Entry point — first concrete step**: For $X$ a smooth proper curve, verify that a v-line bundle $\mathcal{L}$ lies in the essential image if and only if its Sen operator $\Theta_\mathcal{L} \in H^0(X, \mathcal{O}*X)$ is zero — this recovers Heuer’s rank-1 result. The key computation is to show $\Theta*\mathcal{L} = 0 \Leftrightarrow \mathcal{L}$ is in the image of $\text{Pic}(X_{\text{HT}}) \to \text{Pic}(X_v)$.

**Prerequisites**: Anschütz–Heuer–Le Bras arXiv:2302.12747 (Crelle 2025); Anschütz–Heuer–Le Bras arXiv:2211.08470 (Sen theory via Hodge–Tate stack); Heuer “Moduli spaces” arXiv:2207.13819.

**Depends on**: S1 | **Unlocks**: S4, X9

-----

**S4** ★★☆ — p-adic Simpson for G-bundles: non-abelian case beyond curves

**Current state**: Heuer–Xu (arXiv:2402.01365, 2024) proved that for a smooth projective **curve** $X/\mathbb{C}_p$ and any reductive group $G$, the moduli stack of $G$-Higgs bundles is a canonical twist of the moduli stack of v-topological $G$-bundles, giving a geometrization of Faltings’ correspondence. Heuer–Werner–Zhang (Canad. J. Math. 2025) handle commutative $G$ in any dimension. For non-abelian $G$ in dimension $\geq 2$, no result is known.

**The problem**: For $X$ a smooth proper rigid space of dimension $\geq 2$ over $\mathbb{C}_p$ and $G = GL_n$ ($n \geq 2$), construct a natural isomorphism of stacks $\text{Higgs}_G(X) \xrightarrow{\sim} \mathcal{T}wist(\text{Bun}_G(X_v))$ where the twist is by the torsor of Hodge–Tate splittings. Prove this recovers Heuer’s Theorem 1.1 (arXiv:2307.01303) on objects.

**Entry point — first concrete step**: For $X$ smooth proper of dimension 2 and $G = GL_2$, verify the isomorphism on $\mathbb{C}_p$-points: show that a $GL_2$-Higgs bundle $(E, \theta)$ with $\theta \in H^0(X, \mathcal{E}nd(E) \otimes \Omega^1_X)$ corresponds canonically (after a choice of exponential) to a pro-étale $GL_2$-torsor on $X$. Use the Koszul resolution to reduce to the rank-1 case.

**Prerequisites**: Heuer–Xu arXiv:2402.01365; Heuer arXiv:2307.01303; AGT book Foreword and Ch. I.

**Depends on**: S1, S3 | **Unlocks**: X9

-----

**S5** ★★☆ — Relative Hodge–Tate spectral sequence for non-proper morphisms

**Current state**: Heuer (arXiv:2402.00842, 2024) constructed a relative Hodge–Tate spectral sequence $E_2^{i,j} = H^i(X, \Omega^j_{X/S}(-j)) \Rightarrow H^{i+j}(X_{\text{proét}}, \hat{\mathcal{O}}_X)$ for any smooth **proper** morphism $f: X \to S$ of rigid spaces over a perfectoid field. For non-proper $f$, the spectral sequence is expected to degenerate only with a compactification and a growth condition on cohomology.

**The problem**: For $f: X \to S$ smooth (not necessarily proper), with $X$ having a good compactification $\bar{X}$ with normal crossing boundary $D$, construct a “logarithmic relative Hodge–Tate spectral sequence” $E_2^{i,j} = H^i(X, \Omega^j_{X/S}(\log D)(-j)) \Rightarrow H^{i+j}*c(X*{\text{proét}}, \hat{\mathcal{O}}_X)$ and prove $E_2$-degeneration for smooth proper $\bar{X}$ with $D$ a normal crossing divisor.

**Entry point — first concrete step**: For $f: \mathbb{G}_{m,S} \to S$ (punctured line), compute both sides of the expected spectral sequence: $H^i(\mathbb{G}*m, \Omega^j*{\mathbb{G}_m/S}(\log {0,\infty}))$ and $H^{i+j}_c((\mathbb{G}*m)*{\text{proét}}, \hat{\mathcal{O}})$, and verify the $E_2$-degeneration in this case by explicit calculation.

**Prerequisites**: Heuer arXiv:2402.00842; Scholze “p-adic Hodge theory for rigid spaces” (2013) §3; Brinon–Conrad “CMI notes” §4 (Hodge–Tate decomposition).

**Depends on**: S2, R1 | **Unlocks**: X9

-----

**S6** ★★★ — Integral p-adic Simpson correspondence via prismatic cohomology

**Current state**: Min–Wang (arXiv:2201.08030) proved a p-adic Simpson correspondence via prismatic methods: for a smooth p-adic formal scheme $\mathfrak{X}/\mathcal{O}*K$, there is an equivalence between rational Hodge–Tate crystals on $(\mathfrak{X})*\mathbb{A}$ (absolute prismatic site) and enhanced Higgs bundles on the generic fiber $X$. This is a “rational” result (inverts $p$). An integral version — working with $\mathbb{Z}_p$-coefficients throughout — is not known.

**The problem**: For $\mathfrak{X}/\mathcal{O}_K$ smooth proper, construct an integral p-adic Simpson equivalence between $\mathbb{Z}*p$-local systems on $X*{\text{proét}}$ with “integral Hodge–Tate structure” and a suitable integral notion of Higgs bundle (e.g., “Higgs $\mathcal{O}_X^+$-modules” bounded by some Harder–Narasimhan slope condition). Identify the correct integrality condition on the Higgs side.

**Entry point — first concrete step**: For rank-1 objects, verify for $X$ an elliptic curve with good reduction over $\mathbb{Q}_p$: the $\mathbb{Z}_p$-local systems are $T_p(E)$ and its twists, and the corresponding Higgs bundle should be the Hodge bundle $\omega_E$ with $\theta = 0$.

**Prerequisites**: Min–Wang arXiv:2201.08030; AGT book Ch. II–III; Bhatt–Scholze “Prismatic F-crystals” (2023).

**Depends on**: S3, PR9 | **Unlocks**: PR1, X9

-----

### Cross-area Problems (X)

-----

**X1** ★★☆ — Prismatic shtukas and Langlands parameters

**Current state**: Bhatt–Scholze identify crystalline $G_K$-representations with “prismatic shtukas” (BKF-modules with Frobenius). Fargues–Scholze use “shtukas” on the FF-curve to parametrize L-parameters. The two notions of “shtuka” are not directly compared; the bridge would require identifying a “prismatic Langlands parameter” as a shtuka on the prismatization of the FF-curve.

**The problem**: Construct a functor from prismatic $F$-gauges on $\text{Spf}(\mathcal{O}*K)$ to “Weil-parameter shtukas” on $X*{FF}$, extending the known functor ${\text{crystalline reps}} \to {\text{BdR shtukas}}$ (Fargues–Scholze Ch. II). Identify the essential image as “shtukas with crystalline modification.”

**Entry point — first concrete step**: For a crystalline representation $V$ of $G_K$ with HT weights in $[0, 1]$ (i.e., a p-divisible group), trace through both constructions: (1) Anschütz–Le Bras give a prismatic $F$-crystal; (2) Fargues–Scholze give a shtuka on $X_{FF}$ with one leg. Verify the two constructions are compatible via the Berthelot–Ogus comparison.

**Prerequisites**: Bhatt–Scholze (2023); Fargues–Scholze “Geometrization” Ch. II; Anschütz–Le Bras (2023).

**Depends on**: PR3, P8 | **Unlocks**: L7, X8

-----

**X4** ★☆☆ — Explicit comparison: prismatic vs. rigid cohomology

**Current state**: For $X/\mathbb{F}*p$ smooth proper, both $H^**\Delta(X, \mathcal{O}*\Delta)$ (prismatic) and $H^**{\text{rig}}(X/\mathbb{Q}_p)$ (rigid) are defined and known to be isomorphic after inverting $p$ (by H3, partially). But for explicit varieties (projective spaces, elliptic curves, Fermat hypersurfaces), the prismatic calculation has not been done from scratch, and the comparison isomorphism has not been written out at the cochain level.

**The problem**: For $X = E_a: y^2 = x^3 - x + a$ (Weierstrass elliptic curve over $\mathbb{F}*p$), compute $H^1*\Delta(E_a/\mathbb{Z}*p, \mathcal{O}*\Delta)$ directly via the Čech complex on the prismatic site, and verify it equals $H^1_{\text{rig}}(E_a/\mathbb{Q}_p) = \mathbb{Q}_p^2$ with the correct Frobenius eigenvalues ($\alpha, p/\alpha$ where $\alpha$ is a root of $T^2 - a_p T + p$).

**Entry point — first concrete step**: Cover $E_a$ by the two standard affine patches $U_1 = {y \neq \infty}$ and $U_2 = {x \neq \infty}$; find explicit prisms for each patch (use the Witt vector prism for $U_i$ after choosing a lift); compute the Čech 1-cocycle.

**Prerequisites**: Bhatt–Scholze (2022) §7–8; Kedlaya “Finiteness of rigid cohomology” (2006); Monsky–Washnitzer (1968) for comparison.

**Depends on**: PR5, H3 | **Unlocks**: PR1, X5

-----

**X8** ★★☆ — Prismatic Dieudonné theory and the Barsotti–Tate stack

**Current state**: Anschütz–Le Bras (2023) classify p-divisible groups over $\mathcal{O}_K$ via prismatic $F$-crystals. The Emerton–Gee stack $\mathcal{X}_2$ parametrizes 2-dimensional $(\varphi, \Gamma)$-modules; its Barsotti–Tate locus $\mathcal{X}^{BT}_2$ is a closed substack. The relation between prismatic Dieudonné modules (which classify the p-divisible group) and the Barsotti–Tate locus in $\mathcal{X}^{BT}_2$ (which classifies the Galois representation) has not been made into a precise functor.

**The problem**: Construct an isomorphism of stacks $\mathcal{M}^{\text{pris}}_{BT, 2} \xrightarrow{\sim} \mathcal{X}^{BT}_2$ where the left side is the moduli stack of “height-2 prismatic $F$-crystals of type BT” (defined via Anschütz–Le Bras) and $\mathcal{X}^{BT}_2$ is the Emerton–Gee Barsotti–Tate stack. Show the isomorphism is compatible with the Breuil–Kisin period map.

**Entry point — first concrete step**: For $p$-divisible groups of height 2 and dimension 1 over $\mathcal{O}_{\bar{\mathbb{Q}}_p}$ (i.e., formal $\mathcal{O}_F$-modules), write the Anschütz–Le Bras classification explicitly; identify each isomorphism class with a point of $\mathcal{X}^{BT}*2(\mathcal{O}*{\bar{\mathbb{Q}}_p})$ via the Colmez–Fontaine theorem.

**Prerequisites**: Anschütz–Le Bras (2023); Emerton–Gee “Moduli stacks of $(\varphi,\hat{G})$-modules” (2023); Kisin “Potentially semi-stable deformation rings” (2008).

**Depends on**: PR4, X1 | **Unlocks**: L7, L10

-----

**X9** ★★☆ — [Simpson × Langlands] Higgs bundles and the spectral action

**Current state**: In the Fargues–Scholze framework, the spectral action of $\text{Perf}(Z^1(W_F, \hat{G})/\hat{G})$ on $D(\text{Bun}_G)$ encodes the categorical Langlands correspondence. On the other hand, Heuer–Xu show that $G$-Higgs bundles on a curve $X$ are related to v-topological $G$-bundles on $X_v$. The connection between “Higgs bundles as Langlands parameters” (à la Geometric Langlands over $\mathbb{C}$) and “Higgs bundles as Simpson data” in the p-adic setting has not been made precise.

**The problem**: For a smooth projective curve $X/\mathbb{F}_p$ with a lift $\mathfrak{X}/\mathbb{Z}*p$, formulate a precise relation between: (i) the stack of $G$-Higgs bundles on $X*{\mathbb{C}*p}$ (p-adic Simpson side) and (ii) the stack of L-parameters $Z^1(W*{\mathbb{Q}_p}, \hat{G})/\hat{G}$ (Langlands side). Conjecture: there is a “p-adic Hitchin fibration” whose generic fiber recovers the Fargues–Scholze L-parameter stack.

**Entry point — first concrete step**: For $G = GL_1$ and $X$ an elliptic curve, the Higgs moduli is $\text{Pic}^0(X) \times H^0(X, \Omega^1)$; the L-parameter stack is $[\text{Hom}(W_{\mathbb{Q}_p}, \mathbb{G}_m)/\mathbb{G}_m]$. Construct an explicit map between them via the Hodge–Tate period map and verify it factors through the Hodge–Tate filtration.

**Prerequisites**: Heuer–Xu arXiv:2402.01365; Fargues–Scholze “Geometrization” Ch. I–II; Ben-Zvi–Nadler “Loop spaces and Langlands parameters” (for the complex analogy).

**Depends on**: S4, L5 | **Unlocks**: L10

-----

## Dependency Graph Summary

```
P7 ──→ H1 ──→ H3 ──→ PR1
        │            ↑
        └──→ H5 ──→ PR4 ──→ X8 ──→ L7 ──→ L10
                    │              ↑          ↑
P8 ──→ PR9 ──→ PR1  └──→ X1 ───────┘          │
       ↑                                       │
PR3 ───┘                                  X9 ──┘
  ↑                                       ↑
H2                               S4 ──→ X9
                                  ↑      ↑
PR5 ──→ PR3                  S1 ──┘  S5 ─┘
PR5 ──→ X4 ──→ PR1            │
                               └──→ S2 ──→ S5
P2 ──→ P4 ──→ L10              │
P5 ──→ L5 ──→ L6 / X9         └──→ S3 ──→ S4
                                          │
H7 ──→ H8 ──→ X3             S3, PR9 ──→ S6 ──→ PR1
H7 ──→ R1 ──→ R2 ──→ P9
       │
       └──→ S5
```

-----

## Interaction Patterns

When the user asks for ideas, always:

- **Zoom in**: Expand any bank entry to full Output Format
- **Reading plan**: 6-month plan toward a problem (draw from `references/key_papers.md`)
- **Feasibility compare**: Weigh two problems on difficulty/background/timeliness
- **Program design**: Use the dependency graph to propose a 3-year program (e.g. S1 → S3 → S4 → X9, or PR3 → PR4 → X8 → L7)
- **Hot topics**: Flag entries marked ★★★ or those with many dependents as highest current activity; remind user to verify on arXiv (`references/arxiv_guide.md`)

-----

## Notes for Claude

- Be mathematically precise: distinguish B_dR from B_cris, adic spaces from Berkovich spaces, prismatic F-gauges from F-crystals, log prisms from ordinary prisms, v-bundles from pro-étale bundles, Hodge–Tate stack from Cartier–Witt stack.
- State the current state honestly: if a problem may have been recently solved or partially solved, say so and direct to arXiv.
- When a user mentions a specific paper, map it to the relevant problems and identify which “Current state” it advances.
- The dependency graph is a guide, not a constraint: encourage the user to find unexpected shortcuts.