# Deploy Frontend to Vercel

This Phase 1 frontend is a static site, so Vercel can host it easily.

## What Vercel will host

Vercel will host the files inside `frontend/`.

## Before deploying

You need your backend API running on a public URL first.

Example:

```text
http://your-ec2-public-ip:5000
```

## Important frontend setting

The frontend currently uses:

```text
http://localhost:5000
```

for local development.

Before Vercel deployment, update `frontend/api.js` so the API base URL points to your backend URL.

## Basic deployment steps

1. Push this repository to GitHub.
2. Create a Vercel account.
3. Import the GitHub repository into Vercel.
4. Set the Vercel root directory to `frontend`.
5. Deploy the project.

## Important note about HTTPS

Vercel serves your site over HTTPS.
If your EC2 backend only uses plain HTTP, browsers may block frontend requests.

The clean fix is:

- add a proper domain and HTTPS on the backend
- or wait for the later AWS phase where we place the backend behind a Load Balancer

## After deployment

Open the Vercel frontend URL and make sure:

- the page loads
- the backend health check succeeds
- tasks can be created and updated
