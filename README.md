# Mohammad Ali Khan – Portfolio

A single-page animated portfolio built with plain HTML, CSS and JavaScript.
Animations use GSAP + ScrollTrigger and smooth scrolling uses Lenis (loaded from a CDN).
There is no build step: `index.html` is the whole site.

## Run it locally
Open `index.html` in a browser.

## Deploy on Vercel
1. Push this repo to GitHub.
2. In Vercel choose **Add New → Project**, import the repo.
3. Leave the framework as **Other** and the build command empty, then **Deploy**.

## Make the contact form send straight to Gmail
1. Get a free access key at https://web3forms.com using the Gmail address you want to receive messages.
2. In `index.html` find this line and paste the key between the quotes:

   `var KEY='',TO='mohammadalikhan6899h@gmail.com'`

3. Commit and push. Vercel redeploys automatically.

Until a key is added, the form opens a pre-filled Gmail compose window instead.

## Edit projects
Each project card in the **Selected work** section has a matching detail page defined in the `pages` object in the script at the bottom of `index.html` (search for `pages['`). Update titles, text and links there.
