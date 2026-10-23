# Diego’s Drive Tools

Public application information and branding for Diego Amicabile’s personal Google OAuth application used with rclone. This is a static informational site; it does not implement OAuth callbacks, receive credentials, or run file transfers.

## Published pages

- Homepage: https://diegoami.github.io/drive-tools-branding/
- Privacy: https://diegoami.github.io/drive-tools-branding/privacy.html
- Terms: https://diegoami.github.io/drive-tools-branding/terms.html
- Changelog: https://diegoami.github.io/drive-tools-branding/changelog.html
- Contact: https://github.com/diegoami/drive-tools-branding/issues

## Google Auth Platform → Branding

Use **Diego’s Drive Tools** as the application name and `assets/logo-512.png` as the logo. The PNG is an original 512 × 512 image with no Google branding. Set the homepage, privacy and terms links to the URLs above. Choose the real support and developer-contact email addresses in Google Cloud Console; no email address was inferred or published here.

Google requires accurate descriptions and ownership verification of the domains associated with the application. This site alone does not establish verification. Check Google’s treatment of your `diegoami.github.io` domain in Search Console and the Google Auth Platform; use a custom domain that you own if that domain cannot be accepted/verified. Do not add an assumed `github.io` authorized-domain value without checking. A custom domain can be added later through GitHub Pages settings and DNS.

The existing rclone OAuth clients, credentials, scopes and publishing status are not changed by publishing this site. For desktop rclone clients, authorization and callbacks stay in rclone: these static pages are not redirect URIs. Review the deployed privacy text against the actual workflow before submitting branding for review. Full `drive` access is described because it is the current configuration; brand verification does not replace any separate scope-verification requirements. No Google verification or endorsement is claimed.

Official references:

- https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification
- https://support.google.com/cloud/answer/15549049
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Development and deployment

No package installation or build is needed. Preview with `python3 -m http.server 8080` from the project directory. All navigation uses relative URLs and works under the GitHub Pages project subpath. No external scripts, fonts, trackers or runtime services are used.

GitHub Pages publishes the root of `main`; `.nojekyll` keeps files static. Commit and push updates to redeploy. Update `CHANGELOG.md` and `changelog.html` when changing public information. Keep credentials and rclone config files outside this repository.

The source and original logo assets are available under the MIT license. Third-party names and trademarks remain their respective owners’ property.
