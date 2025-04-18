# Render-VPN
# Xray VMess WebSocket (no TLS) for Render

This is a minimal Docker-based Xray server designed for Render.com or Railway, using:
- VMess protocol
- WebSocket transport
- No TLS
- Works with default *.onrender.com domain

## Deploy

1. Fork this repo or upload it to your GitHub.
2. Go to https://render.com/new and choose "Web Service".
3. Point it to this repo.
4. Set the **port to 8080**.
5. Deploy.

## Client Config

```json
{
  "v": "2",
  "ps": "Xray-Render",
  "add": "your-app-name.onrender.com",
  "port": 80,
  "id": "Dvdr00",
  "aid": 0,
  "net": "ws",
  "type": "none",
  "host": "your-app-name.onrender.com",
  "path": "/xray",
  "tls": ""
}
