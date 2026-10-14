# CovePeak Media

An original static marketing website inspired by the supplied Tyne screenshots. No Framer template code, stock assets, testimonials, or client results are included.

## Update the website

Edit `src/content/site.ts` to change the service descriptions and add the public Calendly event link to `bookingUrl`. Until that link is provided, the website clearly states that online booking is coming soon. Confirm the suggested process copy in `src/pages/index.astro` before launch.

The headline lives in the content file; homepage structure lives in `src/pages/index.astro`. Colors, spacing, and responsive layouts live in `src/styles/global.css`.

## Development

Requires Node.js 22.12 or newer.

```sh
npm ci
npm run dev
```

Build production files with `npm run build`. Astro generates the static website in `dist/`.

## Deploy to Vercel

Import the GitHub repository `covepeakmedia-sketch/covepeakmedia`. Choose the Astro framework preset, `npm run build` as the build command, and `dist` as the output directory. No environment variables or database are required.

After reviewing the preview, open the project’s Settings → Domains and add `covepeakmedia.com` and `www.covepeakmedia.com`. Choose the apex domain as the primary address and redirect www to it. Follow the exact DNS guidance shown by Vercel, preserving email records. Domain registration does not need to be transferred.

## Before public launch

- Add and test the actual Calendly booking URL.
- Confirm the proposed Understand → Build → Launch process describes the agency’s offering.
- Review desktop and phone layouts, navigation, and the full booking flow.
- Review privacy requirements before embedding booking widgets or adding tracking. This version links to booking and has no analytics, cookies, or lead collection scripts. The freely licensed DM Sans font is hosted with the website.

## Rollback

Revert the relevant GitHub commit and redeploy, or promote an earlier successful deployment in Vercel.
