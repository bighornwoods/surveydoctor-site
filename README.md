# surveydoctorapp.com

Public one-pager for **SurveyDoctor**. Not the app repo.

The product source stays private (`bighornwoods/bulletproof-redcap`). This repo is the website only.

## Local preview

```bash
cd ~/github/surveydoctor-site
python3 -m http.server 8080
# open http://127.0.0.1:8080
```

## Hosting

GitHub Pages, `main` branch, `/` root, custom domain `surveydoctorapp.com`.

### GoDaddy DNS (skip Website Builder)

Do **not** publish GoDaddy’s preview / Website Builder page. Use DNS only:

| Type | Name | Value |
|------|------|--------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `bighornwoods.github.io` |

After DNS propagates: repo **Settings → Pages → Custom domain** `surveydoctorapp.com`, then enable **Enforce HTTPS**.

Create mailbox **`hello@surveydoctorapp.com`** in GoDaddy email. That is the address on the page.

## Screenshot

`assets/app-light.jpg` is cropped from a local capture. The in-app chrome may still say the old product name. Recapture from a current SurveyDoctor build (enterprise + light) and replace both JPEGs when you can.

## Do not put on this page

- “LLC” until a real entity is filed
- A Buy button that goes nowhere
- Claims of signed / notarized installers
- Vanderbilt / REDCap endorsement
