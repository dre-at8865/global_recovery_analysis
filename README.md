# Global Recovery Analysis

This project analyzes the drivers of economic crisis recovery across countries since 1980. The dashboard explores the central question: What separates countries that recover from crisis in 2 years from those that stagnate for decades?

## Live Dashboard

View the live dashboard here:
**[https://dre-at8865.github.io/global_recovery_analysis/](https://dre-at8865.github.io/global_recovery_analysis/)**

---

## How to Run Locally

This project is designed to run within a dev container or GitHub Codespaces, which has all dependencies pre-installed.

1.  **Install dependencies:**
    ```bash
    npm ci
    ```

2.  **Build data sources:**
    ```bash
    npm run sources
    ```

3.  **Start the development server:**
    ```bash
    npm run dev -- --host 0.0.0.0
    ```

4.  **Open in browser:**
    Once the server is running, open the URL provided in the terminal (usually `http://localhost:3000`). You can also use the following command:
    ```bash
    "$BROWSER" http://localhost:3000
    ```

## Project Structure

-   `/pages`: Contains the markdown files that define the dashboard pages.
-   `/sources`: Data source configurations and local data files (e.g., CSVs).
-   `/evidence.config.yaml`: Main configuration file for the Evidence project, including the deployment `basePath`.
-   `/.github/workflows`: Contains the GitHub Actions workflow for automatic deployment to GitHub Pages.

## Deployment

The dashboard is automatically built and deployed to GitHub Pages on every push to the `main` branch. 
