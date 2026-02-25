---
title: 'Bapagp'
date: 2025-06-10
permalink: /posts/jieun-blog-post-4/
tags:
  - API
  - yelp
  - typescript
---

# Smarter Restaurant Discovery, Built for You  
---

# Personalized Filtering with Bapago

---

# TL;DR

**Bapago** is a Yelp-powered restaurant discovery web application that allows users to dynamically filter and swipe through restaurants based on customized preferences.

Users can apply detailed filters such as **location, price range, rating, distance, delivery options, vegan availability, and sorting preferences**. The system fetches real-time restaurant data using the **Yelp API**, processes the filters through a structured backend, and presents results in an interactive swipe-based interface.

Instead of endlessly scrolling through search results, Bapago lets users explore restaurants in a focused, personalized way.


---

## Why did we build this?

We noticed that traditional restaurant search platforms overwhelm users with static lists and limited filtering flexibility. Even when filters are available, they often feel rigid or unintuitive.

Bapago was designed to:

- Provide **dynamic, multi-condition filtering**
- Allow real-time personalization
- Deliver a more engaging browsing experience through swipe interactions
- Give users better control over how results are sorted and ranked


---

## How does it work?

The system integrates directly with the **Yelp Fusion API** to retrieve restaurant data based on user-selected filters.

### Input:
- Location
- Category
- Distance radius
- Rating threshold
- Price level
- Delivery availability
- Vegan options
- Sorting preference (e.g., rating, review count)

### Backend Processing:
- Constructs dynamic query parameters
- Filters and normalizes API responses
- Applies structured sorting logic
- Returns optimized results to the frontend

The frontend then renders restaurants in a **swipe-based interface**, allowing users to quickly browse through options while maintaining filter constraints.


---

## Features

**Dynamic Filtering System**  
Supports multi-attribute filtering with customizable tag selections.

**Real-Time API Integration**  
Fetches live data from Yelp using structured query construction.

**Swipe-Based UI**  
Improves engagement compared to traditional static search results.

**Scalable Backend Logic**  
Designed to handle complex filter combinations efficiently.


---

## Screenshot Preview
<img width="1417" height="836" alt="search" src="https://github.com/user-attachments/assets/266dd3cc-b2d0-4288-b85a-772a94b0bf55" />
<img width="1418" height="832" alt="filter" src="https://github.com/user-attachments/assets/c763a8a3-f667-4be9-bbce-30c5e0693b00" />
<img width="1419" height="835" alt="fav" src="https://github.com/user-attachments/assets/d41dee19-dd48-42e8-a320-877fbf8f0094" />


---

## Challenges & Learnings

One major challenge was designing a filtering architecture that could handle multiple optional parameters without creating rigid or duplicated logic.

To address this, I:
- Structured a flexible `TagFilters` system to dynamically build API queries
- Ensured backend compatibility with evolving frontend filter requirements
- Implemented sorting logic to support multiple ranking strategies

This project strengthened my understanding of:
- API-driven architecture
- Backend-frontend integration
- Designing scalable filter logic
- Working in a collaborative development environment

---

## What’s next?

We plan to expand Bapago by:

- Implementing recommendation algorithms based on swipe behavior
- Introducing location-based auto-detection
- Improving ranking logic using personalized weighting

---

## Tech Stack

**Front-end:** Next.js, React, TypeScript  
**Backend:** Elysia, TypeScript  
**API Integration:** Yelp Fusion API  
**Filtering Logic:** Custom TagFilters architecture 

---

Bapago reimagines how users discover restaurants—by turning complex filtering into an intuitive, interactive experience.

