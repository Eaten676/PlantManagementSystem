# DRI Plant Management System

Records every vehicle entering and leaving a DRI (sponge iron) plant, weighbridge weighments, raw material consumption, finished goods production and the resulting stock, with a record of who entered each item and when.

## What's here

| Path | What it is |
| --- | --- |
| `demo/index.html` | Phase 1 clickable demo with sample data. One self-contained file: open it in any browser, no server needed. |

The demo saves changes in the browser only. **Reset demo data** on the sign-in screen starts it fresh. All plant names, parties, vehicles and figures are sample data.

## Phase 1 scope

- Gate inward and outward entries with vehicle photos, a block on vehicles already inside, and gate passes
- Weighbridge slips linked to gate entries, with net weight worked out automatically and an optional rule that a vehicle can't leave without a slip
- Shift-wise and kiln-wise consumption and production
- Live stock (opening + in − out), stock adjustments approved by a manager, negative stock shown in red, low-stock alerts
- Alerts when the weighbridge net differs from the bill tonnage by more than a set percentage
- Reports: gate register, vehicles inside, bill vs weighbridge by party, consumption by kiln, production by kiln and shift, stock statement, DRI performance (coal and ore per tonne, yield), with Excel export
- Five roles: security guard, weighbridge operator, stores / production, manager, admin
- Master lists, user management, settings, audit log
- Offline entry, installable on Android phones, English and Hindi

## Phase 2 (quoted separately)

- Automatic weight capture from the weighbridge indicator
- OTP login

## Planned stack for the production build

React web app (installable on phones), Node.js API, PostgreSQL database, on one cloud server in the plant's own account.
