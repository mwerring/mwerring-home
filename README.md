# mwerring-home

The home page at https://mwerring.netlify.app, listing my projects.

Each project has its own repository and its own Netlify site. The `_redirects` file shows each one
under this address, for example `mwerring.netlify.app/glamolotl/` shows `glamolotl.netlify.app`.

## Adding a project

1. Deploy the project as its own Netlify site (for example `meview.netlify.app`).
2. Add one line to `_redirects`:
   ```
   /meview/*    https://meview.netlify.app/:splat   200
   ```
   Don't add a separate rule for `/meview` → `/meview/`: Netlify treats them as the same address,
   so that rule redirects forever. If the project uses relative links, have its page add the
   trailing slash itself (see the small script at the top of Glamolotl's `index.html`).
3. Add a card for it in `index.html`.
