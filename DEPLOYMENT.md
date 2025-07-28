# c8a212c1-28

This project was deployed from Bolt.new and is configured for automatic deployment to Cloudflare Workers.

## 🚀 Deployment Status

Your Shopify store is automatically deployed when you push to the main branch.

**Managed Infrastructure:**
- ✅ **GitHub Repository**: Hosted and managed automatically
- ✅ **Cloudflare Workers**: Deployed using managed Cloudflare account
- ✅ **GitHub Actions**: Configured for automatic deployment

## 🔧 Environment Variables Setup

Since environment files (.env) are excluded for security reasons, you'll need to configure your Shopify credentials as GitHub repository secrets:

### Required Secrets:
Add these secrets in your GitHub repository settings (Settings → Secrets and variables → Actions):

```
NEXT_PUBLIC_SHOPIFY_SHOP=your-shop-name.myshopify.com
NEXT_PUBLIC_SHOPIFY_STOREFRONT_ACCESS_TOKEN=your_storefront_access_token
```

### How to get your Shopify credentials:
1. **Shop Name**: This is your store's domain (e.g., `mystore.myshopify.com`)
2. **Storefront Access Token**: 
   - Go to your Shopify Admin
   - Navigate to Apps → Manage private apps
   - Create a private app or use existing one
   - Enable Storefront API access
   - Copy the Storefront access token

## 🌐 Live URLs

- **Production**: https://c8a212c1-28.workers.dev
- **Repository**: https://github.com/rapidsd/c8a212c1-28

## 📋 Deployment Process

1. **Code**: Push changes to the main branch
2. **Build**: GitHub Actions automatically builds your project
3. **Test**: Runs any configured tests
4. **Deploy**: Deployed to Cloudflare Workers using managed infrastructure

## 🛠️ Local Development

If you want to run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/rapidsd/c8a212c1-28.git
   cd c8a212c1-28
   ```

2. Install dependencies:
   ```bash
   pnpm install
   ```

3. Create a `.env.local` file with your Shopify credentials:
   ```
   NEXT_PUBLIC_SHOPIFY_SHOP=your-shop-name.myshopify.com
   NEXT_PUBLIC_SHOPIFY_STOREFRONT_ACCESS_TOKEN=your_storefront_access_token
   ```

4. Start the development server:
   ```bash
   pnpm dev
   ```

## 📚 Documentation

- [Shopify Storefront API](https://shopify.dev/docs/api/storefront)
- [Cloudflare Workers](https://developers.cloudflare.com/workers/)
- [GitHub Actions](https://docs.github.com/en/actions)

---

*Deployed with ❤️ from [Bolt.new](https://bolt.new)*
