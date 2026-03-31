---
title: Carriers & Container Types
weight: 1
---


**For:** All users | **Updated:** 2026-03-31

---

## What is the Carriers Table?

The global list of shipping lines (Vessel Operating Common Carriers) recognized by the platform. Managed by Flete24 — visible to all tenants, read-only.

When creating a rate card, the carrier dropdown pulls from this list. The AI extraction pipeline uses SCAC codes and synonyms to identify carriers in uploaded documents.

---

## Shipping Lines (27 VOCCs)

| Carrier Name | SCAC | Alternate SCACs |
| ------------ | ---- | --------------- |
| ANL          | ANNU |                 |
| APL          | APLU |                 |
| CMA CGM      | CMDU |                 |
| COSCO        | COSU |                 |
| Evergreen    | EGLV |                 |
| Hamburg Sud  | SUDU |                 |
| Hapag-Lloyd  | HLCU |                 |
| Heung-A      | HASL | 11QU            |
| HMM          | HDMU |                 |
| KMTC         | KMTU |                 |
| Maersk       | MAEU | MAEI            |
| Matson       | MATS |                 |
| MSC          | MSCU |                 |
| Namsung      | NSRU |                 |
| ONE          | ONEY |                 |
| OOCL         | OOCL | OOLU            |
| PIL          | PCIU |                 |
| RCL          | RCLU | REGU            |
| Safmarine    | SAFM |                 |
| Sealand      | SEAU | SEJJ            |
| Sinokor      | SNKO | SKLU            |
| SM Lines     | SMLM |                 |
| Wan Hai      | WHLC | 22AA            |
| WEC Lines    | WECU |                 |
| Westwood     | WWSU |                 |
| Yang Ming    | YMLU |                 |
| ZIM          | ZIMU |                 |

---

## Container Types

| Code | ISO Code | Description          | Size | Category | TEU  |
| ---- | -------- | -------------------- | ---- | -------- | ---- |
| 20GP | 22G1     | 20' Standard         | 20ft | Dry      | 1.00 |
| 40GP | 42G1     | 40' Standard         | 40ft | Dry      | 2.00 |
| 40HC | 45G1     | 40' High Cube        | 40ft | Dry      | 2.00 |
| 20RF | 22R1     | 20' Reefer           | 20ft | Reefer   | 1.00 |
| 40RF | 42R1     | 40' Reefer           | 40ft | Reefer   | 2.00 |
| 40RH | 45R1     | 40' Reefer High Cube | 40ft | Reefer   | 2.00 |

---

## Notes

- SCAC codes follow the NMFTA standard (National Motor Freight Traffic Association)
- Alternate SCACs are secondary codes the same carrier uses (e.g. Maersk uses both `MAEU` and `MAEI`)
- If a carrier you work with is not listed, contact your Flete24 administrator

## Related Guides

- [Carrier Charge Aliases](charge-aliases.md)
- [Charge Master](charge-master.md)
- [Create a Rate Card](../rates/rates.md)
