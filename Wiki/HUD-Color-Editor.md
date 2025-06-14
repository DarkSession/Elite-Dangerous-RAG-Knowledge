# HUD Color Editor
Arkku HUD color theme editor
 		 	 

A **HUD Color Editor** is a custom tool that helps *Elite Dangerous* players customise the colours of the game's universal HUD by changing the RGB values. The standard HUD colours are based on the game's signature "star" orange tint, with varying shades to discern between different sections.^[1]^

Many players do not find the orange tint very desirable and often wish to change it. This can be done by editing the .ini files in the game and can be done without the need of the editor. The effects are purely client-side and Frontier Developments has stated that they have no issue with commanders using such mods, and even promoted several videos feature a customised HUD.

## 

Contents

- 1 Preparation
- 2 Instructions
- 3 Example XML File
- 4 Videos
- 5 References

## Preparation

- Before you do anything to your .xml file, make a backup to save previous settings.
- Note that the colours will affect most aspects of the HUD, including enemy and ally colours as well as shields. Be careful when changing colours as it can make it harder to identify friend from foe or see warnings. Also, one universal downside is that it will always change how commander pictures are seen; with the effects being more profound with certain values.

## Instructions

The .xml file is named GraphicsConfigurationOverride and is located in the following directories:

- **Windows**: %APPDATA%\..\Local\Frontier Developments\Elite Dangerous\Options\Graphics
- **OS X**: Library/Application Support/Frontier Developments/Elite Dangerous/Options/Graphics
- **SD/Linux**: ~/.steam/steam/steamapps/compatdata/359320/pfx/drive\_c/users/steamuser/AppData/Local/Frontier Developments/Elite Dangerous/Options/Graphics/

1. Open Steam and right click on Elite: Dangerous.
2. Go to Manage, then click Browse Local Files.
3. In your File Explorer, open the Products folder, then 'elite-dangerous-64.'
4. Make a copy of the GraphicsConfiguration.xml file (as a backup), then open the original file in a text editor.
5. Under the section 'GUIColour,' look for Standard under the Default heading in LocalisationName tags.
6. In the MatrixRed, MatrixGreen, and MatrixBlue sections, edit the HUD color by entering numbers between 0 and 1.
7. Save the file.^[2]^

- : Customise to your liking; copy the text (which is in the text box at the bottom left); paste the text inside your .xml, replacing the previous text.
- : Customise to your liking; press "Copy XML"; paste it into your .xml file, replacing the previous text.
- : Variation on Kerudo's editor with keyboard controls by Iodred, for ease of experimentation. Credits go to Kerudo

## Example XML File

Below is the default configuration.
```lang
<?xml version="1.0" encoding="UTF-8" ?>
<GraphicsConfig>
    <GUIColour>
        <Default>
            <LocalisationName>Standard</LocalisationName>
            <MatrixRed> 1, 0, 0 </MatrixRed>
            <MatrixGreen> 0, 1, 0 </MatrixGreen>
            <MatrixBlue> 0, 0, 1 </MatrixBlue>
        </Default>
    </GUIColour>
</GraphicsConfig>
```