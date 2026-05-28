# 🖥️ KFS CS Club — Certificate Verification

> Certificate verification portal for the **Introduction to Embedded Systems** course.  
> Students scan a QR code → site opens → instantly verified ✅

---

## 📄 Pages

| Page | Purpose |
|------|---------|
| `index.html` | Public verification page — students use this |
| `admin.html` | Add participants & organizers, auto-generate IDs |
| `generate-qr.html` | Generate QR codes from the admin data |

---

## 🪪 ID Format

| Type | Format | Example |
|------|--------|---------|
| Participant | `KFS-EMB-XX` | `KFS-EMB-07` |
| Organizer | `KFS-EMB-ORG-XX` | `KFS-EMB-ORG-03` |

IDs are auto-generated — just type the name and click Add.

---

## 🚀 Deploy on GitHub Pages

```bash
# 1. Create a public repo named kfs-cs-club on github.com

# 2. Push the files
git init
git add .
git commit -m "🎓 KFS CS Club Certificate Verification"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/kfs-cs-club.git
git push -u origin main

# 3. Enable GitHub Pages:
#    Settings → Pages → Source: Deploy from branch → main / root → Save
#    Live at: https://YOUR-USERNAME.github.io/kfs-cs-club
```

Or drag-drop files at github.com/new.

---

## 📋 Workflow

1. **Add students** → open `admin.html` locally, add names → IDs auto-generate
2. **Export** → copy the JSON from the Export tab → paste into the `getDB()` seed in `index.html`
3. **Push to GitHub** → site is live
4. **Generate QRs** → open `generate-qr.html`, set your GitHub Pages URL, download PNGs
5. **Attach QRs** to certificates — done!

---

*Built with ❤️ by KFS CS Club*
