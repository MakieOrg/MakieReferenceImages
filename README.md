# MakieReferenceImages

Holds the references for Makie's CI. Each minor version has its own separate orphan branch (`git checkout --orphan branch_name`) called `v0.X` so that one can clone the images for each version independently.
Each PR in Makie that has mismatching or new reference images should open a PR against the appropriate version in MakieReferenceImages (via CI).
Such a PR should only ever have one commit, or at least be merged in via squashing.
There's no real need to keep versions around as old images can always be regenerated using the original source in Makie.jl.