# Gym Membership Manager

A single-page gym management app (no build step, no dependencies).

## Features
- Owner and member logins
- Register members with personal details and a plan
- Create plans (monthly, quarterly, yearly, custom) with pricing
- Record payments and keep payment history
- List of members whose plans expire in the next 7 days
- Member dashboard: plan, expiry date, pending amount, payments

## Demo logins
- Owner: `admin` / `admin123`
- Member: `GM001` / `1234`

## Deploy on Render (Static Site)
1. Push these files to a GitHub repository (`index.html` at the repo root).
2. In Render, click **New -> Static Site** and connect the repository.
3. Settings: **Build Command** blank, **Publish Directory** `.`
4. Click **Create Static Site**. Your app goes live at `https://<name>.onrender.com`.

Alternative: **New -> Blueprint** and select the repo; `render.yaml` configures everything.

Every `git push` to the connected branch redeploys automatically.

## Notes
- Data is stored in the browser's localStorage (per device, not shared).
- Change the owner credentials in the `login()` function in `index.html` before real use.
- For multi-device use, replace localStorage with a backend database and hash passwords.
