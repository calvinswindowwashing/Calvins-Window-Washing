# Calvin's Window Washing Website Setup

Welcome to your new website! Here are the step-by-step instructions to get this live on GitHub Pages and set up your calendar/forms.

## 1. Hosting on GitHub Pages
1. Go to [GitHub.com](https://github.com/) and create a new repository named `calvins-window-washing` (or anything you like).
2. Upload these exact files into the repository:
   - `index.html`
   - `styles.css`
3. **IMPORTANT:** Take the two images you provided me (`hero_image.jpg` and `Window Washing Logo Final.png`) and upload them to the exact same repository next to the html and css files. Make sure the filenames match exactly.
4. Go to the repository **Settings** > **Pages** (on the left sidebar).
5. Under "Build and deployment", set the **Source** to `Deploy from a branch`.
6. Under "Branch", select `main` (or `master`) and click **Save**.
7. Wait a few minutes, and GitHub will provide you with a live link to your new site!

## 2. Setting Up the Google Calendar Booking
To prevent double bookings and automatically email customers:
1. Open your Google Calendar for `calvinswindowwashingor@gmail.com`.
2. Click **Create** (top left) and select **Appointment schedule**.
3. Set your title (e.g., "Window Washing Appointment"), duration, and available hours.
4. Follow the prompts to finish saving the schedule.
5. Click on the created Appointment Schedule on your calendar grid, and click **Share**.
6. Select **Website embed** -> **Inline embed**.
7. Copy the `<iframe ...>` code they give you.
8. Open `index.html` in a text editor (like Notepad or directly on GitHub).
9. Find the `<!-- Google Calendar Appointment Scheduling iframe goes here -->` section (around line 96) and replace the dummy `<iframe>` with your real one. 

## 3. Setting Up the Contact Form
Since GitHub Pages is a static host, you need a service to send the contact form emails.
1. Go to [Formspree.io](https://formspree.io/) and create a free account using your email `calvinswindowwashingor@gmail.com`.
2. Create a new form and name it "Website Contact Form".
3. Formspree will give you an endpoint URL that looks like `https://formspree.io/f/XXXXXXXX`.
4. Open `index.html` and find the `<form action="https://formspree.io/f/YOUR_FORMSPREE_ID"...>` line (around line 124).
5. Replace `YOUR_FORMSPREE_ID` with the code Formspree gave you.

That's it! Your site is fully functional, professional, and completely free to host.
