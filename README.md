# Taimour Khan

Data Science student at the University of Management and Technology (UMT), Lahore, in the School of Systems and Technology. I build Python automations, web scrapers and data pipelines, and do applied machine learning.

I test what I build, and I report a number only when I can show where it came from.

## What I've shipped

### LeadForge: lead research that only says what it can prove

[Code](https://github.com/TaimourKhan2132/Lead-Forge) · [Live page](https://taimourkhan2132.github.io/Lead-Forge/)

A pipeline that finds small agencies from public sources, works out who their buyers are, and builds each one a sample list of ten prospects in its own niche and city.

- Opens every listing and website in a real browser on the day, and attaches the link that proves each claim.
- Run so far: 325 agencies discovered, 73 scored against a rubric, 20 sample packs built. 19 passed re-verification and one was blocked instead of stretched.
- When a manual check showed the first version's claims were often wrong, I rebuilt it around seven signals a person can confirm in ten seconds. A linter now rejects the old wording.
- It drafts the outreach and sends nothing. A person sends every message by hand.

Python, Playwright, httpx, BeautifulSoup, pandas, SQLite, pytest, GitHub Actions

### Synthetic ECG augmentation: accepted conference paper, first author

[Code and results](https://github.com/TaimourKhan2132/ecg-synthetic-research)

Does adding synthetic ECG images to real training data improve arrhythmia classification on real patients? Accepted at NEECON 2026.

- Adding Gemini-generated and NeuroKit2-simulated images raised macro-F1 from 0.869 to 0.892 on PTB-XL (p < 0.001 across 9 paired estimates).
- No leakage: patients are grouped across folds, and validation and test sets contain real ECGs only. Tests in the repo enforce both rules.
- The significance tables can be recomputed from committed predictions, without a GPU.

PyTorch, EfficientNet, NeuroKit2, scikit-learn, Vertex AI, Grad-CAM

### DailyPost: a live news site, built and maintained solo

[Code](https://github.com/TaimourKhan2132/dailypost) · [Live site](https://dailypostpk.page.gd)

A community publication for a non-technical owner. Anyone can submit a story, an editor approves it, and it is published.

- I took it from a front-end prototype to a deployed site with search, an editor dashboard and newsletter signups.
- Hardened before launch: CSRF tokens on every form, prepared statements throughout, rate-limited submissions and a login lockout.

PHP 8.2, MySQL, no framework

### Denver Crime Forecasting: weekly forecasts for 430 areas of a city

[Code and results](https://github.com/TaimourKhan2132/DenverCrime)

Weekly crime-count forecasts for every hexagon of Denver, built from 380,000 police records and tested only on future weeks.

- For property crime, the model beat all six naive baselines in each of four test windows.
- For crimes against people, it only tied a simple historical average, and the README says so.
- Found and corrected a bug in the city's own export that shifts two of three timestamps by exactly 7 hours.

Python, pandas, LightGBM, H3, Optuna, pytest, GitHub Actions

## Stack

| Area | Tools |
|---|---|
| Scraping and automation | Python, Playwright, httpx, BeautifulSoup |
| Data | pandas, SQL, SQLite, MySQL |
| Machine learning | PyTorch, scikit-learn, LightGBM, NeuroKit2 |
| Web | PHP, HTML, CSS |
| Tooling | Git, GitHub Actions, pytest |

## Contact

[taimourwk2132@gmail.com](mailto:taimourwk2132@gmail.com) · [LinkedIn](https://www.linkedin.com/in/taimour-khan-869476382) · Lahore, Pakistan (UTC+5)
