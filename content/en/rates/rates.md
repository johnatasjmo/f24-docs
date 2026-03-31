---
title: Rates
weight: 1
---


**For:** Agent | **Updated:** 2026-03-31

---

## What is a Rate Card?

A rate card is the core pricing record — it stores ocean freight for a specific route, carrier, container type, and validity period. Rate cards are the source data that quotes are built from.

**Rate card vs Quote:** A rate card is raw internal pricing. A quote is the client-facing commercial offer built from one or more rate cards, with markup, local charges, and terms added.

Rate cards are never edited — when a rate changes, you create a new card. This preserves pricing history.

---

## Create a Rate Card (Manual Entry)

1. Go to **Rates → New Rate Card**
2. Select the **carrier** (VOCC) — must exist in your directory
3. Set the **routing**: Origin (POL) and Destination (POD) as UN/LOCODE codes
   - Optional: Pre-carriage (PRE) and Place of Delivery (PDE) for inland legs
4. Select **container type** — one card per container type (20GP, 40GP, 40HC, etc.)
5. Enter **base freight** in USD
6. Set **validity dates** — the system warns if dates overlap an existing card on the same route
7. Click **Save**

---

## Import Rates via Excel

For bulk imports from a carrier tariff or rate sheet:

1. Go to **Rates → Import** → click **Download Template**
2. Fill in the template — one row per rate card:

| Column             | Required | Example      |
| ------------------ | -------- | ------------ |
| carrier_scac       | Yes      | `MSCU`       |
| origin_locode      | Yes      | `CRLIM`      |
| destination_locode | Yes      | `PAPTV`      |
| container_type     | Yes      | `40HC`       |
| base_freight_usd   | Yes      | `850`        |
| valid_from         | Yes      | `2026-04-01` |
| valid_to           | Yes      | `2026-06-30` |

3. Upload the file — the system validates each row and shows errors before importing
4. Click **Import** to save valid rows

> **Tip:** Use `YYYY-MM-DD` for dates. The carrier SCAC must match a VOCC in your directory.

---

## Rate Library

Go to **Rates** to browse all your rate cards. Filter by carrier, origin, destination, container type, validity date, or status (active / expired). Click any row to open the detail view.

Expired rates are hidden by default — toggle **Show expired** to include them in results.

---

## Common Issues

| Problem                    | Solution                                                              |
| -------------------------- | --------------------------------------------------------------------- |
| Carrier not in dropdown    | Add the shipping line to your directory with type VOCC                |
| Port not found             | Type the 5-character UN/LOCODE directly (e.g. `CRLIM`)                |
| Overlap warning            | A rate for the same route and container already exists in that period |
| Import error: unknown SCAC | The carrier SCAC must match a company in your directory               |
