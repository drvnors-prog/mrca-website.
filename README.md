# Music Research Centre Australia — website

The public website of Music Research Centre Australia, hosted free on GitHub Pages.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole website (design, text and form) in one file |
| `logo.svg` | The Centre's logo |
| `404.html` | The page shown if someone visits a link that does not exist |
| `CNAME` | Your domain name (edit this once you own the domain) |
| `README.md` | This guide |

## 1. Put the site online

1. Sign in at https://github.com and click **New repository**.
2. Name it `mrca-website`, choose **Public**, tick **Add a README file**, and click **Create repository**.
3. Click **Add file → Upload files**, drag in all the files, and click **Commit changes**.
   (Or use **Add file → Create new file**, type the file name, and paste the code.)
4. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and click **Save**.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/mrca-website/`.

## 2. Connect your own domain

1. Open `CNAME` and replace the example with your real domain, for example `www.musicresearchcentre.org.au`. Commit the change.
2. At your domain registrar, open the DNS settings and add:
   - A **CNAME** record: name `www`, value `YOUR-USERNAME.github.io`
   - Four **A** records for the bare domain (name `@`), pointing to:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. In **Settings → Pages**, enter the same domain under **Custom domain** and tick **Enforce HTTPS** once it is available. DNS changes can take up to 24 hours.

Check GitHub's current guide ("Managing a custom domain for your GitHub Pages site") in case these addresses change.

## 3. Turn on the expression-of-interest form

GitHub Pages cannot send email, so the form uses Formspree (free plan available).

1. Sign up at https://formspree.io with the email address that should receive submissions.
2. Create a new form. Formspree gives you an address like `https://formspree.io/f/abcdwxyz`.
3. In `index.html`, search for `YOUR_FORM_ID` and replace it with your code (for example `abcdwxyz`). Commit the change.
4. Submit a test entry on the live site and confirm it arrives in your inbox.

## 4. Editing the website later

- Open `index.html` on GitHub, click the pencil icon, change the text, and click **Commit changes**. The live site updates within a minute or two.
- **Founder photo:** upload a photo named `founder.jpg`, then in `index.html` replace
  `<svg style="color:var(--ink-2)"><use href="#mark"/></svg>` inside the `portrait` box with
  `<img src="founder.jpg" alt="Associate Professor Vaidya Bala" style="width:100%;height:100%;object-fit:cover;border-radius:4px">`.
- **Registration details:** once registered, replace `Registration in progress` in the footer with `ABN 00 000 000 000` (your real number).
