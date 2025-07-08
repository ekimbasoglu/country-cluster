# Country Cluster – Shopify Theme Extension

> Show shoppers a short list of **peer countries** (same continent) using a Cloudflare-edge lookup.

_Worker repo:_ **<https://github.com/ekimbasoglu/geo-locale-worker>**

_Shopify Demo:_ **<https://country-cluster-demo.myshopify.com>** *password: test*

---

## 📸 Demo
<a id="demo"></a>
![Screenshot 2025-07-08 at 16 06 27](https://github.com/user-attachments/assets/a3186194-f105-4b81-ac7b-17e87249d44d)

https://github.com/user-attachments/assets/5cf9731d-ee3a-4cd6-8b90-efd817662646



---

## 🔧 What’s inside
| Folder | Purpose |
|--------|---------|
| **extensions/country-cluster/** | Theme-app extension (Liquid + JS + ~locales~) |
| **shopify.app.toml** | App manifest – client ID only (no secrets) |

> The Cloudflare Worker that powers the API lives in a **separate repo** (linked above) to keep secrets and deployment history isolated.

---

## 🚀 Quick start

```bash
git clone https://github.com/ekimbasoglu/country-cluster
cd country-cluster

# 1. Set up Shopify credentials
cp .env.example .env          # fill in API secret, scopes, etc.

# 2. Run the app in a dev store
shopify app dev --store <my-dev-store>.myshopify.com
