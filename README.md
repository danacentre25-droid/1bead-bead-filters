# 1bead — Bead Filters Data Feed

This repository builds and serves static JSON filter data for the **1bead.com** BigCommerce storefront via GitHub Pages.

---

## 1. Required GitHub Actions Secrets

To enable the automated nightly build, go to:
**Settings > Secrets and variables > Actions > New repository secret**

Add the following two secrets:
* **`BC_STORE_HASH`**: Your 1bead BigCommerce store hash (e.g. `xr85ifge`)
* **`BC_TOKEN`**: BigCommerce API token with **Products: read-only** scope

---

## 2. GitHub Pages Setup

1. In this repository, go to **Settings > Pages**.
2. Under **Build and deployment**:
   * **Source**: `Deploy from a branch`
   * **Branch**: `main`, Folder: `/docs`
   * Click **Save**.
3. Your data feed will be published at:
   `https://danacentre25-droid.github.io/1bead-bead-filters/`

---

## 3. Triggering a Manual Build

You can trigger a build at any time:
1. Go to the **Actions** tab.
2. Select **Build filter data** in the left sidebar.
3. Click **Run workflow**.
