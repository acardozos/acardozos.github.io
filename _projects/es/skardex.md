---
title: Simple Kardex
ref: skardex
permalink: /proyectos/skardex/
area: software
status: active
year: 2026
order: 1
summary: Un kardex de inventario para un negocio familiar. Reemplaza una hoja de cálculo por un registro de entradas y salidas, con saldos calculados y alertas de stock bajo.
repo: https://github.com/acardozos/skardex
stack: [Python, FastAPI, Jinja2, PostgreSQL, SQLAlchemy, Alembic, uv]
---
## Por qué existe

Un negocio pequeño no necesita un ERP: necesita una lista confiable con usuarios. **Simple Kardex** parte de ese principio. Es más una lista con inicio de sesión que un sistema empresarial.

## Qué hace

- **Catálogo de artículos** con código, unidad de medida y stock mínimo.
- **Registro de movimientos** (entradas y salidas) con su motivo. El saldo se calcula siempre a partir del historial; nunca se guarda aparte.
- **Precios y pagos pendientes**: una venta nunca se bloquea por falta de precio, solo queda marcada hasta corregirla.
- **Panel** con contadores y alerta visual para artículos bajo el mínimo.
- **Dos roles**: administrador y operario. Sin registro público: el administrador crea las cuentas.
- Funciona en teléfono, tableta y escritorio, con tema claro y oscuro y colores de estado que cumplen WCAG AA.

## Lo que aprendí

Que la simplicidad también se diseña: decidir qué *no* hacer fue tan importante como lo que sí se hizo.
