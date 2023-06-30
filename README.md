# FancyWarpPackTemplate
Resource pack template for my Fancy Warp Menu mod

-----

# How to Create Your Own Pack
1. Create a new repository using the button above and checkout to your IDE. Alternatively, you can download this template.
2. Edit the options in [islands.json](Pack/assets/fancywarpmenu/data/islands.json) to your liking using the explanation of options below.
    ```json5
    {
      // Add your islands in this list
      "islandList": [
        {
          // Name label to be shown below the island
          "name": "Hub",
          // Path to the island's texture (relative to the folder pack.mcmeta is in
          "texturePath": "textures/gui/islands/The Hub.png",
          // Grid point to draw the left side of the island at (0-32)
          // 0 is screen left edge, 32 is screen right edge
          "gridX": 10,
          // Grid point to draw the top of the island at (0-18)
          // 0 is screen top edge, 18 is screen bottom edge
          "gridY": 6,
          // Island texture width as a percentage of screen width, expressed as a decimal
          // 0.3 means 30% of screen width and 1 means 100% for example
          "widthPercentage": 0.3,
          // Island texture height as a percentage of island texture width, expressed as a decimal
          // Calculated by dividing island texture height in pixels by island texture width in pixels 
          "heightPercentage": 0.5121412803532,
          // Horizontal texture offset (u)
          // Number of pixels to move to the right before reaching the start of the texture
          "textureXPosition": 0,
          // Vertical texture offset (v)
          // Number of pixels to move down before reaching the start of the texture
          "textureYPosition": 60,
          // Add your warps in this list
          "warpList": [
            {
              // Name label to be shown below the warp
              "displayName": "Spawn",
              // Name of the warp as used in the /warp command
              // The mod will run "/warp {commandName}", or "/warp hub" in this case
              "commandName": "hub",
              // Grid point to draw the left side of the warp at relative to the island
              // The island is divided into 40 grid lines where 0 is the island's left edge and 40 is the right edge
              "gridX": 29,
              // Grid point to draw the top of the warp at, also 0-40
              "gridY": 6
            }
          ]
        }
      ],
      // Warp messages Hypixel sends in chat to indicate warp success/failure
      // You shouldn't have to change these
      "warpMessages": {
        "warpSuccessMessages": [
          "Warping..."
        ],
        "warpFailMessages": {
          "Unknown destination! Check the Fast Travel menu to view options!": "fancywarpmenu.errors.unknownDestination",
          "You haven't unlocked this fast travel destination!": "fancywarpmenu.errors.notUnlocked",
          "Couldn't warp you! Try again later. (NO_DESTINATION_FOUND)": "fancywarpmenu.errors.noDestination",
          "You need to have visited this island at least once before fast traveling to it!": "fancywarpmenu.errors.notVisited"
        }
      },
      // Details of the texture to use for the warp buttons
      "warpIcon": {
        // Path to the warp button texture (relative to the folder pack.mcmeta is in)
        // Make sure the texture is not offset from image top and image left, no u/v options are configurable here
        "texturePath": "textures/gui/Portal.png",
        // Warp button texture width as a percentage of screen width, expressed as a decimal
        "widthPercentage": 0.02,
        // Warp button texture height as a percentage of warp button texture width, expressed as a decimal
        // Calculated by dividing texture height in pixels by texture width in pixels
        "heightPercentage": 1.2
      },
      // Names of the warp command and its variants, used for the reminders feature
      // You shouldn't have to change these
      "warpCommandVariants": [
         "warp",
         "is",
         "warpforge",
         "savethejerrys"
      ]
    }
    ```
3. Add your textures at the texture paths you configured above

# Testing Your Resource Pack
1. Enable the developer mode in the mod's settings (accessed via pause game > mod options > Fancy Warp Menu > config)
2. Go on SkyBlock
3. Apply your resource pack following the same process for applying a regular Minecraft resource pack
4. Open the Fancy Warp Menu. You should see borders around the buttons and a text box by your cursor showing the grid points your mouse is hovering over. These will help you position your textures.
5. Press the `R` key to reload the warp menu textures. The game will freeze for a few seconds as the textures load.
6. Check if your textures have loaded and are displayed correctly. If they didn't load, close the warp menu and there should be a message in chat telling you what went wrong.
7. Edit your resource pack, re-apply it, then press `R` again to reload textures.
8. Check the results and repeat the process until you are satisfied.

# Portal Texture License
The portal texture located at `Pack/pack.png` is licensed under the following terms:

MIT License

Copyright (c) 2023 Biscuit Development

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.