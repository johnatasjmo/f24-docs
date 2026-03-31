---
title: Carrier Charge Aliases
weight: 3
---


**For:** All users | **Updated:** 2026-03-31

---

## What are Charge Aliases?

Different shipping lines and tariff documents use different names for the same charge. The charge aliases table maps those carrier-specific names to the standard charge code in the [Charge Master](charge-master.md).

**Why it matters:** When the AI extracts rates from uploaded documents (PDF, Excel, WhatsApp), it uses aliases to normalize what the carrier wrote (e.g. `"THC ORIGIN"`) into the standard code (`OTHC`). Better alias coverage = higher extraction accuracy.

Aliases are managed by Flete24 administrators. If the AI is consistently misidentifying a charge from a specific carrier, report it so an alias can be added.

---

## Aliases by Charge

### Terminal Handling Charges

| Alias                                | Maps To                              |
| ------------------------------------ | ------------------------------------ |
| THC ORIGIN                           | Origin Terminal Handling (OTHC)      |
| THC O                                | Origin Terminal Handling (OTHC)      |
| OTHC                                 | Origin Terminal Handling (OTHC)      |
| TERMINAL HANDLING ORIGIN             | Origin Terminal Handling (OTHC)      |
| TERMINAL HANDLING CHARGE ORIGIN      | Origin Terminal Handling (OTHC)      |
| THC DEST                             | Destination Terminal Handling (DTHC) |
| THC DESTINATION                      | Destination Terminal Handling (DTHC) |
| THC D                                | Destination Terminal Handling (DTHC) |
| DTHC                                 | Destination Terminal Handling (DTHC) |
| TERMINAL HANDLING DESTINATION        | Destination Terminal Handling (DTHC) |
| TERMINAL HANDLING CHARGE DESTINATION | Destination Terminal Handling (DTHC) |

### Ocean Freight

| Alias        | Maps To       |
| ------------ | ------------- |
| O/F          | Ocean Freight |
| OFR          | Ocean Freight |
| OCEAN FRT    | Ocean Freight |
| FREIGHT      | Ocean Freight |
| BASE FREIGHT | Ocean Freight |

### Documentation

| Alias           | Maps To            |
| --------------- | ------------------ |
| DOC FEE         | Documentation Fee  |
| DOCUMENTATION   | Documentation Fee  |
| DOC             | Documentation Fee  |
| BL FEE          | Bill of Lading Fee |
| B/L FEE         | Bill of Lading Fee |
| MBL RELEASE     | MBL Release Fee    |
| MBL RELEASE FEE | MBL Release Fee    |
| MBL FEE         | MBL Release Fee    |

### Container Handling

| Alias                | Maps To                 |
| -------------------- | ----------------------- |
| SEAL                 | Seal Fee                |
| SEAL CHARGE          | Seal Fee                |
| VGM                  | Verified Gross Mass     |
| VGM FEE              | Verified Gross Mass     |
| VGM CHARGE           | Verified Gross Mass     |
| LIFT ON              | Lift On/Off Origin      |
| LIFT OFF             | Lift On/Off Destination |
| GATE IN              | Gate Fee Origin         |
| GATE OUT             | Gate Fee Destination    |
| WHARFAGE ORIGIN      | Wharfage Origin         |
| WFG                  | Wharfage Origin         |
| WHARFAGE DEST        | Wharfage Destination    |
| WHARFAGE DESTINATION | Wharfage Destination    |
| WFD                  | Wharfage Destination    |

### Surcharges

| Alias            | Maps To                    |
| ---------------- | -------------------------- |
| BAF              | Bunker Adjustment Factor   |
| BUNKER           | Bunker Adjustment Factor   |
| BUNKER SURCHARGE | Bunker Adjustment Factor   |
| EBS              | Emergency Bunker Surcharge |
| GRI              | General Rate Increase      |
| LSS              | Low Sulphur Surcharge      |
| LOW SULPHUR      | Low Sulphur Surcharge      |
| PSS              | Peak Season Surcharge      |
| PEAK SEASON      | Peak Season Surcharge      |
| WAR RISK         | War Risk Surcharge         |
| ISPS             | ISPS Security Surcharge    |
| OWS              | Overweight Surcharge       |
| OVERWEIGHT       | Overweight Surcharge       |
| PCS              | Panama Canal Surcharge     |
| PANAMA CANAL     | Panama Canal Surcharge     |

### Inland Transport

| Alias          | Maps To               |
| -------------- | --------------------- |
| IHI            | Inland Haulage Import |
| IHE            | Inland Haulage Export |
| INLAND HAULAGE | Inland Haulage Import |
| TRUCKING       | Inland Haulage Import |

### Other

| Alias        | Maps To      |
| ------------ | ------------ |
| PROFIT SHARE | Profit Share |
| PSH          | Profit Share |

---

## Carrier Name Aliases

The AI also uses carrier name aliases to match shipping line names in documents to the standard carrier record.

| Alias          | Maps To     |
| -------------- | ----------- |
| YML            | Yang Ming   |
| YM             | Yang Ming   |
| YANG MING LINE | Yang Ming   |
| MSK            | Maersk      |
| MSK ONLINE     | Maersk      |
| MSK NAC        | Maersk      |
| MAERSK LINE    | Maersk      |
| COSCO SHIPPING | COSCO       |
| OOCL LINE      | OOCL        |
| ONE LINE       | ONE         |
| CMA            | CMA CGM     |
| EVERGREEN LINE | Evergreen   |
| EMC            | Evergreen   |
| HPL            | Hapag-Lloyd |
| HAPAG LLOYD    | Hapag-Lloyd |
| HAPAG          | Hapag-Lloyd |
| ZIM LINE       | ZIM         |
| PIL LINE       | PIL         |
| HMM LINE       | HMM         |
| HYUNDAI        | HMM         |

---

## Related Guides

- [Charge Master](charge-master.md)
- [Carriers](carriers.md)
