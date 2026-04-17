# LandingRodi – GitHub + Cloudflare Pages Ready

## Structure
- `public/` static site files
- `functions/api/` Cloudflare Pages Functions
- `wrangler.toml` Cloudflare config

## Connect to Cloudflare Pages
Use **Connect to Git** in Cloudflare Pages, then select this repo.

### Build settings
- Framework preset: **None**
- Build command: *(leave empty)*
- Build output directory: `public`
- Root directory: *(leave empty unless you put this project in a subfolder)*

## Environment variable
Add this in Cloudflare Pages:
- `OPENAI_API_KEY`

Optional:
- `OPENAI_MODEL` = `gpt-4o-mini`

## Test routes after deploy
- `/`
- `/api/test`
- `/workspace/`

## Important
If `/api/test` does not return JSON, the project was not connected/deployed as a Pages project with Functions.
