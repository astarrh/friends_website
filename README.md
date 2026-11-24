# Friends of the Shafter Library

Static one-page site for Friends of the Shafter Library.

Donate uses the PayPal hosted button already in `index.html`.

To preview, open `index.html` in a browser.

## Files

- `index.html`: the website.
- `desk-sign.html`: printable desk sign for the Shafter Library and Learning Center. Its QR code goes straight to the PayPal donation page.
- `desk-sign.pdf`: the desk sign, ready to print on one letter-size sheet.

## Hosting with GitHub Pages

The site is hosted from this repository with GitHub Pages. Every push to `main` updates the live site within a minute or two.

### Turn on Pages

1. On GitHub, open the repository and go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and the folder to `/ (root)`, then click **Save**.

The site will then be live at https://astarrh.github.io/friends_website/.

Everything in this repository is public once Pages is on, including the desk sign files.

### Use a custom domain

1. In **Settings → Pages**, type the domain under **Custom domain** and click **Save**. GitHub adds a `CNAME` file to the repository; keep it.
2. Set up DNS with your domain registrar:
   - **Subdomain** (for example `www.example.org`): add a `CNAME` record pointing to `astarrh.github.io`.
   - **Root domain** (for example `example.org`): add four `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`.
   - To have both work, set up both and enter the `www` version as the custom domain. GitHub then redirects the root domain to it.
3. DNS changes can take up to a day to take effect. Once the domain check in **Settings → Pages** passes, turn on **Enforce HTTPS**.

## Updating the desk sign PDF

If you change `desk-sign.html`, make a new PDF:

1. Open `desk-sign.html` in Edge or Chrome and choose **Print**.
2. Set the destination to **Save as PDF**.
3. Under **More settings**, turn on **Background graphics** and turn off **Headers and footers**.
4. Save it as `desk-sign.pdf`, replacing the old file.
