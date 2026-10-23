# Rotten Tomatoes Scraper

Rotten Tomatoes Scraper (aka Rotten Tomato / RottenTomatoes / Rotten Tamato API) gets you 🎯 accurate, 🔍 detailed Rotten Tomatoes data as clean JSON in **Real-Time**.

No selectors, no proxies, no data cleaning. Just the data.

[**Try it now in the playground**](https://www.omkar.cloud/tools/rotten-tomatoes-scraper/playground) - See the data quality for yourself in one click, **No sign-up required**.

**Build on it free:** 1,000 calls every month, no credit card ❤️

[![Rotten Tomatoes Scraper API playground — run a live request in your browser, free, no sign-up](https://raw.githubusercontent.com/omkarcloud/rotten-tomatoes-scraper/master/playground.png)](https://www.omkar.cloud/tools/rotten-tomatoes-scraper/playground)

## What can I get

- 🍅 **Tomatometer & Popcornmeter for any title in one call** — by name, slug or URL, with Certified Fresh, Verified Hot, average ratings and review counts
- 🎬 **Full movie & TV pages** — critics consensus, top and all-critics scores, cast, credits, box office, trailer, photos, latest reviews & where to watch; every season and episode too
- 🔎 **Search & browse every list on the site** — search titles and people, browse streaming / in-theaters / coming-soon grids with 38 genres, ratings, score and 13 streaming-service filters, Top Box Office, the homepage carousels
- 🎭 **People, critics & editorial** — celebrity profiles with full filmographies, 30,000 critics and publications, ranked editorial guides and news

## Why Rotten Tomatoes Scraper

Most other Rotten Tomatoes APIs fail you in one of four ways:

- 🗄️ **Inaccurate, cached, stale data**
- 🧩 **Low-detail endpoints** — a few fields per call, never the full picture
- 💸 **Pay more to get the same data**
- 🪦 **Works today, breaks next month** — nobody maintains it

Rotten Tomatoes Scraper is scraped live on every call, priced honestly, and actively maintained.

## Example: A Full Rotten Tomatoes Movie

```json
{
  "ems_id": "7b2bcd9a-359f-3ffd-bbbd-abe9e5ce3f9e",
  "title": "Avengers: Endgame",
  "slug": "avengers_endgame",
  "link": "https://www.rottentomatoes.com/m/avengers_endgame",
  "year": 2019,
  "content_rating": "PG-13",
  "runtime_minutes": 181,
  "genres": ["Action", "Adventure", "Fantasy"],
  "synopsis": "Adrift in space with no food or water, Tony Stark sends a message to Pepper Potts as his oxygen supply starts to dwindle...",
  "critics_consensus": "Exciting, entertaining, and emotionally impactful, Avengers: Endgame does whatever it takes to deliver a satisfying finale to Marvel's epic Infinity Saga.",
  "tomatometer": 94,
  "popcornmeter": 90,
  "is_certified_fresh": true,
  "scores": {
    "critics": {
      "all": { "score": 94, "average_rating": 8.2, "review_count": 551, "liked_count": 518, "not_liked_count": 33 },
      "top_critics": { "score": 93, "review_count": 91, "liked_count": 85, "not_liked_count": 6 }
    },
    "audience": {
      "all": { "score": 90, "average_rating": 4.5, "review_count": 20472, "banded_rating_count": "50,000+ Ratings" }
    }
  },
  "release": { "release_date_theaters": "2019-04-26", "release_type_theaters": "wide", "release_date_streaming": "2019-07-30" },
  "credits": {
    "directors": [
      { "name": "Anthony Russo", "slug": "anthony_russo", "link": "https://www.rottentomatoes.com/celebrity/anthony_russo" },
      { "name": "Joe Russo", "slug": "joseph_russo", "link": "https://www.rottentomatoes.com/celebrity/joseph_russo" }
    ],
    "producers": [{ "name": "Kevin Feige", "slug": "kevin_feige" }]
  },
  "production": {
    "distributors": ["Walt Disney Pictures"],
    "production_companies": ["Walt Disney Pictures", "Marvel Studios"],
    "box_office_gross_usa": { "amount": 858400000, "currency": "USD", "text": "$858.4M" }
  },
  "poster_link": "https://resizing.flixster.com/zcGZJicE-5MRF19K_ZaNsE1a_48=/164x246/v2/https://resizing.flixster.com/hu13NxX2cqnYsnL7vDtkOoq7Z-A=/ems.cHJkLWVtcy1hc3NldHMvbW92aWVzLzQwYTA0ZmQyLTEzZmMtNGIwMS1hNDdjLTE3NWIwOTY2MzNkYi5qcGc=",
  "trailer": { "title": "Avengers: Endgame: Encore Trailer", "duration": "1:36", "thumbnail_link": "https://statcdn.fandango.com/MPX/image/NBCU_Fandango/588/215/thumb_B6F8D71D-0BA0-4F86-8826-1DDA78C3209C.jpg" },
  "cast": [
    { "name": "Robert Downey Jr.", "slug": "robert_downey_jr", "role": "Tony Stark", "link": "https://www.rottentomatoes.com/celebrity/robert_downey_jr" }
  ],
  "critic_reviews": [
    {
      "critic": { "name": "Amy Nicholson", "slug": "amy-nicholson", "is_top_critic": true },
      "publication": { "name": "FilmWeek (LAist)" },
      "date": "2019-09-27",
      "sentiment": "positive",
      "quote": "This is a feat of engineering... I felt a sense of catharsis finishing it."
    }
  ],
  "where_to_watch": { "primary_cta": { "label": "Buy Tickets", "affiliate": "fandango", "link": "https://www.fandango.com/avengers-endgame-encore-2026-246870/movie-overview" } }
}
```

*Trimmed for readability.*

## Get Started with 1,000 Free Calls

Start in the [playground](https://www.omkar.cloud/tools/rotten-tomatoes-scraper/playground) — try any endpoint with one click, no sign-up required.

Once you're happy with the data, start with the free plan for 1,000 free calls every month:

1. [Sign up on Omkar Cloud](https://www.omkar.cloud/auth/sign-up?redirect=/tools/rotten-tomatoes-scraper/playground) — free, no credit card.
2. Open the [Rotten Tomatoes Scraper playground](https://www.omkar.cloud/tools/rotten-tomatoes-scraper/playground) and enter any movie you like. Click **Get Live Data**.
3. Enjoy your data 😎.

## Endpoints

31 endpoints cover everything you need.

| Endpoint | Path | Returns |
|---|---|---|
| Movie Details | `/movies/details` | Everything on a movie page in a single call |
| Ratings Lookup | `/ratings` | Tomatometer + Popcornmeter for any title by name, slug or URL |
| Autocomplete | `/search/auto-complete` | Typeahead for titles, people and query completions |
| Search Titles / People | `/search`, `/search/people` | 20 per page; filter by type and year window |
| Movie Cast / Reviews / Where to Watch | `/movies/cast`, `/movies/reviews`, `/movies/where-to-watch` | Full credits, latest critic or audience reviews, streaming affiliates |
| Movie Videos / Photos | `/movies/videos`, `/movies/photos` | Every trailer and clip with stream links; full gallery |
| TV Show / Season / Episode Details | `/tv/details`, `/tv/seasons`, `/tv/episodes` | Series, season and episode pages with scores and episode lists |
| TV Cast / Reviews / Videos / Photos | `/tv/cast`, `/tv/reviews`, `/tv/videos`, `/tv/photos` | Same sub-resources for any series, season or episode |
| Browse Movies / TV Shows | `/browse/movies`, `/browse/tv` | Streaming, in-theaters, coming-soon grids with every site filter, 30 per page |
| Top Box Office / Homepage / Browse Filters | `/box-office`, `/home`, `/browse/filters` | Box office ranking, every homepage carousel, the filter vocabulary |
| Celebrity Details / Filmography / Photos | `/celebrities/details`, `/celebrities/filmography`, `/celebrities/photos` | Bio, best and worst titles, 25 credits per page, gallery |
| Search Critics / Critic Details | `/critics/search`, `/critics/details` | 30,000 critics and publications; one critic's profile |
| Critics / Publications Directory | `/critics/list`, `/publications/list` | Tomatometer-approved roster by letter |
| Editorial Guide / Articles | `/editorial/guide`, `/editorial/articles` | Ranked "best of" lists with scores; news by keyword |

## Pricing

High value, Low price.

| Plan | Price | Calls / month | Per 1,000 |
|---|---|---|---|
| **Basic** | **Free** | **1,000** — the most generous free plan | $0 |
| **Pro** | $16/mo | 20,000 | $0.80 |
| **Ultra** | $48/mo | 100,000 | $0.48 |
| **Mega** | $148/mo | 400,000 | $0.37 |

Need a bigger plan? Ask on [WhatsApp](https://api.whatsapp.com/send?phone=918178804274&text=I%20need%20a%20custom%20plan%20for%20the%20Rotten%20Tomatoes%20Scraper%20API.) or [Email](mailto:happy.to.help@omkar.cloud?subject=Custom%20plan%20for%20Rotten%20Tomatoes%20Scraper%20API&body=I%20need%20a%20custom%20plan%20for%20the%20Rotten%20Tomatoes%20Scraper%20API.).

- [**90 Day 2 Click Refund Guarantee**](https://www.omkar.cloud/refund-process)
- This is an excellent API made by Omkar Cloud, which is Rated Excellent — [4.7 based on 30 reviews on Trustpilot](https://www.trustpilot.com/review/omkar.cloud).

👉 [Start with Free Plan](https://www.omkar.cloud/auth/sign-up?redirect=/tools/rotten-tomatoes-scraper/playground) — 1,000 free calls/month

## 💬 Have Questions? We Have Answers.

You're a developer — we know how hard completing a project can be. So we offer full support: just message us and we'll reply ✅ with a solution within 1 working day.

[![Message Us on WhatsApp about Rotten Tomatoes Scraper](https://raw.githubusercontent.com/omkarcloud/assets/master/images/whatsapp-us.png)](https://api.whatsapp.com/send?phone=918178804274&text=I%20need%20help%20using%20the%20Rotten%20Tomatoes%20Scraper%20API.)

[![Ask Us by Email about Rotten Tomatoes Scraper](https://raw.githubusercontent.com/omkarcloud/assets/master/images/ask-on-email.png)](mailto:happy.to.help@omkar.cloud?subject=Help%20with%20Rotten%20Tomatoes%20Scraper%20API&body=I%20need%20help%20using%20the%20Rotten%20Tomatoes%20Scraper%20API.)

## Popular Scrapers by Omkar Cloud

- [**Google Maps Scraper (3,100+ GitHub Stars)**](https://github.com/omkarcloud/google-maps-scraper) — type "movie theaters in Los Angeles", get every business as a ready-to-call lead list: phones, emails, websites & reviews. Up to 100K free leads/month.
- [**IMDb Scraper**](https://www.omkar.cloud/tools/imdb-scraper) — movies, TV, ratings, cast, charts & box office
- [**G2 Scraper**](https://www.omkar.cloud/tools/g2-scraper) — G2 product details, ratings & AI-found contacts
- [**Website Email Contact Scraper**](https://www.omkar.cloud/tools/website-email-contact-scraper) — emails, phones & socials from any website
- [**AliExpress Scraper**](https://www.omkar.cloud/tools/aliexpress-scraper-api) — live product details, SKU variants, stock & shipping
- [**Booking Scraper**](https://www.omkar.cloud/tools/booking-scraper) — Booking.com hotels: prices, ratings, rooms & amenities

👉 [Start with Free Plan](https://www.omkar.cloud/auth/sign-up?redirect=/tools/rotten-tomatoes-scraper/playground) — 1,000 free calls/month
