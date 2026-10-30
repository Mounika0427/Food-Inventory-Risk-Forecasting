# Food Inventory & Restaurant Management

React 18, TypeScript, Vite and Tailwind CSS restaurant demo with menu browsing, cart, payment simulation, ingredient availability, inventory management, purchase management and consumption analytics.

## Run in VS Code

Install Node.js 20+, open this folder, then run:

```bash
npm ci
npm run dev
```

Open the local URL printed by Vite. For a production bundle:

```bash
npm run build
npm run preview
```

Admin demo login: **demo / demo123**. These public credentials demonstrate the interface only.

## Data and scope

Menu data is in `public/indian_food.csv`. State is stored in browser localStorage and sessionStorage. The cloudStorage module simulates shared storage within one browser; there is no deployed database, secure server authentication or real payment gateway. Use sample data only.

The repository name reflects the broader inventory forecasting project. This supplied app implements inventory calculations and analytics; it does not include a trained forecasting model. The root `manage.py` and `templates/` are legacy Python artifacts; a complete Django backend is not included. Run the React application with npm.

Source: `src/components/`, `src/utils/`, and `src/types/`.

## Validation status

Source review completed. A strict `tsc -b` check reports existing unused symbols and type errors, including an unsupported `jsx` attribute on a style element. The supplied `build` command uses `tsc` without build mode and does not check the referenced app project. Vite bundling could not be verified here because the uploaded node_modules came from another platform and lacks the Linux Rollup native dependency. Install fresh dependencies with `npm ci` on your machine. This source upload does not claim a clean production build.
