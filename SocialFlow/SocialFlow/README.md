# SocialFlow (frontend prototype)

Social media management app for businesses, agencies and creators.
Everything runs in the browser. Data is saved in localStorage.

## Run it
1. Unzip to `D:\SocialFlow`.
2. Open the folder in VS Code (`code .`).
3. Double-click `index.html`, or right-click it and choose "Open with Live Server".

## Demo logins
- Admin portal: open `index.html#admin-login`
  - admin@socialflow.demo / Admin@123
- User portal: open `index.html#login`
  - maya@brewbloom.com / User@123 (agency workspace with sample data)
  - dev@fitnest.in / User@123 (separate empty business workspace)
- New users: `index.html#register`

## Routes (hash based)
Admin: #admin-login, #admin-dashboard, #admin-users, #admin-workspaces, #admin-activity, #admin-settings
User: #login, #register, #dashboard, #clients, #accounts, #posts, #create, #calendar, #campaigns, #analytics, #settings

## Where to edit in index.html
- `seed()` and `seedA()`: sample data, demo users and workspaces
- `V` object: user pages. `AV` object: admin pages
- `need()` and the wrapper list: role permissions
- `render()`: route guards and page layout
- CSS variables at the top: colours and dark theme

## Important
Sign-in here is simulated. Passwords use a simple demo hash, which is NOT secure.
Production needs a backend: Node.js + Express, MySQL, bcrypt, JWT and server-side role checks.

## Not built yet
React + Vite + Tailwind project, Team page, edit modals on every page, real backend, real social APIs.
