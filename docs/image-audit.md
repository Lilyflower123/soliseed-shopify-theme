# Image Audit

## Executive Summary

The theme repository contains very few local image assets. The only local files in `assets/` that match the requested image formats are Instagram/UI assets and arrow SVGs. They are useful for UI and social display, but they are not enough to support the full Soliseed homepage visual system.

The current homepage Hero image is a Shopify admin media reference, not a repository file: `shopify://shop_images/1_83b91b63-5502-4aa1-9552-c4d3b43df58c.jpg` in `templates/index.json`. The header logo is also a Shopify media reference: `shopify://shop_images/logo.png` in `sections/header-group.json`.

Product cards and featured collection modules use Shopify product or collection media, especially `product.featured_media`, variant media, and `collection.featured_image`. That is suitable for Best Sellers if the Shopify product images are strong.

## Image Inventory Table

| File path / reference | File name | Format | File size | Dimensions | Currently referenced | Referenced by | Content judgment | Suggested use category | Suggested action |
|---|---|---|---|---|---|---|---|---|---|
| `assets/Instagram-glyph-gradient.png` | `Instagram-glyph-gradient.png` | png | 10,954 bytes | 256 x 256 | Yes | `snippets/showcase-item.liquid` | Instagram gradient glyph for showcase/social UI. | Icon / UI 可用 | 保留原用 |
| `assets/Instagram_logo_2016.svg` | `Instagram_logo_2016.svg` | svg | 4,334 bytes | 132.004 x 132 from SVG attributes | Yes | `snippets/showcase-item.liquid`, `sections/showcase.liquid` | Instagram logo mark. | Icon / UI 可用 | 保留原用 |
| `assets/arrow-left.svg` | `arrow-left.svg` | svg | 288 bytes | 24 x 24, viewBox 0 0 256 256 | Yes | `snippets/css-variables.liquid` | Theme carousel/navigation arrow. | Icon / UI 可用 | 保留原用 |
| `assets/arrow-right.svg` | `arrow-right.svg` | svg | 283 bytes | 24 x 24, viewBox 0 0 256 256 | Yes | `snippets/css-variables.liquid` | Theme carousel/navigation arrow. | Icon / UI 可用 | 保留原用 |
| `shopify://shop_images/1_83b91b63-5502-4aa1-9552-c4d3b43df58c.jpg` | `1_83b91b63-5502-4aa1-9552-c4d3b43df58c.jpg` | jpg | Not available locally | Not readable locally | Yes | `templates/index.json` | Current homepage Hero image in Shopify admin media. Content cannot be confirmed from repository alone. | Hero 可用 / 需要人工查看 | 仅作临时占位 |
| `shopify://shop_images/logo.png` | `logo.png` | png | Not available locally | Not readable locally | Yes | `sections/header-group.json` | Header logo from Shopify admin media. | Icon / UI 可用 | 保留原用 |

## Recommended Reuse Plan

| Homepage need | Best available current asset | Fit assessment | Recommendation |
|---|---|---|---|
| Hero: Every Spot Can Grow | `shopify://shop_images/1_83b91b63-5502-4aa1-9552-c4d3b43df58c.jpg` | Potentially usable, but content cannot be verified locally. | Use temporarily only after manual Shopify preview review. Replace if it does not show plants in a real placement. |
| Desk Plants | Shopify product/admin media | No confirmed repository asset. | Export or select a desk/clip-on scene. |
| Plant Shelves | Shopify product/admin media | No confirmed repository asset. | Export or select a plant rack or shelf scene. |
| Dark Corners | Shopify product/admin media | No confirmed repository asset. | Need a corner or larger plant support scene. |
| Kitchen Herbs | Herb kit product/admin media | Likely available only through Shopify product records. | Use if it shows kitchen, counter, or windowsill context. |
| Living Room Plant Corners | Shopify product/admin media | No confirmed repository asset. | Need a calm living room plant corner scene. |
| Greenhouse & Seedlings | Greenhouse string light product/admin media | Likely available only through Shopify product records. | Use if it shows seedlings, greenhouse, or wider coverage. |
| Shop by Setup cards | Product/collection featured media | Likely usable if images are lifestyle/setup focused. | Use product media temporarily; replace white-background images with scene images later. |
| Support / Setup Guide | None local | Weak visual support. | Use simple layout now; add instructional diagrams later. |

## Missing Image List

1. Hero lifestyle image showing plants in a real indoor spot with Soliseed light support.
2. Desk Plants scene.
3. Plant Shelves / plant rack scene.
4. Dark Corners scene.
5. Kitchen Herbs / herb kit in kitchen context.
6. Living Room Plant Corners scene.
7. Greenhouse & Seedlings scene.
8. Clip-on Grow Lights setup card image.
9. Pendant Grow Lights setup card image.
10. Herb Garden Kits setup card image.
11. Greenhouse String Lights setup card image.
12. Setup Guide support image or simple instructional visual.

## Priority New Image List

Highest priority:

1. Hero image for `Every Spot Can Grow.`
2. Plant Shelves image.
3. Desk Plants / clip-on image.
4. Kitchen Herbs image.
5. Greenhouse & Seedlings image.

Second priority:

1. Living Room Plant Corners image.
2. Dark Corners image.
3. Pendant Grow Lights image.
4. Setup Guide instructional image or diagram.

## Notes for Shopify Admin

- Review the current Hero media `1_83b91b63-5502-4aa1-9552-c4d3b43df58c.jpg` in Shopify admin.
- Export or screenshot strong product/scene images for Best Sellers, clip-on, pendant, herb kit, and greenhouse string light products.
- Check whether `compact-clip`, `the-pendant-collection`, `grow-kits-cabinets`, and `floor-flex-system` have strong collection images.
- If product photos are only white-background ecommerce images, keep them for Best Sellers but do not rely on them for Shop by Space cards.
- Prefer images that show the plant, location, and light form together.

## Final Assessment

Current repository assets are not enough to visually support the full upgraded homepage. The theme can technically launch using Shopify admin media and product images, but the Shop by Space story needs better lifestyle images.

Directly reusable: Instagram assets, arrow SVGs, and Shopify admin logo.

Potentially reusable: current Shopify Hero image, product featured media, and collection featured images after manual review.

Temporary placeholders: current Hero image until reviewed, and product-only ecommerce photos for space cards.

Recommended to reshoot or regenerate: Desk Plants, Plant Shelves, Dark Corners, Kitchen Herbs, Living Room Plant Corners, Greenhouse & Seedlings, and any Hero image that does not clearly show real plant placement with grow light support.