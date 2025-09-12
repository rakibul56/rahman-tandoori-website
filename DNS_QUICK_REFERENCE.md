# 🌐 Quick DNS Setup Reference for rahmantandoori.de

## GoDaddy DNS Records to Add:

### Root Domain Record:
```
Type: A
Name: @
Value: 76.76.19.61
TTL: 3600
```

### WWW Subdomain Record:
```
Type: CNAME  
Name: www
Value: cname.vercel-dns.com
TTL: 3600
```

## Important Notes:
- ❌ Delete any existing A records for @ 
- ❌ Delete any existing CNAME records for www
- ✅ Keep MX records (for email)
- ⏰ Changes take 1-24 hours to propagate

## Verification:
- Test: https://rahmantandoori.de
- Test: https://www.rahmantandoori.de
- Check: https://dnschecker.org

## After Setup:
✅ Your website will be live globally  
✅ Automatic SSL certificate  
✅ Fast loading with Vercel's CDN  
✅ Automatic deployments from GitHub