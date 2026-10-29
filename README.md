# Gristcity

A custom widget for [Grist](https://www.getgrist.com) that draws a table as a city in isometric 3D.

Each row becomes a building that grows as it moves through its stages: reserved plot, construction site, finished building, skyscraper... Districts group the buildings by a column of your choice. A weather layer flags what needs watching (cloud) and what needs attention now (storm).

Everything is configured inside the widget, no code required.

> **Note:** the widget interface is in French.

## Six worlds

| World | Each row becomes | Great for |
|---|---|---|
| 🏙️ City | a building | projects, requests, case files |
| 🌳 Garden | a plant | people's journeys, training paths |
| 🚗 Garage | a vehicle | a vehicle fleet, equipment |
| ✈️ Airport | a plane | missions, business trips |
| 🚀 Space base | a rocket | ideas, innovation |
| ⚓ Harbour | a ship | programmes, partnerships |

## Installation

1. In your Grist document, add a **Custom** widget.
2. Choose **Custom URL** and paste:
   `https://cezionlyone.github.io/grist-widgets/`
3. In the right panel, under **Access**, select **Full document access**.
4. Follow the setup wizard: pick a world, then start from a ready-made template or connect the widget to one of your tables.

## Features

- **Setup wizard** in 8 steps, with a live preview that builds up as you answer.
- **Ready-made templates**: project portfolio, team workload, request tracking, application portfolio, org chart, vehicle fleet... The widget creates the tables, with sample rows if you want them.
- **Several cities per document**, shown as tabs.
- **Editable record card** for each building, attachments included.
- **Move mode**: drag a building to another district to update the matching column.
- **Filters, search and list view**, an accessible alternative to the map.

## What the widget writes to your document

- A technical table, `BIBLIOTHEQUE_VILLE`, created with the first city: one settings row per city.
- In the table being drawn: only the values edited in a record card, the buildings you add and the moves you make. Its structure is never changed.
- The tables of a template, only if you choose one.

## Permissions

The widget follows each person's rights in the document:

- **Viewers**: browse, search, filter, read record cards.
- **Editors**: also edit record cards, add buildings and move them.
- **Settings**: can be restricted to owners with an access rule. The widget shows how to set it up.

## Dependencies

- [DSFR](https://www.systeme-de-design.gouv.fr) v1.13.1 (French government design system)
- Grist widget API (`grist-plugin-api.js`)
- [pdf.js](https://mozilla.github.io/pdf.js/) v6.2.108, loaded only to preview attached PDFs, with its checksum verified

> **Good to know:** the DSFR terms of use restrict it to French government websites. Check that they cover your use before deploying this widget.

## License

[MIT](../LICENSE): you are free to use, modify and redistribute this widget, as long as you keep the author credit.

---

made **X** Cé
