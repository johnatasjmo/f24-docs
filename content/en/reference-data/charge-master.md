---
title: Charge Master
weight: 2
---


**For:** All users | **Updated:** 2026-03-31

---

## What is the Charge Master?

The global list of standardized freight charge codes. Managed by Flete24 — visible to all tenants, read-only.

Local charges and rate surcharges reference these codes. The AI extraction pipeline uses charge codes to normalize carrier-specific charge names into standard codes. See [Carrier Charge Aliases](charge-aliases.md) for the alias mappings.

---

## Freight

Base cost of moving cargo from origin to destination.

| Code | Name                | Description                                                   | Basis         |
| ---- | ------------------- | ------------------------------------------------------------- | ------------- |
| OFR  | Ocean Freight       | Base ocean freight rate for FCL shipments                     | Per container |
| OFR  | Ocean Freight (W/M) | Base ocean freight rate for LCL shipments (weight or measure) | Per W/M       |
| AFR  | Air Freight         | Base air freight rate                                         | Per kg        |
| IFR  | Inland Freight      | Base inland/intermodal freight rate                           | Flat          |

---

## Surcharges

Carrier, market, or regulatory adjustments on top of base freight.

| Code | Name                          | Description                                                    | Basis         |
| ---- | ----------------------------- | -------------------------------------------------------------- | ------------- |
| BAF  | Bunker Adjustment Factor      | Fuel surcharge compensating for oil price fluctuations         | Per container |
| LSS  | Low Sulphur Surcharge         | IMO 2020 low-sulphur fuel compliance surcharge                 | Per container |
| CAF  | Currency Adjustment Factor    | Surcharge compensating for currency exchange rate fluctuations | Percentage    |
| PSS  | Peak Season Surcharge         | Applied during high-demand shipping periods                    | Per container |
| GRI  | General Rate Increase         | Periodic rate increase applied across trade lanes              | Per container |
| ERR  | Emergency Rate Restoration    | Emergency rate increase to restore carrier profitability       | Per container |
| WAR  | War Risk Surcharge            | Applied when routing through conflict zones                    | Per container |
| PCS  | Port Congestion Surcharge     | Applied when origin or destination port is congested           | Per container |
| ISPS | ISPS Security Surcharge       | International Ship and Port Facility Security Code compliance  | Per container |
| ECA  | Emission Control Area         | Surcharge for routing through emission control areas           | Per container |
| EIS  | Equipment Imbalance Surcharge | Compensates for repositioning empty containers                 | Per container |
| CSF  | Carrier Security Fee          | Security surcharge for high-risk routing areas                 | Per container |
| FAF  | Fuel Adjustment Factor        | Alternative fuel surcharge (Japan/Oceania routes)              | Per container |
| PAN  | Panama Canal Surcharge        | Transit fee for Panama Canal passage                           | Per container |
| SUE  | Suez Canal Surcharge          | Transit fee for Suez Canal passage                             | Per container |
| WHS  | Winter Surcharge              | Applied during winter months for weather-affected routes       | Per container |
| CIC  | Container Imbalance Charge    | Charge for container repositioning on imbalanced trade lanes   | Per container |
| EBS  | Emergency Bunker Surcharge    | Emergency fuel surcharge for unexpected price spikes           | Per container |
| HLA  | Haulage Adjustment            | Inland transport cost adjustment surcharge                     | Per container |
| OWS  | Overweight Surcharge          | Surcharge for containers exceeding weight limits               | Per container |
| DGS  | Dangerous Goods Surcharge     | Surcharge for shipping hazardous materials (IMO classes)       | Per container |
| RFS  | Reefer Surcharge              | Additional charge for refrigerated containers                  | Per container |
| OOG  | Out of Gauge                  | Surcharge for oversized cargo requiring special equipment      | Per container |
| FLR  | Flat Rack Surcharge           | Surcharge for flat rack container usage                        | Per container |
| OPT  | Open Top Surcharge            | Surcharge for open top container usage                         | Per container |

---

## Accessorial — Origin (POL)

Operational handling charges at the port of loading.

| Code | Name                           | Description                                          | Basis         |
| ---- | ------------------------------ | ---------------------------------------------------- | ------------- |
| OTHC | Origin Terminal Handling       | Terminal handling charge at origin port              | Per container |
| OTHC | Origin Terminal Handling (W/M) | Terminal handling charge at origin for LCL           | Per W/M       |
| ORC  | Origin Receiving Charge        | Charge for receiving cargo at origin terminal        | Per container |
| SEAL | Seal Fee                       | Container seal charge at origin                      | Per container |
| VGM  | Verified Gross Mass            | SOLAS VGM weighing and certification                 | Per container |
| LFT  | Lift On/Off Origin             | Crane lift charge at origin terminal                 | Per container |
| WFG  | Wharfage Origin                | Port authority charge for use of wharf at origin     | Per container |
| GAT  | Gate Fee Origin                | Container gate-in/gate-out charge at origin terminal | Per container |
| XRY  | X-Ray Inspection               | Container scanning/inspection fee at origin          | Per container |
| EXP  | Export Service Fee             | Export clearance and handling at origin              | Per B/L       |
| STF  | Stuffing/Loading               | Container stuffing/loading service at origin CFS     | Per CBM       |

---

## Accessorial — Destination (POD)

Operational handling charges at the port of discharge.

| Code | Name                                | Description                                               | Basis         |
| ---- | ----------------------------------- | --------------------------------------------------------- | ------------- |
| DTHC | Destination Terminal Handling       | Terminal handling charge at destination port              | Per container |
| DTHC | Destination Terminal Handling (W/M) | Terminal handling charge at destination for LCL           | Per W/M       |
| LFD  | Lift On/Off Destination             | Crane lift charge at destination terminal                 | Per container |
| WFD  | Wharfage Destination                | Port authority charge for use of wharf at destination     | Per container |
| GAD  | Gate Fee Destination                | Container gate-in/gate-out charge at destination terminal | Per container |
| IMP  | Import Service Fee                  | Import clearance and handling at destination              | Per B/L       |
| DOF  | Delivery Order Fee                  | Fee for issuing delivery order at destination             | Per B/L       |
| UST  | Unstuffing/Unloading                | Container unstuffing service at destination CFS           | Per CBM       |
| CFS  | CFS Handling                        | Container Freight Station handling charge for LCL         | Per CBM       |

---

## Accessorial — Transport Legs

| Code | Name                  | Description                                       | Basis         |
| ---- | --------------------- | ------------------------------------------------- | ------------- |
| IHE  | Inland Haulage Export | Trucking from shipper location to port of loading | Per container |
| IHI  | Inland Haulage Import | Trucking from port of discharge to consignee      | Per container |
| PIK  | Pickup/Collection     | Cargo pickup or collection service                | Per container |
| DLV  | Delivery              | Final delivery to consignee premises              | Per container |

---

## Accessorial — Demurrage & Detention

| Code | Name                  | Description                                              | Basis         |
| ---- | --------------------- | -------------------------------------------------------- | ------------- |
| DEMO | Demurrage Origin      | Container held beyond free time at origin port           | Per container |
| DEMD | Demurrage Destination | Container held beyond free time at destination port      | Per container |
| DETO | Detention Origin      | Container held beyond free time outside origin port      | Per container |
| DETD | Detention Destination | Container held beyond free time outside destination port | Per container |
| STO  | Storage               | Container or cargo storage at terminal                   | Per container |
| PLT  | Palletization         | Cargo palletization service                              | Per CBM       |

---

## Documentation

| Code | Name                      | Description                                      | Basis   |
| ---- | ------------------------- | ------------------------------------------------ | ------- |
| BLF  | Bill of Lading Fee        | Processing and issuance of B/L document          | Per B/L |
| TLX  | Telex Release             | Electronic release of B/L                        | Per B/L |
| SWB  | Sea Waybill Fee           | Issuance of sea waybill (non-negotiable B/L)     | Per B/L |
| AMS  | AMS Filing                | U.S. Automated Manifest System filing fee        | Per B/L |
| ISF  | Importer Security Filing  | U.S. ISF 10+2 filing fee                         | Per B/L |
| ENS  | Entry Summary Declaration | EU Import Control System filing fee              | Per B/L |
| DOC  | Documentation Fee         | General documentation processing fee             | Per B/L |
| MAN  | Manifest Fee              | Cargo manifest preparation and filing            | Per B/L |
| AFI  | ACI Filing                | Canada Advance Commercial Information filing fee | Per B/L |
| ADM  | Administrative Fee        | General administrative/handling fee              | Flat    |

---

## Value-Added Services (VAS)

| Code | Name                      | Description                         | Basis         |
| ---- | ------------------------- | ----------------------------------- | ------------- |
| INS  | Cargo Insurance           | All-risk cargo insurance premium    | Percentage    |
| FUM  | Fumigation                | Cargo fumigation treatment fee      | Per container |
| CHB  | Customs Brokerage         | Customs clearance service fee       | Per B/L       |
| PHY  | Phytosanitary Certificate | Plant health inspection certificate | Per B/L       |
| COD  | Certificate of Origin     | Issuance of certificate of origin   | Per B/L       |
| CDD  | Customs Declaration       | Customs declaration processing fee  | Per B/L       |

---

## Related Guides

- [Carrier Charge Aliases](charge-aliases.md)
- [Carriers](carriers.md)
- [Local Charges](../local-charges/local-charges.md)
