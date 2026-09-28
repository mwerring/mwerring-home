# mwerring-home

The home page at https://mwerring.netlify.app, listing my projects.

Each project has its own repository and its own Netlify site. The `_redirects` file shows each one
under this address, for example `mwerring.netlify.app/glamolotl/` shows `glamolotl.netlify.app`.

## Adding a project

1. Deploy the project as its own Netlify site (for example `meview.netlify.app`).
2. Add two lines to `_redirects`:
   ```
   /meview      /meview/                            301
   /meview/*    https://meview.netlify.app/:splat   200
   ```
3. Add a card for it in `index.html`.
