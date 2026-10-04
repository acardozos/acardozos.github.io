---
title: Simple Kardex
ref: skardex
permalink: /en/projects/skardex/
area: software
status: active
year: 2026
order: 1
summary: An inventory ledger for a family business. It replaces a spreadsheet with a log of entries and exits, calculated balances and low-stock alerts.
repo: https://github.com/acardozos/skardex
stack: [Python, FastAPI, Jinja2, PostgreSQL, SQLAlchemy, Alembic, uv]
---
## Why it exists

A small business doesn't need an ERP: it needs a reliable list with users. **Simple Kardex** starts from that idea. It is more a list with a login than an enterprise system.

## What it does

- **Item catalogue** with code, unit of measure and minimum stock.
- **Movement log** (entries and exits), each with a reason. The balance is always calculated from history; it is never stored separately.
- **Prices and pending payments**: a sale is never blocked for lack of a price, it is just flagged until fixed.
- **Dashboard** with counters and a visual alert for items below their minimum.
- **Two roles**: admin and operator. No public sign-up: the admin creates the accounts.
- Works on phone, tablet and desktop, with light and dark themes and status colours that meet WCAG AA.

## What I learned

That simplicity is designed too: deciding what *not* to build mattered as much as what got built.
