# Fairway Finds — Website Guide

Your complete guide to managing and updating your website.

---

## 📁 File Structure

```
your-repo/
├── index.html        → Homepage
├── listings.html     → Browse all listings
├── contact.html      → Contact form
├── trade-in.html     → Trade-in request form
├── styles.css        → All styling (colours, fonts, layout)
├── script.js         → Site functionality
├── listings.json     → ⭐ YOUR LISTINGS DATA — edit this to update stock
└── README.md         → This guide
```

---

## ⭐ How to Add / Update Listings

All your listings live in **listings.json**. To add, edit or remove a listing:

1. Open your repository on **github.com**
2. Click on **listings.json**
3. Click the **pencil icon** (Edit) in the top right
4. Add or edit listings following this format:

```json
{
  "id": 7,
  "title": "Callaway Big Bertha Driver",
  "category": "Drivers",
  "price": 120,
  "condition": "Good",
  "description": "10.5° loft, regular flex shaft. Light scuffs on sole only.",
  "image": "https://your-image-link.com/photo.jpg"
}
```

5. Click **"Commit changes"** — the site updates instantly!

### Categories you can use:
- `Drivers`
- `Fairway Woods`
- `Irons`
- `Wedges`
- `Putters`
- `Bags`
- `Accessories`

### Condition options:
- `Excellent`
- `Very Good`
- `Good`

### For images:
- Upload photos to a free service like **imgur.com** or **imgbb.com**
- Copy the direct image link and paste it into the `"image"` field

---

## 📬 Setting Up Your Contact Forms (One-Time Setup)

Your forms use **Formspree** (free — up to 50 submissions/month).

1. Go to **formspree.io** and create a free account
2. Click **"New Form"**, name it "Contact" and copy the Form ID (e.g. `xpzvygkb`)
3. In GitHub, open **contact.html** and find this line:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
   Replace `YOUR_FORM_ID` with your actual ID
4. Do the same in **trade-in.html** (you can use the same or a separate form)
5. Commit the changes — forms will now send straight to your email!

---

## 🎨 Changing Your Business Name

1. Open each HTML file (`index.html`, `listings.html`, etc.)
2. Find `Fairway Finds` and replace with your business name
3. Update the `<title>` tags and meta descriptions too

---

## 📞 Updating Contact Details

In **contact.html**, find and update:
```html
<a href="mailto:hello@fairwayfinds.co.uk">hello@fairwayfinds.co.uk</a>
<a href="tel:+447700000000">07700 000 000</a>
```

---

## 🌐 Connecting a Custom Domain (Optional)

1. Buy a domain from **namecheap.com** (~£10/year)
2. In your GitHub repo go to **Settings → Pages**
3. Under "Custom domain" enter your domain name
4. In Namecheap, add a CNAME record pointing to `yourusername.github.io`

---

## 💡 Tips

- Keep condition ratings honest — buyers trust accurate descriptions
- Add clear photos for every listing — it significantly increases enquiries
- Respond to contact form submissions promptly for the best experience
- Commit changes at any time — the site updates within minutes
