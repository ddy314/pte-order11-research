# PTE size eleven: common-center pair obstructions

The integer ideal Prouhet–Tarry–Escott problem of size eleven remains open.
This project gives conditional results for symmetric solutions, not a solution
or a general nonexistence theorem.

**Main result.** If one side of a symmetric size-eleven solution consists of
five disjoint pairs about a common center and one remaining element, then its
height in integer coordinates centered at the symmetry center is at least

```
4264914784302653186685253811259318130882488669797076480249850785413789679541836572698823410736766760419030769
```

This is approximately 4.2649 × 10^108. The proof combines an exact one-parameter
normal form with an exhaustive finite-field calculation. It applies to
unbounded integer parameters and is not a bounded search over integer tuples.

For the larger class containing four common-center pairs, a two-parameter
normal form forces the additional divisors
23, 29, 37, 41, 43, 47, 53, 59, 67, 73 in the PTE constant.
A consequence of the published local classification already forces 29 when
there are three common-center pairs.

- [Proofs, scope, and literature](PROOF.md)
- `check_five_pairs_mod.py`: the 393-prime certificate and height calculation.
- `check_four_pairs_mod.py`: the two-parameter certificate and local patterns.

Run with Python 3.8 or newer, without third-party dependencies:

```
python3 check_four_pairs_mod.py
python3 check_five_pairs_mod.py
```

The scripts allow repeated roots after reduction modulo a prime. Distinct
integer roots can coincide modulo a prime, so excluding such reductions would
invalidate the argument.

These are research results with reproducible finite certificates. Their
novelty and publication suitability have not been established. No claim is
made about arbitrary nonsymmetric solutions or symmetric solutions outside
the stated pair configurations.
