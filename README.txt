Files included:
- public/index.html    --> the static site (already using your trained model coeffs)
- firebase.json        --> hosting config (public folder)
- .firebaserc          --> replace 'your-firebase-project-id' with your project's id

Quick deploy steps (on your machine):
1) Install firebase tools: npm install -g firebase-tools
2) Login: firebase login
3) Initialize (if not yet): firebase init hosting --project your-firebase-project-id
   - set public directory to 'public' (or keep existing)
   - choose 'no' when asked to configure as a single-page app (unless you want SPA rewrite)
4) Copy these files into your local project folder, or git clone this repo
5) Deploy: firebase deploy --only hosting --project your-firebase-project-id
6) Your site will be available at https://<your-project-id>.web.app or https://<your-project-id>.firebaseapp.com

Notes:
- This is a fully static client-side model. The model coefficients are visible in the JS.
- If you need the full Streamlit experience (Python server), consider Streamlit Community Cloud (free) or Firebase+Cloud Run (requires billing account / Blaze).
