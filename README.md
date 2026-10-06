# yk-site-tests

Black-box functional tests for [yk-site](https://github.com/tyklol/yk-site), written with Playwright (TypeScript) from `SPEC.md` only.
The tests never read the site's source; they run against a live URL.

## Run

```sh
npm ci
npx playwright install chromium
BASE_URL=http://localhost:8000 npm test
```

Against the deployed site:

```sh
BASE_URL=https://tyklol.github.io/yk-site/ npm test
```
