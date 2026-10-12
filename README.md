# Centurion Showdown

A static battle damage calculator for Centurion Showdown. Open `index.html` in a
browser or publish the repository with GitHub Pages.

The calculator uses the matchup chart and damage rules from
`Adventurer_damage_calculator!.ipynb`. Effectiveness changes the attack by one
doubling/halving step for each matching attacking and defending element pair;
choosing the same attacking element twice does not count it twice. When the net
effectiveness is positive, nonzero DEF absorbs one advantage step; immunity
always results in zero damage. Secret types are not supported.

## Website deployment

The calculator's GitHub Pages URL is:
https://chansey4759.github.io/Centurion-Showdown-Coding-services-/

The old `https://centurion_showdown_calculator.github.io/` link does not
identify this repository's Pages site. GitHub Pages project URLs use the
repository owner's username and repository name.

To publish the calculator:

1. Commit and push `index.html`, `styles.css`, `script.js`, and
   `.github/workflows/pages.yml` to `main`.
2. In the repository's **Settings > Pages > Build and deployment**, select
   **GitHub Actions** as the source.
3. Open **Actions > Deploy calculator to GitHub Pages** and run the workflow
   if it has not already started. Future pushes to `main` deploy automatically.
4. Wait for a successful deployment, then open the URL above.

The workflow publishes only the calculator's HTML, CSS, and JavaScript.
