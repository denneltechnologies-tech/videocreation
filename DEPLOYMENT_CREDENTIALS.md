# Video Creation Tool — Deployment Reference & Credentials

## 🚀 Repository & Hosting
- **GitHub Repository**: https://github.com/denneltechnologies-tech/videocreation
- **Active Branch**: `main`
- **VPS IP**: `69.62.106.189`
- **SSH User**: `root`
- **SSH Password**: `Kissinger2026@`

## 🎛️ Dokploy Control Panel
- **Dokploy URL**: http://69.62.106.189:3000 (or https://admin.growthshperegh.cloud)
- **Dokploy Admin User**: `otooaggreydennis@gmail.com`
- **Project Name in Dokploy**: `video Creation tool` (ID: `0X7ogyftEelHte5YLgiLo`)
- **Environment**: `production` (ID: `71zRaicjGXM-oll8evD9U`)
- **Dokploy App Name**: `videocreation-app-ghpn2026` (App ID: `app_videocreation_prod_2026`)

## ⚡ Automatic Deployment Webhook
- **Webhook URL**: `http://69.62.106.189:3000/api/deploy/video_webhook_ghpn_2026_auto`
- **Webhook Token**: `video_webhook_ghpn_2026_auto`
- **GitHub Webhook Setup**:
  1. Go to: `https://github.com/denneltechnologies-tech/videocreation/settings/hooks`
  2. Click **Add webhook**
  3. **Payload URL**: `http://69.62.106.189:3000/api/deploy/video_webhook_ghpn_2026_auto`
  4. **Content type**: `application/json`
  5. **Which events**: `Just the push event`
  6. **Active**: Checked ✅
  7. Click **Add webhook**

## 🗄️ Database (PostgreSQL)
- **Container Name**: `videocreation-postgres-db`
- **Host (Inside Dokploy Swarm Network)**: `videocreation-postgres-db`
- **External Port**: `5435`
- **Database**: `videocreation_db`
- **User**: `videocreation_user`
- **Password**: `Kissinger2026@`
- **Connection URL**:
  - Internal: `postgresql://videocreation_user:Kissinger2026%40@videocreation-postgres-db:5432/videocreation_db`
  - External: `postgresql://videocreation_user:Kissinger2026%40@69.62.106.189:5435/videocreation_db`

## 🔑 Environment Variables for Dokploy Application
```env
DATABASE_URL="postgresql://videocreation_user:Kissinger2026%40@videocreation-postgres-db:5432/videocreation_db"
DIRECT_URL="postgresql://videocreation_user:Kissinger2026%40@videocreation-postgres-db:5432/videocreation_db"
NEXTAUTH_URL="http://69.62.106.189:3000"
NEXTAUTH_SECRET="e9a1c8f35b29074d92ef7612c6a495da"
UGC_API_KEY="your_muapi_key_here"
WEBHOOK_URL="http://69.62.106.189:3000"
```
