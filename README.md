#  Zambian Job Portal Scraper

**This is a full-stack job aggregation application built entirely within the **Google Ecosystem** (Google Sheets and Google Apps Script).

It demonstrates robust server-side logic (Scraping/Backend) and a dynamic, user-friendly client-side interface (Frontend).

## 🌍 Live Application
✨ **See the Job Portal Live:** https://sites.google.com/view/sebenzani-com/home](https://sites.google.com/view/sebenzani-com/home

***

## 🚀 Key Technical Features

* **Custom Web Backend (`Code.gs`):** Handles URL routing via the `doGet(e)` function to serve the main job listing (`Index.html`) or a dedicated job detail page (`Job.html`).
* **Automated Data Scraping:** The `runAllScrapers()` function uses **UrlFetchApp** to fetch, parse, and structure LinkedIn job data specifically for the Zambian market.
* **Server-as-a-Database:** Data is persisted, read, and managed directly from a **Google Sheet**, eliminating the need for an external database.
* **Robust Sharing Feature:** Each job can be shared via a unique URL (`/webappurl?job=JOB_ID`). This link goes to a standalone, dedicated landing page (`Job.html`), which then links back to the main Google Site. This is a common pattern for shareability in web applications.
* **Dynamic Frontend (`Index.html`):** Uses JavaScript and Google Apps Script's `google.script.run` API to handle initial data loading, "Load More" pagination, and client-side job filtering.

***

## 🛠️ Tech Stack

* **Backend & Logic:** Google Apps Script (JavaScript)
* **Database:** Google Sheets
* **Frontend:** HTML5, CSS3, ES6 JavaScript

***

## ✍️ Note on Development Process

To be transparent, I utilized **Google's Studio Bot (AI)** as a development partner. This helped accelerate the initial code generation, troubleshoot Apps Script-specific API calls, and refine the robust sharing logic, allowing me to focus on system architecture and solving the core problem: creating a functional, user-friendly job board from scratch.

***

## 🏃 Getting Started

1.  **Clone** this repository.
2.  Create a new **Google Sheet** and open the **Extensions** > **Apps Script** editor.
3.  Copy the code from `Code.gs`, `Index.html`, and `Job.html` into their corresponding files in the Apps Script editor.
4.  Create a file named `appsscript.json` (if not already visible) and paste the content from this repo.
5.  Run the `runAllScrapers()` function once to populate the "Jobs" sheet.
6.  **Deploy** the script as a Web App to view the live result.
