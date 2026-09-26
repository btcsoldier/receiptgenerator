# Receipt Studio — Vinted Valley

A single self-contained HTML file for designing and printing custom receipt layouts. No install, no server — just open `vinted_valley_receipt_studio.html` in a browser.

## Getting started

1. Open the file in any modern browser (Chrome, Edge, Firefox, Safari).
2. Start from the **Retail receipt** or **Simple** template (top-left "Templates" panel), or click **New** to reset.
3. Add elements from the **Add elements** panel, click one on the canvas to select it, and edit it in the **Selected element** panel on the right.
4. When it looks right, hit **Print / PDF** to print or save as PDF.

## Elements

| Element | What it's for |
|---|---|
| Text | Any free line of text — headers, addresses, notes |
| Image | A logo or artwork embedded in the printed receipt |
| Separator | A dashed/character line that automatically fills the receipt width |
| Spacer | Blank vertical space |
| Item | A product line with optional SKU, description, qty, price, tax code |
| Total | A label + amount row (subtotal, tax, total, etc.) |
| Barcode | A generated barcode graphic |
| QR code | A QR code linking to a URL or containing text |

Every text-based element (Text, Separator, Item, Total) has a **Left offset / Right offset** field so you can nudge it horizontally to match spacing on a real receipt. Barcode and QR elements have a left/center/right alignment option.

## Reference image (trace a real receipt)

Click **Reference image** in the top bar or the sidebar panel to upload a photo of an actual receipt. It appears as a faint, semi-transparent guide layered over your canvas so you can match spacing and structure while you rebuild it with real elements.

- Adjust its **opacity** with the slider
- **Show/hide** it at any time
- **Remove** it when you're done

The reference image is a guide only — it's never included in the printed receipt, the exported HTML, or a saved project file.

## Organizing elements

- **Layers panel** (bottom-right) lists every element top to bottom. Click one to select it.
- Use the ▲ / ▼ buttons to reorder, the copy icon to **duplicate**, or the trash icon to delete.
- The **Selected element** panel also has Duplicate / Copy / Delete buttons at the top.

### Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl/⌘ + S` | Save project as JSON |
| `Ctrl/⌘ + D` | Duplicate selected element |
| `Ctrl/⌘ + C` | Copy selected element |
| `Ctrl/⌘ + V` | Paste copied element after the current selection |
| `Delete` / `Backspace` | Delete selected element |

Shortcuts are disabled while you're typing in a text field, so Backspace still works normally for editing text.

## Receipt size & fonts

- Set width in mm or px, and choose auto height (fits content) or a fixed height.
- Adjust horizontal padding.
- Pick a default monospace/receipt font, or add any Google Font by name and apply it per-element.

## Saving & exporting

- **Save** — downloads the current design as a `.json` project file.
- **Load** — re-opens a previously saved `.json` project.
- **Export HTML** — downloads a standalone, printable HTML file of just the receipt.
- **Print / PDF** — opens the browser print dialog (use "Save as PDF" as the destination for a PDF file).

## Notes

- Everything runs client-side in your browser; no data is uploaded anywhere.
- Uploaded images (logos, reference photos) are embedded as base64 data, so saved project files can get large if you use big images.
