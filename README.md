# Gatsby Boilerplate

![Fleek 2024 Rebrand Gatsby Boilerplate](https://github.com/fleek-tools/gatsby-template/assets/74613246/fbc70aff-0309-45c1-a250-2f290d0baf8c)

## 🚀 Project Structure

Inside of your Gatsby project, you'll see the following folders and files:

```text
/
├── src/
│   └── pages
│       └── index.js
├── static/
│   └── favicon.ico
├── gatsby-config.js
└── package.json
```

In Gatsby, static files refer to assets like images, fonts, CSS files, and other resources that are served directly to the client’s browser without any server-side processing. These files are added to the /static directory at the root of your project.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command         | Action                                      |
| :-------------- | :------------------------------------------ |
| `npm install`   | Installs dependencies                       |
| `npm run build` | Build your production site to `./build/`    |
| `npm run start` | Starts local dev server at `localhost:8000` |

## ⚡ How to deploy to Fleek

### 1. Create a `fleek.json` config file

You can configure this site deployment using [Fleek CLI](https://fleek.xyz/docs/cli/) and running:

```bash
 > fleek sites init
  WARN! Fleek CLI is in beta phase, use it under your own responsibility
   ? Choose one of the existing sites or create a new one. ›
    ❯ Create a new site
```

It will prompt you for a `name`, `dist` directory location & `build command`

- `name`: How you want to name the site
- `dist`: The output directory where the site is located, for this template it's `build`
- `build command`: Command to build your site, this will be used to deploy the latest version either by CLI or Github Actions

### 2. Deploy the site

After configuring your `fleek.json` file, you can deploy the site by running

```bash
fleek sites deploy
```

After running it you will get an output like this:

```bash
 WARN! Fleek CLI is in beta, use it at your own discretion
  > Success! Deployed!
  > Site IPFS CID: QmP1nDyoHqSrRabwUSrxRV3DJqiKH7b9t1tpLcr1NTkm1M

  > You can visit through the gateway:
  > https://ipfs.io/ipfs/QmP1nDyoHqSrRabwUSrxRV3DJqiKH7b9t1tpLcr1NTkm1M
```

### Extra features

- **Continuous Integration (CI):** `fleek sites ci` [Documentation.](https://fleek.xyz/docs/cli/sites/#continuous-integration)
- **Adding custom domains:** `fleek domains create` [Documentation.](https://fleek.xyz/docs/platform/domains/)

You can find more information about static builds in [Gatsby Documentation](https://www.gatsbyjs.com/docs/quick-start/)

## 👀 Want to learn more?

Feel free to check [Gatsby documentation](https://www.gatsbyjs.com/docs/conceptual/rendering-options/#static-site-generation-ssg).
