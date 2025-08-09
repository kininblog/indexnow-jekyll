# Jekyll IndexNow SEO Automation Script

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Works with: Netlify](https://img.shields.io/badge/Works%20with-Netlify-00C7B7?logo=netlify)](https://www.netlify.com/)

A simple, powerful, server-side script to automatically submit your new and updated Jekyll posts to the **IndexNow API**. This ensures your content gets indexed by search engines like Bing and Yandex almost instantly, giving your SEO a significant boost without needing any complex plugins.

This script is designed for CI/CD environments like **Netlify**, **Vercel**, or **GitHub Actions**.

---

## Why Use This Script?

Search engines can take days or even weeks to discover new content on your site. The **IndexNow protocol** solves this by allowing you to "ping" search engines directly the moment your content is published.

This script automates that entire process:
1.  It runs automatically after your Jekyll site is successfully built.
2.  It finds all URLs that were published or updated *today*.
3.  It sends only these new URLs to the IndexNow API.

The result? Faster indexing, quicker traffic, and better SEO performance.

## Features

-   **Zero Dependencies:** No need to install any Ruby gems or npm packages. It's pure shell script.
-   **Fully Automated:** Set it up once in your deployment workflow and forget about it.
-   **Efficient:** Only submits URLs that have changed on the day of the build, respecting API limits.
-   **Smart Filtering:** Automatically ignores taxonomy pages like tags and categories.
-   **Easy to Adapt:** Can be quickly modified for other static site generators like Hugo, Eleventy, etc.

---

## Setup Guide

Follow these steps to integrate the script into your Jekyll site hosted on Netlify.
