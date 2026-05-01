# RedevIQ
### Housing Society Redevelopment Intelligence

A free, open-source decision tool for housing society members, managing committees, and PMCs navigating the redevelopment process in Maharashtra. No installation. No login. No data sent anywhere. Works entirely in your browser.

---

## What it does

Redevelopment is one of the most complex financial decisions a housing society will ever make. Most members go into it without a clear picture of what they are entitled to, what the developer is actually offering, and whether the numbers add up.

RedevIQ puts the analysis in the hands of the society — not the developer, not the consultant.

| Tab | What you get |
|-----|-------------|
| **Setup** | Enter your society's plot area, member count, flat mix, and market rates. All calculations update live. |
| **Options** | Compare up to 5 redevelopment schemes (FSI, BUA, developer sale area, project cost, profit %) side by side. Best option highlighted automatically. |
| **Member Entitlement** | Any member enters their current carpet area and sees exactly what they get — new area, corpus, rent, shifting charges, total cash benefit — under each option. |
| **Developer Scoring** | Enter offers from up to 10 developers. Adjust scoring weights (carpet area %, corpus, rent, networth, completed projects, bank guarantee, litigation). Auto-ranked with a full scoring matrix. |
| **Compare** | Best option × best developer in one view. MC checklist of 16 items to verify before signing the Development Agreement. |

---

## How to use it

**Option A — Use online (once hosted):**
Open the link in any browser. No installation needed.

**Option B — Run locally:**
1. Download `index.html`
2. Open it in any browser (Chrome, Firefox, Safari, Edge)
3. That's it

No Python. No Node.js. No server. No internet required after the page loads.

---

## Key features

**Works for any society**
All fields are blank by default. Enter your own plot area, member count, flat sizes, FSI, sale rates, and scheme names. Works for any Maharashtra society — Mumbai, Pune, Thane, Nashik, or any other city.

**Nothing leaves your device**
All data is calculated and stored in your browser only. The Export JSON button saves a file to your computer. Nothing is sent to any server.

**Save and load**
Use the Save to browser button to preserve your data between sessions. Export JSON to share with your PMC or other MC members.

**Developer scoring is transparent**
Every scoring weight is visible and adjustable. The society decides what matters most — not a black box algorithm. Adjust the sliders, watch the ranking update in real time.

**MC checklist built in**
16 items that must be verified before signing the Development Agreement — covering legal, technical, financial, and governance requirements.

---

## Input fields explained

| Field | What to enter |
|-------|-------------|
| Net plot area | From your society's last approved plan (sq mt) |
| Reservation / encroachment | Area deducted for road widening, reservations etc. |
| Road setback | As per DCPR / local authority rules |
| MCGM amenity | 5% of net plot area handed over to MCGM |
| Ready Reckoner rate | From IGR Maharashtra website for your area (₹/sq mt) |
| Construction cost | Current rate in your area, typically ₹3,000–4,500/sq ft |
| Avg 1BHK / 2BHK carpet | Average MOFA carpet area of your existing flats |
| Corpus fund | Amount offered per sq ft of existing carpet (₹/sq ft) |
| Rent | Monthly rent offered per sq ft of existing carpet |
| Rent period | Number of months rent is guaranteed (typically 36–42) |
| Sale rate | Expected market rate per sq ft for new construction in your area |

---

## How the calculations work

**Net usable plot** = Gross plot − Reservation − Road setback − MCGM amenity (5%)

**Total BUA** = Net plot (sq mt) × FSI × 10.764 (sq ft conversion)

**Member carpet** = Existing total carpet × (1 + additional area %)

**Sale carpet** = (Total BUA × 85%) − Member carpet

**Project cost** = Construction + Corpus + Rent + Shifting + GST (18% on construction) + Consultant fees (approx) + MCGM charges (approx 4%) + Brokerage (5% of sale)

**Profit** = Sale value − Total project cost − Interest on peak finance

All figures are indicative. Have your licensed architect and PMC validate the numbers before any decision.

---

## Developer scoring methodology

Each developer is scored on 7 parameters. Weights are adjustable and must total 100 points.

| Parameter | Default weight | Basis |
|-----------|---------------|-------|
| Additional carpet area % | 25 | Higher % = higher score |
| Corpus fund (₹/sq ft) | 15 | Higher corpus = higher score |
| Rent offered | 10 | Higher rent = higher score |
| Developer networth | 15 | Higher = higher score |
| Completed projects | 15 | More = higher score |
| Bank guarantee | 10 | Higher BG = higher score |
| Litigation / track record | 10 | Clean record = full marks |

Scoring is relative — each parameter is scored as a percentage of the best offer received. A developer who offers the highest carpet area gets full marks on that parameter; others are scored proportionally.

**Important:** Scoring weights must be finalised by the MC/RDC/PMC before opening developer offers. Never create criteria after seeing the numbers.

---

## Who this is for

- **Managing Committee members** evaluating redevelopment options and developer bids
- **RDC (Redevelopment Committee)** members doing detailed due diligence
- **PMC (Project Management Consultants)** preparing feasibility reports for societies
- **General members** who want to understand what they are actually entitled to before voting

---

## Limitations

- Calculations are indicative, not legally binding
- FSI rules vary by scheme (33-7B, 33-9, 33-10, 33-11, 33-12B, 33-20B) — enter the correct FSI for your applicable scheme as confirmed by a licensed architect
- MCGM charges, premiums, and TDR costs vary by plot and scheme — refine with your architect
- The tool does not replace a licensed PMC or legal advisor

---

## Roadmap

- [ ] PDF export of full analysis report
- [ ] WhatsApp share of member entitlement summary
- [ ] Marathi language support
- [ ] RERA number verification for developers
- [ ] Pre-filled scheme templates for common Mumbai FSI rules

---

## Contributing

This is an open-source tool. Contributions welcome — especially from architects, PMCs, and legal professionals who can improve the calculation accuracy.

Fork → improve → raise a pull request.

---

## Licence

MIT — free to use, modify, and distribute. If you improve it, share it back.

---

*Built for housing society members who deserve to understand their own redevelopment — not just be told what to sign.*
