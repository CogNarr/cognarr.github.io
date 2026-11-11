# cognarr.org

Source for the CogNarr project website at [cognarr.org](https://cognarr.org).

The site is a static [Documenter.jl](https://documenter.juliadocs.org/) build.
GitHub Actions builds it on every push to `main` and deploys it to GitHub Pages.

## Build locally

    julia --project=. -e 'using Pkg; Pkg.instantiate()'
    julia --startup-file=no --project=. make.jl

Then open `build/index.html` in a browser.
