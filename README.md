# 🌍 The Global Platforms Data
### A Curated, Open-Source JSON List of the World's Major Online Platforms

[![File Type](https://img.shields.io/badge/Data%20Format-JSON-blue.svg)](platforms.json)
[![Open Source](https://img.shields.io/badge/License-CC0-green.svg)](LICENSE)

***

## 🌟 What the Heck is This?

Welcome to a meticulously maintained, open-source list of major online platforms and services, structured in a clean, easily consumable JSON format.

If you've ever needed a reliable, categorized, and structured directory of search engines, social media sites, streaming platforms, and more—complete with links and icons—this is your go-to source.

This data is perfect for building custom search bars, dynamic directories, research projects, or simply powering the "link out" features in your own apps.

***

## 📁 `platforms.json` Structure

The central file, `platforms.json`, is organized by **categories**, with each category holding an array of **platforms**.

We made sure every single platform object is standardized and includes all the fields you requested. It’s consistent, correct, and ready to be consumed by any modern application.

### The Platform Object

Each platform entry includes the following fields:

| Key | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| `id` | `string` | **A unique, production-ready identifier** for the platform. | `search_google` |
| `name` | `string` | The official name of the platform (e.g., Google). | `Google` |
| `category` | `string` | **The name of the category** it belongs to. | `Search Engines` |
| `description` | `string` | A very brief, one-line summary of the platform. | `Dominant global search engine` |
| `about` | `string` | A longer, more informative description. | `Google Search is the most widely used...` |
| `link` | `string` | The main URL for the platform. | `https://www.google.com/` |
| `searchLink` | `string` | The parameterized URL for direct searching. Use this with `?q=` or equivalent. | `https://www.google.com/search?q=` |
| `icon` | `string` or `null` | A standardized icon identifier (e.g., from [Simple Icons](https://simpleicons.org/)). Can be `null`. | `si:SiGoogle` |

### JSON Example Snippet

```json
{
  "categories": [
    {
      "name": "Search Engines",
      "platforms": [
        {
          "id": "search_google",
          "name": "Google",
          "category": "Search Engines",
          "description": "Dominant global search engine",
          "about": "Google Search is the most widely used search engine...",
          "link": "[https://www.google.com/](https://www.google.com/)",
          "searchLink": "[https://www.google.com/search?q=](https://www.google.com/search?q=)",
          "icon": "si:SiGoogle"
        }
        // ... more platforms
      ]
    }
    // ... more categories
  ]
}
