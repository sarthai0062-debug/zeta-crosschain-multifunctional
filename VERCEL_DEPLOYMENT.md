# 🚀 Vercel Deployment Guide

## Quick Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/sarthai0062-debug/zeta-crosschain-multifunctional)

## Manual Deployment Steps

### Option 1: Deploy via Vercel Dashboard (Easiest)

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New" → "Project"
3. Import your GitHub repository: `sarthai0062-debug/zeta-crosschain-multifunctional`
4. Vercel will auto-detect the configuration from `vercel.json`
5. Click "Deploy"

### Option 2: Deploy via Vercel CLI

```bash
# Install Vercel CLI
npm install -g vercel

# Login to Vercel
vercel login

# Deploy
vercel

# Deploy to production
vercel --prod
```

## Configuration

The project is already configured with `vercel.json`:

```json
{
  "buildCommand": "cd frontend && npm install && npm run build",
  "outputDirectory": "frontend/dist",
  "framework": "vite"
}
```

## Environment Variables

No environment variables needed for the frontend! The contract address is already configured in `frontend/src/config.js`.

## After Deployment

1. Your app will be live at: `https://your-project.vercel.app`
2. Update the README.md with your live URL
3. Test the deployment:
   - Connect MetaMask
   - Mint an NFT
   - Transfer cross-chain

## Custom Domain (Optional)

1. Go to your project settings on Vercel
2. Click "Domains"
3. Add your custom domain
4. Follow Vercel's DNS configuration instructions

## Troubleshooting

### Build Fails

If build fails, check:
- `frontend/package.json` has all dependencies
- `vite.config.js` is properly configured
- No TypeScript errors

### App Doesn't Load

- Check browser console for errors
- Verify MetaMask is installed
- Ensure you're on ZetaChain testnet

### MetaMask Connection Issues

- Clear browser cache
- Reconnect MetaMask
- Check network configuration

## Performance Optimization

Vercel automatically provides:
- ✅ Global CDN
- ✅ Automatic HTTPS
- ✅ Edge caching
- ✅ Compression
- ✅ Image optimization

## Monitoring

View your deployment:
- **Dashboard**: https://vercel.com/dashboard
- **Analytics**: Check visitor stats
- **Logs**: View build and runtime logs

## Update Deployment

Every push to `main` branch will automatically deploy to Vercel!

```bash
git add .
git commit -m "update: improve UI"
git push origin main
```

Vercel will automatically rebuild and deploy. 🚀

## Cost

- **Free tier** includes:
  - Unlimited deployments
  - 100GB bandwidth/month
  - Automatic HTTPS
  - Perfect for hackathons!

## Support

- [Vercel Documentation](https://vercel.com/docs)
- [Vercel Discord](https://vercel.com/discord)
- [GitHub Issues](https://github.com/sarthai0062-debug/zeta-crosschain-multifunctional/issues)
