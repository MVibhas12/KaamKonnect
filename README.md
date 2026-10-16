# KaamKonnect

**The bridge to homes.** KaamKonnect is a cooperative-owned home-services marketplace for India. Customers book verified local workers, and workers earn fair wages. Workers also get access to welfare schemes and skill training.

**Live site:** https://MVibhas12.github.io/kaamkonnect/.

---

## Features

### For customers
- Browse **10 trades**: Plumbing, Electrical, Carpentry, Painting, AC & Appliance Repair, Home Cleaning, Pest Control, Gardening, Beauty & Wellness, and Packers & Movers.
- **Rule-based worker matching** by trade, city, distance, rating and price. No AI ranking is used.
- A **map with live tracking** of the assigned worker.
- **Emergency booking** for urgent jobs.
- **Transparent GST pricing**: every bill shows the service charge plus CGST and SGST (18%), with a downloadable tax invoice.
- **Demo payments** (UPI, card or cash).
- **Chat** for each booking.
- **Two-way ratings** after every completed job.
- A **grievance cell** that can escalate a complaint to a government portal.

### For workers
- A dashboard with bookings, earnings and statistics.
- Transparent payouts. A **5% platform fee** and a **5% upskilling fee** are deducted from the worker's payout and are never added to the customer's bill.
- **Government welfare schemes**: 11 schemes with eligibility checked automatically from the worker's profile and platform income.
- **Upskilling**: 14 courses of 4 lessons each, with shareable credentials.
- Worker sign-up requires joining a **cooperative society**, and a federation admin must approve it.

### For the federation admin
- Worker and cooperative-society approvals.
- Monitoring of bookings and grievances.
- A demand forecast with a suggested staffing plan.

### Across the platform
- **Aadhaar OTP verification** at sign-up (demo flow).
- **7 languages**: English, हिन्दी, मराठी, বাংলা, தமிழ், తెలుగు and ಕನ್ನಡ.
- Light and dark themes, and a layout that works on phones.
- An interactive home page with scroll-reveal sections, a painter scene you can paint with your cursor, and illustrated service cards.
- A refresh returns you to the page you were on.

---

## Demo accounts

The login page lists demo worker accounts: 10 for each trade, with IDs like `dw-plumber-1`. Use them to explore the worker side without signing up.

---

## Run locally

This is a single self-contained HTML file with no build step.

```bash
git clone https://github.com/YOUR-USERNAME/kaamkonnect.git
cd kaamkonnect
open index.html        # macOS
# or: start index.html (Windows) / xdg-open index.html (Linux)
```

## Deploy with GitHub Pages

1. Push `index.html`, `README.md` and `.nojekyll` to the `main` branch.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`, and click **Save**.
4. Your site will be live at `https://YOUR-USERNAME.github.io/kaamkonnect/` within a minute or two.

The empty `.nojekyll` file tells GitHub Pages to serve the files as they are, without processing them through Jekyll.

---

## Project structure

```
kaamkonnect/
├── index.html   # the entire app: HTML, CSS and JavaScript in one file
├── README.md
└── .nojekyll
```

## Tech notes

- Vanilla JavaScript with hash-based routing and no frameworks.
- Fonts come from Google Fonts: Anek Latin and Figtree, with Noto Sans fallbacks for the Indian scripts.
- All illustrations are hand-built inline SVG and canvas.
- On GitHub Pages, data (accounts, bookings, chats, ratings) is saved in each visitor's browser through `localStorage`. It is not shared between visitors or devices.

## Disclaimer

KaamKonnect is a demo project built for learning purposes. Aadhaar verification, payments, government-scheme data and statistics are simulated. Do not enter real Aadhaar numbers, card details or other personal information.

## License

MIT. You are free to use and adapt it.
