# bohramatch-site

The public site for **BohraMatch**. Static HTML, no build step, served by GitHub Pages.

**Live at:** https://taha-lakdawala.github.io/bohramatch-site/

It exists because three URLs have to be public before the app can ship:

| Page | Needed by |
|---|---|
| `index.html` | Meta, as the business website for the WhatsApp Business account |
| `privacy.html` | Google Play data safety form, Apple App Store, Meta business verification |
| `delete-account.html` | Google Play, which requires an account-deletion route reachable **without installing the app** |
| `terms.html` | Play and App Store user-generated-content policies |

## Editing

Edit the HTML and push to `main`. Pages redeploys in about a minute.
`style.css` holds the tokens, which mirror `src/theme/tokens.ts` in the app repo. Change
one, change the other.

Keep the `Last updated` date at the top of `privacy.html` and `terms.html` current whenever
either changes. A stale date on a privacy policy is something reviewers check.

## When a domain is bought

1. Add a `CNAME` file to this repo containing the bare domain, for example `bohramatch.app`.
2. Point the DNS at GitHub Pages.
3. Update every published URL: the Meta business profile, the Play Console data safety form
   and the account-deletion URL, and `ARCHITECTURE.md` in the app repo.

## Contact

The contact address on every page is `tahalakdawala03@gmail.com`. It has to be a real,
monitored inbox, because both Meta and Google check it.
