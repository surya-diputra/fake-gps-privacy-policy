# Fake GPS privacy site

Static privacy and support site for **Fake GPS - Inertia Joystick**.

Production URL: `https://fake-gps.sdmv.my.id/`

## Publish with GitHub Pages

Use the contents of this directory as the root of a dedicated GitHub repository.

1. Create a public GitHub repository, for example `fake-gps-site`.
2. Push every file in this directory, including `.nojekyll`, `CNAME`, and `assets/`, to the repository's default branch.
3. Open repository **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then select the default branch and `/ (root)`.
5. In the DNS provider for `sdmv.my.id`, create a CNAME record:

   ```text
   Name: fake-gps
   Target: YOUR-GITHUB-USERNAME.github.io
   Proxy: DNS only until GitHub provisions HTTPS
   ```

6. In GitHub Pages settings, confirm the custom domain is `fake-gps.sdmv.my.id`, wait for DNS verification, then enable **Enforce HTTPS**.
7. Verify these public URLs:

   - `https://fake-gps.sdmv.my.id/`
   - `https://fake-gps.sdmv.my.id/app-ads.txt`
   - `https://fake-gps.sdmv.my.id/robots.txt`

Use the root URL as the Google Play privacy-policy URL and the developer website URL. Add the same root domain to the app's AdMob store settings so AdMob can crawl `app-ads.txt`.

## AdMob launch checklist

1. In Google Play Console, set the app's developer website to `https://fake-gps.sdmv.my.id/` and its privacy policy to the same URL.
2. Confirm the public Play listing shows that developer website under app support.
3. In AdMob, link the app to its Google Play listing.
4. In AdMob **Privacy & messaging**, use `https://fake-gps.sdmv.my.id/` as the privacy policy URL and publish the European regulations message.
5. Confirm `https://fake-gps.sdmv.my.id/app-ads.txt` returns the exact publisher record from this repository.
6. Request an app-ads.txt refresh in AdMob after deployment. Google notes that discovery and status updates can take up to 24 hours.

The policy page intentionally contains no advertising tags, analytics scripts, consent-message tags, forms, cookies, or browser storage.
