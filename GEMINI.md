# scDiffusion Presentation

## Project Overview
This project is a **Slidev** presentation titled "scDiffusion". It is a scientific presentation focusing on biological vision, data reality ("The Swamp"), and model runs (specifically diffusion models applied to single-cell data). It utilizes Vue.js components for interactive visualizations.

## Tech Stack
-   **Framework:** [Slidev](https://sli.dev/) (Vue.js based presentation framework)
-   **Core:** Vue 3, TypeScript, Vite
-   **Styling:** Windi CSS / Tailwind CSS (implicit in Slidev)

## Key Commands
Based on `package.json` and `README.md`, `pnpm` is the recommended package manager.

-   **Install Dependencies:** `pnpm install`
-   **Start Development Server:** `pnpm dev` (starts slide show at http://localhost:3030)
-   **Build for Production:** `pnpm build`
-   **Export to PDF/PNG:** `pnpm export`

## Directory Structure

### Core Files
-   **`slides.md`**: The main entry point for the presentation. Contains the slides content in Markdown format with embedded Vue components.
-   **`package.json`**: Project dependencies and scripts.

### Directories
-   **`components/`**: Custom Vue components used in the slides.
    -   `CellVisualizer.vue`: Visualizes the reverse diffusion process (noise to clusters).
    -   `DogDenoise.vue`, `DogNoise.vue`, `DogGallery.vue`: Likely visualization components for explaining diffusion concepts (using the common "dog" example).
-   **`resources/`**: specific scientific plots and data visualizations (e.g., UMAP plots, loss curves). Organized by run types (`proper_normalization_run`, `wrong_library_size_run`).
-   **`public/`**: Static assets like images (`Images/`) served directly.
-   **`pages/`**: Contains additional markdown files for slides (e.g., `imported-slides.md`).
-   **`snippets/`**: Code snippets for display or inclusion.

## Development Conventions
-   **Slides:** content is written in Markdown within `slides.md`.
-   **Components:** Interactive elements are built as Vue Single File Components (SFCs) in `components/` and used directly in markdown.
-   **Assets:** Scientific results are stored in `resources/` and referenced in slides.
-   **Theme:** Uses the `seriph` theme.
