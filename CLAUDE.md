# CLAUDE.md — Pizza Planet

Menú digital para Pizza Planet, cadena de pizzas artesanales con 5 sedes en Quito, Ecuador.

## Tecnología

Mismo stack que deli-express: HTML/CSS/JS vanilla, sin build. Un solo `index.html` + `config.json` + `productos.json`.

## Estructura

```
index.html        # UI completa copiada de deli-express (template base)
config.json       # Config de la tienda + info de sedes
productos.json    # Catálogo completo (21 productos)
```

## Datos del cliente

- **WhatsApp principal**: +593969064106
- **Sedes**: Católica, Valle de los Chillos, Real Audiencia, UTE–Rumipamba, La Michelena
- **Fuente original**: https://qr.food724.com/pizzaplanet/ (WooCommerce + Elementor)

## Catálogo (21 productos)

### Categorías
| Slug | Nombre |
|---|---|
| pizzas-familiares | 🍕 Pizzas Familiares (35cm, 12 porciones) |
| pizzas-medianas | 🍕 Pizzas Medianas (30cm, 8 porciones) |
| especialidades | ⭐ Especialidades |
| combos-individuales | 🍱 Combos Individuales |
| ensaladas | 🥗 Ensaladas |
| porciones | 🍟 Porciones |
| bebidas | 🥤 Bebidas |

### Sabores de pizza (disponibles en familiares y medianas)
**Sin cargo extra:** Americana, Andina, Argentina, Francesa, Italiana, New York, Portuguesa, SuperPlanet
**+$1:** Hawaiana, Texana, Española, Mexicana
**+$1.50:** Dubai

### Sabores pizza personal (20cm)
Similar a familiares/medianas pero sin algunas opciones premium. Argentina y Dubai: +$0.50.

### Precios clave
- Pizza Familiar (35cm): $9.00 | +Bebida: $9.99
- 2 Familiares: $17.00 | +Bebida: $18.00
- 3×2 Familiares: $26.99 (Envío Gratis*)
- Festín Familiar (2 pizzas+2 ensaladas+12 panes+2 bebidas): $23.99
- Pizza Mediana (30cm): $7.00 | +Bebida: $8.50
- 2 Medianas +Bebida: $15.99 | 3×2 Medianas: $19.99
- Combo Mediano (pizza+panes+ensalada+bebida): $13.99
- Pizza Personal (20cm): $3.99
- Lasañas: $5.99 | Combo Lasaña: $7.99
- Combo Lunch: $4.99

## Deploy

```bash
git add .
git commit -m "descripción"
git push
```

Cloudflare Pages despliega automáticamente en push a `main`.
