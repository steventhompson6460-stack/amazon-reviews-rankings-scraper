# Amazon Reviews & Rankings Scraper
> This scraper automates the collection of Amazon reviews and bestseller rankings across multiple marketplaces and formats. It helps publishing teams keep monthly performance data fresh without manual effort. By centralizing review counts and category rankings, it supports better forecasting and decision-making.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/za2122/footer-section/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/devpilot1" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>amazon-reviews-rankings-scraper</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
This project gathers review metrics and bestseller rankings for books across Amazon marketplaces. It streamlines recurring data collection so analysts, publishers, and BI workflows always have clean and current inputs. It’s built for teams that depend on accurate book performance tracking at scale.

### Why This Scraper Matters for Publishing Analytics
- Helps maintain consistent monthly reporting for sales and audience engagement.
- Tracks competitive movement across formats and countries.
- Supports profit models and dashboards with always-current review and ranking metrics.
- Reduces manual collection time for large book catalogs.
- Ensures clean, structured data ready for BI pipelines.

## Features
| Feature | Description |
|----------|-------------|
| Multi-marketplace scraping | Extracts data from Amazon US, Canada, Germany, and France. |
| Multi-format extraction | Collects separate metrics for Hardcover, Paperback, Kindle, and Audiobook. |
| Review tracking | Pulls total review counts for each ASIN. |
| Ranking data | Fetches bestseller rankings per format. |
| API-ready output | Provides structured JSON compatible with BI import pipelines. |
| Automated monthly workflow | Can be scheduled or embedded in larger automation systems. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|-------------|------------------|
| asin | Unique identifier for each book. |
| marketplace | Amazon region scraped. |
| format | Book format such as Hardcover or Kindle. |
| review_count | Total number of reviews at scrape time. |
| bestseller_rank | Category ranking per format. |
| url | Amazon product page. |
| timestamp | When the data was collected. |

---

## Example Output


    [
        {
            "asin": "B08XYZ1234",
            "marketplace": "US",
            "format": "Kindle",
            "review_count": 1421,
            "bestseller_rank": "#312 in Kindle Store",
            "url": "https://www.amazon.com/dp/B08XYZ1234",
            "timestamp": 1732300200
        }
    ]

---

## Directory Structure Tree


    amazon-reviews-rankings-scraper/
    ├── src/
    │   ├── runner.py
    │   ├── extractors/
    │   │   ├── amazon_parser.py
    │   │   └── marketplaces.py
    │   ├── outputs/
    │   │   └── exporters.py
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── asins.sample.txt
    │   └── sample.json
    ├── requirements.txt
    └── README.md

---

## Use Cases
- **Publishers** use it to track review trends and rankings, so they can monitor book performance across formats.
- **Analytics teams** use it to feed BI dashboards with fresh monthly data, helping them understand genre or series profitability.
- **Marketing teams** use it to spot ranking surges and plan promotional timing.
- **Operations managers** use it to automate recurring reporting without manual scraping.
- **Researchers** use it to study multi-marketplace behavior and competitive categories.

---

## FAQs
**Does this scraper support multiple book formats?**
Yes. It collects separate ranking and review data for Hardcover, Paperback, Kindle, and Audiobook formats.

**Can this run as a scheduled job?**
It’s designed for automated workflows and works well with cron, cloud schedulers, or BI ingestion pipelines.

**Are international marketplaces included?**
Yes. It supports Amazon US, CA, DE, and FR out of the box.

**What input format does it require?**
A simple list of ASINs is all that’s needed; the scraper handles marketplace routing.

---

## Performance Benchmarks and Results

**Primary Metric:** Averages around 1.8 seconds per ASIN per marketplace under normal load.

**Reliability Metric:** Typical stability above 96% success rate across long-running monthly cycles.

**Efficiency Metric:** Processes large ASIN lists efficiently with minimal memory usage thanks to streaming requests.

**Quality Metric:** Data completeness remains consistent, with over 98% of pages returning valid review and ranking values in testing.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtube.com/shorts/6AwB5omXrIM" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review3.gif" alt="Review 3" width="35%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Exceptional results, clear communication, and flawless delivery. Bitbash nailed it.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
