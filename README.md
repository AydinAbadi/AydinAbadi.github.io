# Aydin Abadi website

This repository contains the static, production-ready website for Dr Aydin Abadi and the Cryptography and AI Security Lab. The `site` directory is the complete GitHub Pages artifact; it has no server, database, cookies or third-party runtime dependencies.

## Publish on GitHub Pages

1. Create a new public repository named `AydinAbadi.github.io` under the `AydinAbadi` account.
2. Upload the contents of this package to the repository's `main` branch. Keep `.github`, `site` and this README at the repository root.
3. In **Settings → Pages**, choose **GitHub Actions** as the publishing source.
4. The included workflow will publish the `site` directory. The initial address will be `https://aydinabadi.github.io/`.
5. After confirming that address works, add `www.aydinabadi.com` under **Settings → Pages → Custom domain**. GitHub recommends adding the custom domain in repository settings before changing DNS.
6. At the domain provider, change the `www` CNAME record to `AydinAbadi.github.io` (without a repository name). If the bare domain `aydinabadi.com` should also work, follow GitHub's current apex-domain instructions in its official documentation.
7. When GitHub's DNS check succeeds, enable **Enforce HTTPS**.

DNS changes can take up to 24 hours to propagate. Do not remove the current Google Sites connection until the GitHub Pages address has been tested.

Official guidance: [Publishing with GitHub Actions](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages) and [managing a custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

## Site map

- `/` — personal homepage
- `/research/` — research and impact
- `/publications/` — selected publications and software routes
- `/lab/` — lab overview
- `/lab/people/` — team and affiliated researchers
- `/lab/collaborate/` — industry and academic collaboration
- `/lab/join/` — vacancies and research opportunities
- `/about/` — biography, recognition, service and speaking
- `/contact/` — enquiry routes

Legacy URLs from the Google Sites version redirect to their new destinations.

## Updating the site

The deployed files are plain HTML, CSS and WebP/SVG assets. For small text changes, edit the relevant `site/.../index.html` file. After a commit to `main`, GitHub Pages publishes the update automatically.
