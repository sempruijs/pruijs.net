# pruijs.net

Source for my personal site, built with Svelte and deployed on merge with main.

---

## What's in here?

- **Svelte** – Frontend framework
- **Tailwind CSS** – Utility-first styling
- **Nix Flakes** – Reproducible dev environment and build system
- **GitHub Actions** – Deploys the Nix build as a static site via GitHub Pages

---

## Getting Started

### With Nix (recommended)

The best way to work on this site is with Nix flakes.

1. Enter the development shell:

   ```bash
   nix develop
   ```

2. Run the development server:

   ```bash
   nix run .#dev
   ```

3. Build the app as a static site:

   ```bash
   nix build
   ```

4. Preview the build locally:

   ```bash
   nix run
   ```

---

### Without Nix

While using Nix is highly recommended for a robust setup, you can still work on this site with just `npm`:

1. Run the development server:

   ```bash
   cd site
   npm install
   npm run dev
   ```

2. Build the static website:

   ```bash
   cd site
   npm run build
   ```

---

## License

[MIT License](./LICENSE)
