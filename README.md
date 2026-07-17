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
