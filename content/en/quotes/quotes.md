---
title: Quotes
weight: 1
---


**For:** Agent | **Updated:** 2026-03-31

---

## What is a Quote?

A quote is the commercial document you send to a BCO. It is built from rate cards in your rate library and includes ocean freight, local charges, markup, and validity terms.

**Quote vs Rate Card:** A rate card is raw internal pricing. A quote is the client-facing offer — rate cards plus markup, local charges, and terms.

---

## Quote Lifecycle

```
Draft → Review → Final → Published (coming soon)
```

| Status    | Editable | Visible to BCO | Use when                               |
| --------- | -------- | -------------- | -------------------------------------- |
| Draft     | Yes      | No             | Building or adjusting                  |
| Review    | No       | No             | Internal approval                      |
| Final     | No       | No             | Ready to send — export PDF/Excel       |
| Published | No       | Yes            | Delivered via platform _(coming soon)_ |

To make changes to a Final quote, create a **revision** — the original is preserved.

---

## Create a Quote

1. Go to **Quotes → New Quote**
2. Select the **client** (BCO company) and optionally a contact
3. Click **Add Lane** — enter Origin (POL) and Destination (POD) as UN/LOCODE
4. Select matching **rate cards** from your library. Per rate you can:
   - Apply a markup (fixed or percentage)
   - Adjust validity dates
   - Add or remove container types
5. Click **Add Local Charges** to attach port charges to the lane (optional)
6. Repeat steps 3–5 for additional lanes (multi-lane quotes)
7. Add **notes** — transit times, conditions, exclusions
8. Save as **Draft**, move to **Review**, or mark as **Final**

---

## Export a Quote

A quote must be in **Final** status to export.

- **PDF** — click **Export → PDF**. Includes all lanes, charges, and terms formatted for client delivery.
- **Excel** — click **Export → Excel**. One sheet per lane, full charge breakdown.

---

## Common Issues

| Problem                       | Solution                                                       |
| ----------------------------- | -------------------------------------------------------------- |
| No rate cards found for route | Create or import a rate card for that origin/destination first |
| Client not in dropdown        | Add the BCO company to your directory                          |
| Export button greyed out      | Quote must be in Final status                                  |
| Need to edit a Final quote    | Create a new revision — do not try to edit the Final           |
