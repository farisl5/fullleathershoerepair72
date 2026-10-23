# Full Leather Shoe Repair

A responsive, independent website concept for the Upper West Side business. Built with vanilla JavaScript, CSS, and Vite. No backend, API keys, or paid services are required.

## Develop

Use Node.js 22 or newer.

```sh
npm ci
npm run dev
```

If the machine restricts the default npm cache, use `npm ci --cache /tmp/full-leather-npm-cache`.

## Edit

- `src/business.js`: business name, address, phone, and Google Maps URL.
- `src/main.js`: page content, services, image sources, navigation, and generated LocalBusiness structured data.
- `src/style.css`: colors, typography, layouts, and responsive styles.
- `index.html`: page title and search description. Update these too if business identity changes.
- `public/favicon.svg`: brand favicon.

Photography is illustrative Unsplash imagery, delivered with width, quality, and automatic-format parameters. Images require access to `images.unsplash.com`; fonts require `fonts.googleapis.com` and `fonts.gstatic.com`. System font fallbacks are included. Replace photography with licensed shop photos before an official launch. Verify service details with the business. No unverified opening hours, history, reviews, or prices are published.

## Production build

```sh
npm run build
npm run preview
```

The generated `dist/` directory can be served by any static host. Navigation, click-to-call, directions, responsive layouts, keyboard focus, reduced-motion support, SEO metadata, and structured data are included. There is no contact form requiring a server.

## GitHub and Vercel deployment

1. In this repository, commit the source and lockfile (exclude `node_modules` and `dist`): `git add .`, then `git commit -m "Build Full Leather Shoe Repair website"`.
2. For the initially empty GitHub repository, name the branch `main` with `git branch -M main`, then push with `git push -u origin main`.
3. Sign in to Vercel, choose **Add New → Project**, and import `farisl5/fullleathershoerepair72`.
4. Select **Vite**. Keep the repository root as the root directory, use `npm run build`, and use `dist` as the output directory. No environment variables are needed.
5. Click **Deploy**. Future pushes to `main` trigger production deployments. Add a custom domain in the project's domain settings if desired.
6. On the deployed site, verify the mobile menu, telephone link, directions link, imagery, and SEO information. Obtain business authorization and confirm all content before presenting the concept as its official website.

The website has not been pushed or deployed automatically.

## GitHub Pages

The `gh-pages` branch contains the built static site. In GitHub **Settings → Pages**, select **Deploy from a branch**, choose **gh-pages** and **/ (root)**, then save.

The site URL is `https://farisl5.github.io/fullleathershoerepair72/` after GitHub finishes publishing. Build updates with `npm ci` followed by `npm run build:pages`, then publish the contents of `dist/` to the `gh-pages` branch. Keep `.nojekyll` in that branch. Source code stays on `main`.
