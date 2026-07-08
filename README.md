# Cheap worlds first: two-stage K-annealing

Methods paper: evolve twists on a 10% goal subsample (cheap, noisy
fitness), consolidate with a short full-goal tail seeded from the
stage-one population.  Beats full-goal baselines -- including a 5x-budget
one -- at every environment and scale tested (9x9 pilot, 13x13, 15x15;
25x25 in progress), and finds the *same* attractor objects (cycle
Jaccard 1.00 in the pilot).

Source assets are tagged in main.tex header: scripts 46/48/49/50/52 in
`gridFour/notebooks/attractor-fingerprint-probe/`, the
`goal-subsampling-validation/` series, and the campaign manifests in
`gridOps/vars/`.  Synced run data under
`/media/merlin/grid-twist/gridtwist-outputs/` (anneal experiments, tails,
and their K=1 baselines).

Build: `latexmk -lualatex main.tex`.  Includes vendored (same set as
twists-infodesics / twists-home-vectors).
