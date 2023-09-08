# Fancy Warp Pack Template
Resource pack template for my Fancy Warp Menu mod

-----

# How to Create Your Own Pack
1. Create a new repository using the button above and checkout to your IDE. Alternatively, you can download this template using the `<> Code` button above.
2. Choose a Resource Pack Template

## Custom Layout Pack Template
Use this template to create a custom layout with custom button positions and/or button textures.
1. The template is located in `Resource Packs/Custom Layout Pack`. This folder contains the folders and files you'll need to create your pack.
2. Set up your text editor to use the [layout.schema.json](Schemas/layout.schema.json) schema to provide hints and autocomplete. Here are some links to instructions for common text editors:
   1. [VSCode](https://code.visualstudio.com/docs/languages/json#_mapping-to-a-schema-in-the-workspace)
   2. [JetBrains IDEs](https://www.jetbrains.com/help/idea/json.html#ws_json_schema_add_custom)
   3. [Other Supported Editors](https://json-schema.org/implementations.html#editors)
   <br>
   If you don't have any of these text editors, you can look at the contents of `layout.schema.json` or see [layout.json](Resource%20Packs/Custom%20Layout%20Pack/assets/fancywarpmenu/data/layout.json) for an example. 
3. Edit the options in [layout.json](Resource%20Packs/Custom%20Layout%20Pack/assets/fancywarpmenu/data/layout.json) to your liking.
4. Add your textures at the texture paths you configured above.
5. Change the pack description in `pack.mcmeta` and the name of the `Custom Layout Pack` folder to your liking.

## Translation Test Pack Template
Use this template to check how your translations appear in the mod.
1. The template is located in `Resource Packs/Translation Test Pack`. This folder contains the folders and files you'll need to create your pack.
2. Go to the [Crowdin project](https://crowdin.com/project/fancy-warp-menu) and open the translation editor.
3. Click the `≡` icon in the top left. Then click `Download` to download your translations.
4. Copy the downloaded file to `Translation Test Pack/assets/fancywarpmenu/lang`
5. Copy the `Translation Test Pack` folder to your Minecraft resource packs folder and apply the resource pack.
6. Change your Minecraft language to the language you are working on in Crowdin
7. Your translations should now show in the Fancy Warp Menu. Check that they appear correctly.

# Testing Your Resource Pack
1. Enable the developer mode in the mod's settings at `Fancy Warp Menu > Settings Button (bottom right) > Developer Settings > Enable Developer Features`.
2. Enable the `Show Debug Overlay` and `Draw Button Borders` settings in the Developer Settings section. 
   These add borders around the buttons and a text box by your cursor showing the grid points your mouse is hovering over. These will help you position your textures.
   You cna toggle the debug overlay by pressing `TAB` in the Fancy Warp Menu and toggle the button borders by pressing `B`.
3. Go on SkyBlock or enable the `Skip SkyBlock Checks` setting in the mod and go to a single player world.
4. Copy your resource pack folder (e.g. `Custom Layout Pack`) to Minecraft's resource pack folder.
5. Apply your resource pack following the same process for applying a regular Minecraft resource pack.
6. Open the Fancy Warp Menu (If you're in single player you'll need to use the hotkey). You should now see your custom layout in the Fancy Warp Menu.
7. Check if your textures have loaded and are displayed correctly. If they didn't load, close the warp menu and there should be a message in chat telling you what went wrong.
8. Edit the files in your resource pack as required.
9. Press the `R` key to reload `layout.json` or `SHIFT + R` to reload `layout.json` and textures. The game will freeze for a few seconds as the textures load.
10. Check the results and repeat the process until you are satisfied.

![A screenshot of the Fancy Warp Menu Debug Overlay with button borders enabled](Debug%20Overlay.png)
_A screenshot of the Fancy Warp Menu Debug Overlay with button borders enabled_