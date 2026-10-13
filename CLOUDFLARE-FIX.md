Study Hub Cloudflare deployment fix

1. This project entry point is worker.js at the repository root. wrangler.jsonc must contain: "main": "worker.js".
2. In wrangler.jsonc, set the actual Cloudflare D1 database ID for binding DB. The database name is study-hub-db. Do not use a made-up ID.
3. Ensure the R2 bucket named study-hub-files exists for binding BUCKET.
4. Commit the files and redeploy the Worker.
5. Do not deploy only the public folder; deploy the project root with wrangler.jsonc and worker.js.
