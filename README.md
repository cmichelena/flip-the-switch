# Flip the Switch

Remove one thing from the world today, give it some years to be replaced or none, and see what happens to population, GDP and life expectancy over the next century.

A thought experiment by [Vector56](https://vector56.com). The numbers are judgement calls. The mechanisms are the argument, and every lever is editable on the page.

## Run it

Open `public/index.html`. No build, no dependencies.

## Deploy on Cloudflare

Connect this repo in Cloudflare (Workers and Pages, create, connect to git).

- Build command: none
- Deploy command: `npx wrangler deploy`
- Or as a Pages project: build output directory `public`

Then add the custom domain, for example `flip.v56.dev`.

## Model

The simulation lives in one block at the top of the script in `index.html`, between `MODEL` markers. Fertility effects add, growth effects compound, and each switch's shock scales with the gap between the years given and the years its replacement takes to build.
