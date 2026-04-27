# PayFlow — Arc Testnet

A modern USDC payment app on Arc Testnet with:
- **Payment Requests** — create, share links, auto check onchain
- **Swap** — USDC ↔ EURC via Circle App Kit
- **Bridge** — USDC from Ethereum Sepolia, Base Sepolia, Solana Devnet → Arc Testnet

## Stack
- Next.js 14 (App Router)
- Tailwind CSS
- Circle App Kit (Swap + Bridge)
- MetaMask + Phantom wallet support
- Arc Testnet (Chain ID: 2818)

## Deploy to Vercel

### 1. Import to Vercel
1. Push this repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import your GitHub repo
4. Vercel auto-detects Next.js

### 2. Add Environment Variable
In Vercel Dashboard → Project → Settings → Environment Variables:

| Name | Value |
|------|-------|
| `NEXT_PUBLIC_KIT_KEY` | `9437dcc1867fbd3cb7ab0e236140aa6f:ca22a2a485cb3152331130f9cd597c16` |

### 3. Deploy
Click "Deploy" — Vercel builds and gives you a live URL.

## Local Development

```bash
npm install
cp .env.example .env.local
# Edit .env.local with your KIT_KEY
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## Arc Testnet Details
- Chain ID: 2818
- RPC: https://rpc.arc-testnet.caldera.dev
- Explorer: https://explorer.arc-testnet.caldera.dev
