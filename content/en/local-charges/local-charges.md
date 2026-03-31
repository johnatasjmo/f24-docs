---
title: Local Charges
weight: 1
---


**For:** Agent | **Updated:** 2026-03-31

---

## What are Local Charges?

Local charges are port-related fees at origin or destination — separate from ocean freight. They cover terminal handling, documentation, customs, and other port services. Local charges are stored independently from rate cards and attached to quotes per lane.

### Charge Direction

| Direction   | Where                   | Examples                                          |
| ----------- | ----------------------- | ------------------------------------------------- |
| Origin      | Port of Loading (POL)   | THC, B/L fee, VGM, export customs                 |
| Destination | Port of Discharge (POD) | THC, delivery order, import customs, port storage |

### Charge Basis

| Basis         | Meaning                         |
| ------------- | ------------------------------- |
| Per container | Charged once per container      |
| Per B/L       | Charged once per bill of lading |
| Per shipment  | Charged once per shipment       |
| Per kg        | Charged per kilogram            |
| Ad valorem    | Percentage of cargo value       |

---

## Import Local Charges via Excel

1. Go to **Local Charges → Import** → click **Download Template**
2. Fill in the template — one row per charge:

| Column         | Required | Example                    |
| -------------- | -------- | -------------------------- |
| port_locode    | Yes      | `CRLIM`                    |
| direction      | Yes      | `origin` or `destination`  |
| charge_code    | Yes      | `THC`                      |
| charge_name    | Yes      | `Terminal Handling Charge` |
| basis          | Yes      | `per_container`            |
| container_type | Yes      | `40HC` or `ALL`            |
| amount_usd     | Yes      | `185`                      |
| valid_from     | Yes      | `2026-04-01`               |
| valid_to       | Yes      | `2026-12-31`               |

> **Tip:** Use `ALL` in `container_type` to apply the charge to every container size.

3. Upload — the system validates each row before importing
4. Click **Import** to save valid rows

---

## Attaching Local Charges to a Quote

When building a quote, click **Add Local Charges** on any lane. Search by port and direction — charges from your library are applied to the lane and appear in the quote export.

---

## Common Issues

| Problem                       | Solution                                                                            |
| ----------------------------- | ----------------------------------------------------------------------------------- |
| "Invalid LOCODE" error        | Use the 5-character UN/LOCODE code, not the city name                               |
| "Unknown basis" error         | Use exact values: `per_container`, `per_bl`, `per_shipment`, `per_kg`, `ad_valorem` |
| Charge not appearing in quote | Check the charge direction matches the lane (origin vs destination)                 |
