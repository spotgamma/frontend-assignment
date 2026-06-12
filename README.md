
# Assignment: Build a Live-Calculating Matrix UI

Candidates must build a web-based, editable grid (like a mini Google Sheet) that handles real-time formulas and circular dependencies.
The Specific Requirements The Grid:
 * It should be exposed as a GitHub repository named `spotgamma-frontend-takehome`
 * Render a 10x10 grid using CSS Grid.
 * The columns should be labeled A-J and rows 1-10.
 * The Formulas:
   * Each cell must accept raw text.
   * If a cell starts with an =, it must evaluate simple mathematical formulas (e.g., =A1 + B2) or ranges (e.g., =SUM(A1:A5))
   * Circular Dependencies: Implement a cycle-detection graph. If a user types =B1 in A1, and then types =A1 in B1, the app must safely block the update and display an error without crashing the DOM.
 * Performance: Changing the value of a top-level cell (e.g., A1) must dynamically and instantly update the calculated display values of all dependent cells (B1, C1, etc.) without lagging.
 * Shipping: Your app should ship using the gh-pages plugin.  That is, it should be exposed and able to be used at `https://${your_github_name}.github.io/spotgamma-frontend-takehome/`

You are free to use any LLM tools you like to tackle this assignment.  When finished, create a *private* GitHub repository with your solution.  Add the [sp0tgamma](https://github.com/sp0tgamma) GitHub user as a collaborator to your repository and email us a link to your repository at `eng+frontend_candidate@spotgamma.com` and to your gh-pages URL.


