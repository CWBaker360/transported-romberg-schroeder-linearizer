# Transported Romberg Extrapolation for the Arcsine Schröder Linearizer

**Polynomial Composition Lifts and a Flat Infinite-Depth Limit**  
Wayne Baker — Independent Researcher  
Version 7.4 — October 1, 2026

## Overview

For each odd integer \(m\ge 3\), define

\[
S_m(z)=\sin(m\arcsin z), \qquad A(z)=\arcsin z,
\]

so that \(S_m\) is an odd polynomial and \(A(S_m(z))=mA(z)\) as an analytic germ at the origin.

The manuscript studies the finite-polynomial recursion

\[
P^{(m)}_{j+1}(z)
=
P^{(m)}_j(z)
+
\frac{mP^{(m)}_j(z)-P^{(m)}_j(S_m(z))}{m^{2j+1}-m},
\]

and shows that, after \(z=\sin u\), it is exactly Richardson–Romberg polynomial extrapolation of

\[
T_u(h)=\frac{\sin(hu)}{h}
\]

to \(h=0\) on the geometric nodes \(1,m,\ldots,m^{j-1}\).

## Main results

The paper establishes:

- an exact transported Romberg representation in forward polynomial iterates \(S_m^{\circ i}\);
- finite-depth moment cancellation, jet recovery, degree growth, and the exact leading defect
  \[
  \arcsin z-P^{(m)}_j(z)
  =\frac{m^{j(j-1)}}{(2j+1)!}z^{2j+1}+O(z^{2j+3});
  \]
- a scale/composition intertwining identity for geometric refinement towers;
- closed finite and limiting Lagrange weights in \(q\)-product form with \(q=m^{-2}\);
- \(C^\infty\) convergence of the infinite-depth tableau;
- a limiting Hadamard-lacunary trigonometric series whose complete Taylor jet at the fixed point is the identity jet;
- a nonzero flat discrepancy \(H_m(u)=u-F_m(u)\) at the origin;
- the functional-differential identity
  \[
  F_m(mu)=m\bigl(F_m''(u)+F_m(u)\bigr);
  \]
- nowhere real analyticity of \(F_m\), obtained from its non-exponential Fourier-coefficient decay together with the dilation identity above.

The cubic specialization \(m=3\) includes a small numerical table illustrating the flat gap without using numerics in the proof.

## Claim boundary

Richardson/Romberg extrapolation, geometric extrapolation grids, Schröder linearization, multiple-angle identities, and the general theory of lacunary trigonometric series are classical. The contribution claimed here is the exact transport of the classical extrapolation tableau into a finite polynomial-composition hierarchy for \(S_m\), together with the explicit infinite-depth analysis: a smooth Hadamard-lacunary limit with a prescribed full Taylor jet, a nonzero flat discrepancy, and a nowhere-real-analytic global limit.

The manuscript cites the classical extrapolation and Schröder literature together with Iserles and Sidi, and situates the infinite-depth limit within the lacunary-series literature of Zygmund, Kahane, and Katznelson.

## Files

- `baker_polynomial_composition_lift_v7_4.pdf` — compiled manuscript
- `baker_polynomial_composition_lift_v7_4.tex` — LaTeX source
- `CITATION.cff` — citation metadata
- `SHA256SUMS.txt` — SHA-256 checksums
- `RELEASE_CHECKLIST.md` — private-to-public release checklist

## Build

A standard two-pass `pdflatex` build is sufficient. Required packages are `amsmath`, `amssymb`, `amsthm`, `mathtools`, `geometry`, `booktabs`, and `hyperref`.

## Status

**Publication candidate.** The mathematical development is frozen at version 7.4. Repository visibility, licensing, DOI assignment, arXiv submission, and formal public-release timing remain separate decisions.

## Citation

Until a persistent identifier is assigned, use the metadata in `CITATION.cff`.
