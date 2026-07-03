# VoyaLift Website

Static website for App Store Connect links:

- Privacy Policy: `/privacy/`
- Terms of Use (EULA): `/terms/`
- Support URL: `/support/`

## GitHub Pages deployment

1. Create a public GitHub repository, for example `voyalift-site`.
2. Copy everything inside this `Website/` folder into that repository.
3. In GitHub, open `Settings -> Pages`.
4. Set `Build and deployment` to `Deploy from a branch`.
5. Choose the `main` branch and `/root`.
6. Save and wait for GitHub Pages to publish.

Default URLs before the custom domain is active:

```text
https://<github-user>.github.io/voyalift-site/privacy/
https://<github-user>.github.io/voyalift-site/terms/
https://<github-user>.github.io/voyalift-site/support/
```

## Custom domain

In the GitHub Pages repository, add `voyalift.com` under `Settings -> Pages -> Custom domain`.

For a `www` subdomain, add this DNS record at your domain provider:

```text
Type: CNAME
Name: www
Value: <github-user>.github.io
```

For the root domain, follow GitHub Pages' current A/AAAA record instructions in the Pages settings screen.

## Before publishing

- Confirm `support@voyalift.com` forwards to a real inbox before App Store submission.
- Use `https://voyalift.com/privacy/`, `https://voyalift.com/terms/`, and `https://voyalift.com/support/` in App Store Connect.
- Test both pages in a private browser window.
