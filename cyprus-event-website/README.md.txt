yprus Prosperity Collective Landing Page
This repository contains the single-page HTML landing page for the "Cyprus Prosperity Collective" workshop, designed for female entrepreneurs and property investors in the Cyprus region.

The page features event details, benefits, host information, and a registration form powered by Google Firebase (Firestore).

🚀 Key Technologies
HTML5 & CSS3: Core structure.

Tailwind CSS: Used for all styling and ensuring a modern, mobile-responsive design.

Google Firebase (Firestore): Handles form submission and securely stores registration data (Name, Email, Phone, Interest) in a workshop_registrations collection.

🛠 Project Setup & Customization
Before deploying, ensure you complete the following mandatory steps within the event_landing_page.html file:

1. Update Placeholder Images
You must replace the placeholder URLs for the two image assets:

Tochni Village Visual: Update the src attribute for the image with the ID tochni-image.

Host Headshot (Marta Tracz): Update the src attribute for the image with the ID marta-image.

2. Configure Firebase Variables (Automatic in Canvas)
The form submission relies on global variables (__app_id, __firebase_config, __initial_auth_token) injected by the deployment environment (Canvas). If running this locally outside of the Canvas environment, you must manually define these variables in the <script type="module"> block to initialize Firebase and authentication correctly.

🌐 Deployment Instructions (Using GitHub Pages)
Since this is a single HTML file with inline CSS and JavaScript, deployment is straightforward:

Upload: Ensure both event_landing_page.html and this README.md are pushed to the root of your GitHub repository.

Activate Pages: Go to your repository's Settings tab, navigate to Pages, and set the Source Branch to main (or master) and the folder to / (root).

Live Site: Your site will be live within minutes at the URL provided by GitHub Pages (e.g., https://<username>.github.io/<repo-name>/).

✍️ Data Management
All registration data is saved to your associated Firestore database under the path:
/artifacts/{appId}/public/data/workshop_registrations