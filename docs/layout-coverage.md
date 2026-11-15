# Reference layout coverage

The 22-page source contains repeated section dividers and multiple content compositions. The public example contains 18 slides and uses each of the 18 layouts once.

| Reference page(s) | Composition | Published layout / component |
|---|---|---|
| 1 | Cover and diagonal corner squares | cover, CmrDecor |
| 2 | Bilingual agenda | contents |
| 3, 11, 15, 20 | Numbered bilingual section divider | section |
| 4 | Explanatory panels beside an image | image-right, two-cols |
| 5 | Three numbered rounded rows | process with CmrSteps |
| 6 | Centered technical figure with explanation | default or image-right |
| 7 | Technical figure with a side callout | image-left |
| 8 | Central theme and four branches | radial with CmrRadial |
| 9 | Two charts and right-hand notes | chart-notes with CmrBars |
| 10 | Evidence / table image with metrics | image-left with metrics content |
| 12 | System image and blue explanation area | image-left with a callout |
| 13 | Five module groups | modules with CmrModules |
| 14 | Four software groups with central marks | gallery |
| 16 | Vertical workflow and explanation | process with CmrFlow |
| 17 | U-shaped workflow and side callout | flow-snake with CmrFlow |
| 18 | Icon steps and contrasting right panel | icon-steps with CmrIconSteps |
| 19 | Four charts with shared explanation | chart-grid with caption |
| 21 | Summary list and contrasting side panel | summary |
| 22 | Closing | end |

Additional `default`, `compare`, and `two-cols` compositions support general technical writing. The generic starter demonstrates CmrSteps, while the 18-page company example uses CmrFlow on its process page. Native Markdown tables may be placed in a column; source tables were images and are not silently converted into invented data.

“Coverage” means reusable composition and slots, not pixel-for-pixel reproduction, identical custom outline geometry, or exact PowerPoint animation timing. Users supply their own figures and data. NVIDIA's example uses sourced historical revenue figures rather than invented CPU benchmarks.
