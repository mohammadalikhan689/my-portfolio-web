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

## Turn on the voice agent ("Talk to my AI" button)
1. In Retell AI, create the agent, paste in the prompt, and publish it. Copy the **agent ID**.
2. In Retell, create a **public key** and add your live site's domain to its allowed domains
   (use `localhost` for local testing). Never put your secret API key in this file.
3. In `index.html` find this line and paste both values between the quotes:

   `var PUBLIC_KEY='',AGENT_ID='';`

4. Commit and push. Open the live site, click **Talk to my AI**, press **Start call** and allow the microphone.

The button stays hidden until both values are filled in. It needs HTTPS (Vercel provides this).

## Edit projects
Each project card in the **Selected work** section has a matching detail page defined in the `pages` object in the script at the bottom of `index.html` (search for `pages['`). Update titles, text and links there.
The **Work** page also lists every YouTube video; edit the `VIDS` list in the same script.

## Voice agent ("Talk to my AI" button)
The button uses a Retell AI voice agent. Its public key and agent ID are in `index.html` on the line that starts with `var PUBLIC_KEY=`.

1. In the Retell dashboard, open **Public Keys**, open your key and add your live website address (for example `your-site.vercel.app`) to its allowed domains. Add `localhost` too if you test on your computer.
2. Make sure the agent is published.
3. Open the live site over https, click **Talk to my AI**, press **Start call** and allow the microphone.

Only the public key belongs in the page. Never put your Retell secret API key in `index.html`.
