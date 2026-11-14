# Paper Revisions Checklist

## General & Conceptual Clarifications

* [x] **Novelty & Prior Work:** Clarify which of the alpha-equivalence definitions and equivalence proofs are novel contributions of this paper versus those already established in the literature or formalized in other proof assistants.
* [ ] **Introduction Contributions:** Explain clearly in the Introduction in what sense the alternative definitions constitute a contribution of the present work.
* [ ] **Nominal Sets & Transpositions:** Add a remark noting that theorems about `a/p`-equivalence invariances follow from invariance under name permutations (via nominal sets), and clarify that restricting to transpositions is sufficient for the current development.
* [ ] **Future Work Expansion:** Mention in the future work/conclusion the potential for generalizing this comparison to syntax with a general name binder (e.g., `<a>t`), terms with metavariables, and the impact of Definition 4 on unification and matching problems.

## Page-by-Page Edits

### Page 1 (Abstract)

* [x] Replace "several definitions" with "four different definitions" (or similar phrasing) in the abstract.

### Page 2

* [x] **Citations:** Add more supporting references (such as a relevant survey) to back up the claim regarding the wide adoption of the nominal approach.
* [x] **Grammar:** Change "continue following the above framework of untyped" to "continue to follow...".

### Page 3

* [x] **Spacing/Formatting (Line 4 from bottom):** Fix the extra empty space between "of the metatheory." and "The third".

### Page 4

* [x] **Terminology Clarification:** Clarify what "lower positions" means regarding variables `a` and `b`, addressing the potential confusion between higher positions in the syntax tree and list indexing/positions (considering a list with the head on the right).
* [x] **Definition 4 (`ThereVA`):** Clarify or justify the choice of using `a` and `b` to denote variables in rule `(ThereVA)`.
* [ ] **Definition 4 (`HereVA`):** Explain why `xs` and `ys` are not restricted to lists of the same length in rule `(HereVA)`.

### Page 5

* [x] **`Lemma alpha_rename_gen` Proof (Derivation Tree):** Explain why `z` in `l :: z` is not also replaced by `w` when reading `(\forall_i)` bottom-up in the derivation tree.
* [x] **`Lemma alpha_rename_gen` Proof (Hypothesis):** Define or clarify what `t` refers to in the hypothesis `z \in fv(t)` at the end of the proof.
* [x] **`Lemma alpha_rename`:** Clarify where the `y \neq z` hypothesis comes from.
* [ ] **Shadowing Explanation:** Define "shadowed" explicitly when stating that variables can be removed from the context if shadowed by earlier ones with the same value. Also verify/clarify whether a variable is shadowed by *earlier* or *later* ones when comparing the path in the syntax tree versus the list of bound variables along that path.

### Page 6 & Page 7

* [x] **`Theorem aeq_aeqp` Proof:** Clarify where `(I.H.)` comes from in the proof.
* [x] **Formatting (`Theorem aeq_aeqp`):** Fix the formatting/line-break issue between the end of the `aeq_aeqp` proof and the start of the sentence "We now prove that Definition 2 implies...".
* [x] **Formatting (`Theorem aeqp_aeqs`):** Fix the same end-of-proof formatting issue at the end of the `aeqp_aeqs` proof on the following page (p. 7).
* [x] **Restructuring (Page 7):** Move the text starting from "Using the proofs in [Apinis and Ahman 2026]..." through the end of the paragraph into the proof of the lemma, and remove the duplicated information already present in that proof.

### References

* [x] **Update Citation:** Update the `[Apinis and Ahman 2026]` reference to reflect its publication in *Logical Methods in Computer Science* (LMCS).