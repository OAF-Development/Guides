# PhotoShop Surface Mask

This guide assumes that you have completed the initial steps to start your map project, obtained your satellite map, and have a basic understanding of the purpose of your surface mask.

I will be using a `gtt_satmap.bmp` exported with **Game Terrain Tools** plugin on **QGIS**.


## Requirements
- Adobe PhotoShop
- Satellite Map
- RGB references from your `layers.cfg` file
- This [Reference Image](images\LayerLegendComplete_v2.png) of terrain textures in-game may also help you along the way.
  - Credit to BergTheBeard in [DZ Academy Discord](https://discord.com/channels/728090560304382002/761156911398780958/1118673530394001528)




## Getting Started

 Open your sat map image in PhotoShop.

![Step One](./images/Step1.png)
*Open your satellite map image in PhotoShop*

---
 In your toolbar: `Select` > `Color Range`

![Step Two](./images/Step2.png)
*Go to `Select` > `Color Range` in the toolbar*

---
- You'll be presented with the **Eyedropper Tool** as well as the **Color Range** modal.


![Step Three](./images/Step3.png)
*Adjust the `Fuzziness` slider and select a sample area.*

---
For this guide, I will select the dense forestry area to isolate the majority of trees into their own layer.


![Step Four](./images/Step4.png)
*Dense forestry area selected with Fuzziness set to `60`*

---
- `CTRL+C` to Copy the Selection.

- `CTRL+V` to Paste it into a new Layer.

![Step Five](./images/Step5.png)
*Hide your Alpha layer, select your new one.*

- Select > **Color Range** again, grab a sample from the new pasted layer, click `OK` to regain the selection.

---
With the area selected, open your **Color Picker** in the top right by double clicking the the two boxes on the side of it.

![Step Six](./images/Step6.png)
*Enter your desired terrain RGB values in the highlighted areas shown above.* 

**Remember**:  [Reference Image](images\LayerLegendComplete_v2.png) will assist in this, but ensure you're using the values defined in your `layers.cfg` as they may vary.

---
- Open the **Brush Tool** with `B` - may help to adjust your size to the maximum.
- Start painting away. Only the selection will be applied.
![Step Seven](./images/Step7.png)
![Rename your layers as you go to the terrains to help you easily identfy them.](./images/rename_layers.png)
*Tip: Rename your layers as the terrain textures as you go to help you easily identfy them.*

---

## Repeat the Process

You'll want to repeat these steps for each area you want to define within your mask.


![Step 8](./images/Rinse_Repeat.png)
*Doing the same for the Snow covered areas, so on and so forth.*


---
**Tips:** Allow yourself up to 6 types of materials while doing this. 

- *You can further refine & tune in areas where you are certain that the **limit of 6 materials per cell** is not going to be exceeded.*

- Depending on the complexity of your map, you may want to limit yourself to 4-5 layers of terrain colors.

- *This will allow you to add a layer for your Road shapes if you so choose to do so at the end (which I will cover later), as well as consideration of leaving yourself an available layer for a background material to be placed in (i.e. `grass`, etc.)*

- You can `Quick Export as PNG` by right-clicking a layer once it's complete. Save these to your `source` folder for safe keeping just in case you need to revert or make some adjustments going forward.
---


## Merging Down Layers
- Once you have completed the process a few times, the results should be something similar.

![Step 9](./images/multiple_layers.png)
---
- Arrange the order of your layers to work as you desire, this will help to cover any areas that you want to be more prominent over any overlapping selections that may have been painted during the process.

![Step 10](./images/layers_ordered.png)

- Once you're happy with the arrangement, you can right-click & `Merge Down` each layer starting from the top of the list and working your way down.
    - *Do **NOT** merge them into your Alpha satmap image.*

- Go ahead & `Quick Export as PNG` this merged version to your source for safe keeping as well.
---

## Road Shapes & Background Material

**WIP** -- Will continue this section later.