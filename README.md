# project_autokz
AutoKZ
Modern AI-powered car advisor for the Kazakhstan market.

AutoKZ is a polished single-page web app that helps users explore cars, compare options, estimate ownership costs, and get AI-driven recommendations with a strong mobile-first experience and a presentation-ready desktop layout.

Why this project stands out
Built as a visually rich, interactive demo instead of a plain form-based prototype
Focused on the Kazakhstan used-car market
Designed for both phone screens and classroom/demo presentations
Includes AI analysis, saved favorites, history, budget matching, and Kolesa handoff
Main experience
AI car analysis by brand, model, year, and body type
Separate animated result panes:
Overview, Service, Ownership, Market, Verdict
Budget-based recommendations with curated picks
Favorites and recent history stored in the browser
Credit and leasing calculator
Trend and market-style insight blocks
AI chat section for quick automotive questions
Improved car image matching using Wikimedia / Wikidata sources
Kolesa.kz button that opens matching listings for the selected car
Design direction
The interface was intentionally redesigned to feel closer to a modern 2025-2026 concept:

soft glass-like cards
layered gradients and warm premium tones
smooth tab and panel transitions
intro/welcome sequence
mobile-friendly bottom navigation
richer desktop presentation without breaking the mobile version
Tech
HTML
CSS
Vanilla JavaScript
Groq API for AI responses
Wikidata / Wikipedia / Wikimedia Commons for car image lookup
No framework is required. The current version is shipped as a single-file frontend:

autokz_v3.html
Run locally
The fastest way is simply to open the file in a browser:

open autokz_v3.html
If you prefer serving it locally:

python3 -m http.server 8000
Then open:

http://127.0.0.1:8000/autokz_v3.html
How to use
Open the site
Add your Groq API key
Choose a brand, model, and year
Run the AI analysis
Explore the result panes
Save cars to favorites or open matching Kolesa listings
Deployment
Because the app is static, it can be deployed easily to:

GitHub Pages
Netlify
Cloudflare Pages
For GitHub Pages, rename the main file to index.html or create a copy:

cp autokz_v3.html index.html
Notes
The current version stores the Groq API key in the browser for convenience.
For a production-grade public launch, the AI request should go through a secure backend proxy instead of exposing direct frontend API access.
The Kolesa integration opens a targeted results page for the selected car. It does not scrape a single live listing inside the app, which keeps the frontend more stable.
Project goal
This project was built to feel more like a real automotive product concept than a typical school demo. The goal was to combine strong UI, useful car-market logic, and AI features into something that looks impressive on both mobile and desktop.

Future ideas
voice search
direct marketplace integrations through a backend
dark mode
multiple photo gallery per car
generation-aware model recommendations
more accurate cost-of-ownership formulas
Repository note
This repository also contains older experimental files from previous work. The main showcase for this project is:

autokz_v3.html
