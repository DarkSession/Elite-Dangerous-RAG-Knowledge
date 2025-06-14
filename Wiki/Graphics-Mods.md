# Graphics Mods
The graphics of ED can be modified in various ways.

## 

Contents

- 1 Texture resolution
- 2 For 8GB+ GPU
- 3 Custom Display Quality Settings
- 4 Ultra+ terrain quality
- 5 Anti-aliasing
    - 5.1 Nvidia Settings
    - 5.2 Supersampling
    - 5.3 Graphics settings
    - 5.4 AMD anti-aliasing
- 6 ED HUD Mod
- 7 ReShade
    - 7.1 Presets
- 8 Graphic Tweaks, Dreamscape Feeling & alii
- 9 Skybox Detail
- 10 Graphics override example
- 11 Videos
- 12 Gallery
- 13 References

## Texture resolution

 	 	[![Elite-Dangerous-Higher-Resolution-Planet-Textures](https://static.wikia.nocookie.net/elite-dangerous/images/0/09/Elite-Dangerous-Higher-Resolution-Planet-Textures.jpg/revision/latest/scale-to-width-down/200?cb=20181107090041)](https://static.wikia.nocookie.net/elite-dangerous/images/0/09/Elite-Dangerous-Higher-Resolution-Planet-Textures.jpg/revision/latest?cb=20181107090041) 	 		 			 		 		 		 			
ED higher resolution planet textures
 		 	 

You can increase the texture resolution of planets, the galaxy background and the environment map. Note this was tested on 1 November 2018.

If you want to keep things simple you can paste this into your "GraphicsConfigurationOverride.xml" file (normally located in %LocalAppData%\Frontier Developments\Elite Dangerous\Options\Graphics\):^[1]^^[2]^

```
<?xml version="1.0" encoding="UTF-8" ?>
<GraphicsConfig><Planets>	<Ultra>		<TextureSize>4096</TextureSize>		<WorkPerFrame>512</WorkPerFrame>	</Ultra></Planets><GalaxyBackground>	<High>		<TextureSize>4096</TextureSize>	</High></GalaxyBackground><Envmap>	<High>		<TextureSize>1024</TextureSize>		<NumMips>10</NumMips>	</High></Envmap>
</GraphicsConfig>
```

Note that I recommend against using texture resolutions past 4096 as you will get progressively more noticeable texture pop-in around complex areas like starports, irrespective of how much video memory you have. You can use 8192 or even 16384 for screen shots of planets, but I don't consider them suitable for general play.^[1]^

## For 8GB+ GPU

The following should only be implemented if you have a decent newer card with 8GB+ VRAM - and note my setup is only 2560x1080 with 75hz monitor, RX 6800 card - If you run ED at 4K and are already struggling maybe these will not be any benefit for you.  They cause no FPS hits during ship and on foot exploring gameplay and see a huge improvement to the milkyway skybox, planet texture quality and anecdotally see far less terrain LOD morphing on surfaces either on approach or driving/flying low over the surface.^[2]^ These recommendations were made by DisillusionedBook.

In my `GraphicsConfigurationOverride.xml` file I have these overrides (I also make the same changes in the main `GraphicsConfiguration.xml` file to the relevant sections (because one or more of the overrides need to be in there -- particularly the GalaxyMap ones I think). Make backup copies named .old of your existing files just in case.^[2]^ I modified these setting to be triggered when the graphics options are set to max (high/ultra depending on the setting).

```
<?xml version="1.0" encoding="UTF-8" ?>
<GraphicsConfig>
  <GalaxyMap><High>	<LocalisationName>$QUALITY_HIGH;</LocalisationName>	<NebulasCount>100</NebulasCount>	<NebulasInBackgroundCount>100</NebulasInBackgroundCount>	<LowResNebulasCount>50</LowResNebulasCount>	<HighResNebulasCount>10</HighResNebulasCount>	<LowResNebulaDimensions>64</LowResNebulaDimensions>	<HighResNebulaDimensions>256</HighResNebulaDimensions>	<LowResSamplesCount>276</LowResSamplesCount>	<HighResSamplesCount>552</HighResSamplesCount>	<MilkyWayInstancesCount>16000</MilkyWayInstancesCount>	<LocalDustBrightness>0.05</LocalDustBrightness>	<MilkywayInstancesBrightness>1.0</MilkywayInstancesBrightness>	<MilkywayInstancesSize>1.0</MilkywayInstancesSize>	<MilkyWayInstancesOffscreenRTEnabled>false</MilkyWayInstancesOffscreenRTEnabled>	<StarInstanceCount>5000</StarInstanceCount></High>
  </GalaxyMap>
  <GalaxyBackground><High><LocalisationName>$QUALITY_HIGH;</LocalisationName><TextureSize>4096</TextureSize></High>
  </GalaxyBackground>  
  <Planets>
    <Ultra>
      <LocalisationName>$QUALITY_ULTRA;</LocalisationName>
      <TextureSize>4096</TextureSize>
      <AtmosphereSteps>6</AtmosphereSteps>
      <CloudsEnabled>true</CloudsEnabled>
      <WorkPerFrame>328</WorkPerFrame>  <TexturePoolBudget>100</TexturePoolBudget>
    </Ultra>
  </Planets>
  <Envmap><High>	<LocalisationName>$QUALITY_HIGH;</LocalisationName>	<TextureSize>512</TextureSize>	<NumMips>16</NumMips></High>
  </Envmap>
</GraphicsConfig>
```

## Custom Display Quality Settings

The display quality settings can be customized. It appears that values as high as "1.999999" work for "Model Draw Distance"/"LODDistanceScale". Note this was tested on 15 June 2018.^[3]^

So, my Custom.fxcfg (normally located in "%LocalAppData%\Frontier Developments\Elite Dangerous\Options\Graphics" in your user profile directory), which contains the main display menu settings, looks like this:^[3]^

```
<?xml version="1.0" encoding="UTF-8" ?>
<Root PresetName="Custom"><BlurEnabled>true</BlurEnabled><AOQuality>3</AOQuality><DOFEnabled>0</DOFEnabled><BloomQuality>2</BloomQuality><EnvmapQuality>1</EnvmapQuality><MaterialQuality>3</MaterialQuality><EnvironmentQuality>3</EnvironmentQuality><FXQuality>3</FXQuality><GalaxyMapQuality>2</GalaxyMapQuality><GUIColourQuality>0</GUIColourQuality><TerrainQuality>3</TerrainQuality><TerrainLodBlendingQuality>2</TerrainLodBlendingQuality><SurfaceMaterialQuality>3</SurfaceMaterialQuality><JetConeQuality>3</JetConeQuality><VolumetricsQuality>3</VolumetricsQuality><ShadowQuality>4</ShadowQuality><TextureQualityEx>2</TextureQualityEx><AAMode>4</AAMode><SurfaceSamplerQuality>3</SurfaceSamplerQuality><PerformanceQualitySetting>0</PerformanceQualitySetting><ResolutionSetting>0</ResolutionSetting><LODDistanceScale>1.999999</LODDistanceScale><HMDRenderTargetMultiplier>1.000000</HMDRenderTargetMultiplier><SSAAMultiplier>1.000000</SSAAMultiplier><GpuSchedulerMultiplier>1.000000</GpuSchedulerMultiplier>
</Root>
```

This is essentially the "Ultra" preset with DOF (which is normally only used in the camera modes, but eats quite a bit of performance for an effect I don't like) disabled, the GPU terrain work slider maxed out (despite what the description states, I've only seen performance and smoothness improvements from increasing this to maximum on any upper end GPU hardware of the last several years, going back to at least my Radeon HD 290 and GeForce GTX 780), and the custom "LODDistanceScale" increase, which must be manually entered into this file, because the in-game slider maxes out at "1.000000".^[3]^

## Ultra+ terrain quality

In ED: Odyssey 4.1 you could set the "terrain quality" to "ULTRAFORCAPTURE". This increases the terrain level of detail and lighting beyond ultra. Odyssey - Update 6 renamed the "terrain quality" setting to "Ultra+" on July 29, 2021.^[4]^

## Anti-aliasing

ED doesn't currently have proper in-game anti-aliasing options. However, it can be improved with the following:

### Nvidia Settings

In Nvidia Settings select the following parameters:^[5]^

1. Default nvidia settings
2. In game AA = SMAA
3. In game supersampling 1.5
4. In game upscaling Normal

### Supersampling

A method to improve anti-aliasing is via supersampling. In 'quality' graphics options there is a property called 'supersampling'. Try setting your viewport to 1.25 or 1.50 and see the difference. It can impact the FPS (frames per second), because you're rendering a larger image in the background with much more pixels and the game scales that down to give you smoother graphics. 1.25x *size* is closer to 1.56x the area. **2.0x supersampling** renders twice the width and height or 4x the amount of pixels. The 'size' is 4x the area. If you don't have a powerful GPU then it can *tank* your frame rate.

If you're using a VR headset, use "HMD Quality" instead of "Supersampling" -- this defers the downsampling to the lens distortion compensation stage of your VR runtime's compositor, which yields much better quality due to a better fit, without intermediate degradation. If you are already at 2.0 HMDQ, *then* you can use SS on top, to go past that point (it *takes* that to really begin to have an effect on the aliasing), but you are unlikely to do that as yet, because by then you get into seconds-per-frame territory). 

**Recommended:** for the least aliasing use **X2.0 Supersampling,** then turn **FSR and Fidelity off**.^[6]^

The benefit with an NVidia RTX graphics card is you can use “DLDSR”, which upscales the image with DLSS 1.0 and then downscales it to your native resolution which makes it more efficient compared to regular super sampling.

### Graphics settings

Another option is set upscaling to Normal and AA to FXAA. This is the least non-blurry setting with little to no flickering of the edges. The other two AMD upscaling techniques can look good under certain circumstances but they reveal edge flickering. The sharpening option only applies to the "AMD FidelityFX CAS" upscaler.

### AMD anti-aliasing

Reduce aliasing to a minimum on AMD requires a high-end PC, because the performance decreases significantly.^[7]^

**Setup**

- AMD Ryzen 2700x
- RX 6800
- 34" Display at 3440x1440 100Hz

**Custom settings on Radeon Adrenalyn:**

- Radeon Super resolution enabled (Press on the "?" icon, the wizard will tell you which resolutions it will work with)
- AMD Fluid Motion Frames enabled
- Anti-lag enable
- Enhanced sync enable

Unfortunately the AMD Anti-aliasing doesn't seem to do a thing with this driver setting

**Game setting:**

- Resolution dropped to 3024x1296
- all quality settings on maximum
- Anti-Aliasing SMAA
- Supersampling 2.0
- Upscaling AMD FidelityFX CAS. However, FidelityFX CAS was broken in ED version 18.06. If you want any sharpening in-game, you need to use FSR, which you can supersample with by changing the "SSAAMultiplier" variable in Custom.4.0.fxcfg.

Now the important thing: Don't look at in-game FPS overlay. That will only show game rendering FPS, not final FPS. Use the Adrenalyn FPS counter. I get around 70-75 fps inside stations, 70-85 fps in surfaces, and it looks fluid.

6048\*2592 internal resolution with multiple filtering (VSR, plus the game's internal scaler or FSR) passes sent to a 3440\*1440 display will significantly reduce aliasing, but the performance hit is extreme and fluid motion frames has serious trade-offs.^[8]^

## ED HUD Mod

 	 	[![ED-HUD-Mod-EDHM](https://static.wikia.nocookie.net/elite-dangerous/images/f/f7/ED-HUD-Mod-EDHM.jpg/revision/latest/scale-to-width-down/200?cb=20200917234727)](https://static.wikia.nocookie.net/elite-dangerous/images/f/f7/ED-HUD-Mod-EDHM.jpg/revision/latest?cb=20200917234727) 	 		 			 		 		 		 			
ED HUD Mod
 		 	 

The HUD mod enables precise re-colouring of each HUD element, without the need to alter the XML. In doing so, we avoid the unintended XML side-effects on radar icons and pilot portraits. But it also means we can re-colour any HUD element, and we're not locked into a particular palette.^[9]^

We've also enabled coloured lighting effects in the cabin. The ambient light really changes the 'mood' of the pilot's environment, and you can even have multi-coloured lighting if you prefer.^[9]^

Lastly, some ships have lights on the dashboard or canopy that shine directly in your face. So we dimmed them down to reduce eye fatigue and make flying a more pleasant experience.^[9]^

The mod is based on software called 3dmigoto, which was introduced into the Elite community by CMDR AD in Feb 2019. He used 3dmigoto to turn off particular shaders, such as scratches on the windows, space dust and smoke in the cabin.^[9]^

- You can download and install the EDHM + UI here:
- The mod is also available bundled with the official UI, available at this link:
- Related mod:

## ReShade

 	 	[![EDFX Graphics Mod](https://static.wikia.nocookie.net/elite-dangerous/images/a/a4/EDFX_Graphics_Mod.jpg/revision/latest/scale-to-width-down/200?cb=20170214124253)](https://static.wikia.nocookie.net/elite-dangerous/images/a/a4/EDFX_Graphics_Mod.jpg/revision/latest?cb=20170214124253) 	 		 			 		 		 		 			
EDFX graphics mod
 		 	 
- Note the following mods could be outdated due to the lighting improvements of Beyond Chapter Four.

### Presets

- - EDFX add FX graphics effects to games using ReShade Shader Framework and manage Hud color.^[11]^ It's a premade Reshade profile with its own launcher and some other options.

For installing be careful to always follow the instructions of the preset.

## Graphic Tweaks, Dreamscape Feeling & alii

 	 	[![ED 035 Reshade zps63c772ba](https://static.wikia.nocookie.net/elite-dangerous/images/1/1e/ED_035_Reshade_zps63c772ba.jpg/revision/latest/scale-to-width-down/200?cb=20170222115947)](https://static.wikia.nocookie.net/elite-dangerous/images/1/1e/ED_035_Reshade_zps63c772ba.jpg/revision/latest?cb=20170222115947) 	 		 			 		 		 		 			
EDFX graphics mod
 		 	 
- **Note**: do this at your own risk and always make a backup of the GraphicsConfigurationOverride.xml file. If you're unsure what to do, don't try it.

The GraphicsConfigurationOverride.xml file is in %LocalAppData%\Frontier Developments\Elite Dangerous\Options\Graphics. Remove it, copy the original GraphicsConfiguration.xml there, rename it GraphicsConfigurationOverride.xml. Tweak there. Beware that some tweaks don't work with the Override (galaxy background for example).

## Skybox Detail

*Elite Dangerous* can be forced to render the skybox in much more detail, including nebulae, at the small cost of some stuttering in witchspace. Success also depends on the PC's capabilities.^[13]^ The process is as follows:

1. Find the GraphicsConfigurationOverride.xml file (copy and paste this on the address bar of any folder to find it: "%LocalAppData%\Frontier Developments\Elite Dangerous\Options\Graphics"). The GraphicsConfigurationOverride file is a disposable xml that can be used to safely edit the game's parameters without disrupting the GraphicsConfiguration file. Do undo any changes, delete the GraphicsConfigurationOverride file and the game will generate a new, blank one the next time it is loaded.

To verify the change is successful, then before implementing the change, take a screenshot of the Milky Way or a nebula and then immediately exit the game. Once the xml file has been edited, take a second screenshot immediately after logging back into the game. Both screenshots will have been taken from the exact same position with the exact same view of the skybox, allowing a direct comparison to be made.

Again, if there are any problems, delete the GraphicsConfigurationOverride file. Note that there are no apparent visual improvements if the TextureSize is set to a value higher than 4096, and doing so may only worsen the game's stuttering.

## Graphics override example

Created by StrixLVG aka LCARS and shared by Numenor1379.

Elite Dangerous allows you to run custom graphics settings that can increase the maximum graphics settings and in some cases correct some things. I have made an GraphicsConfigurationOverride XML file which changes the following:

- More stars rendered at once. You have 3 options (32.000, 64000 & 128000).
- Increases the planet texture resolution on the ultra setting to 4096x4096.
- Increases skybox texture resolution (Galaxy Background) to 1024x1024, 2048x2048 & 4096x4096 on Low, Medium and High settings respectively.
- Sets the correct Environment Ultra settings.
- Reduces the skybox dust visuals.
- Increases the amount of nebulas that can be shown on screen at the same time.
- Enhances Ultra Shadows to higher resolution and less issues.

The XML file should be placed in the following directory to install:
C:\Users\YOUR USERNAME\*\AppData\Local\Frontier Developments\Elite Dangerous\Options\Graphics

The username is whatever you have set it to be.

These settings are meant for people running the game with (near) max settings. For best results, run the game at max settings.

To the right of each setting value you can find the default value set by FDev to see the changes made.
Popular settings:

- StarInstanceCount: 				Maximum number of stars in your instance. A higher number shows more stars in your skybox.
- LocalDustBrightness:  			The amount of dust you can see in the instance skybox. A value of -0.1 completely disables the dust. A   non negative value increases the intensity of the dust.
- NebulasCount:						The amount of nebulas you can see at once in your instance and the galaxy map.
- Planets -&gt; TextureSize:			The texture quality of the planets. A higher number means higher detailed planets.
- GalaxyBackground -&gt; TextureSize:	Resolution of your skybox. A higher texture size is higher clarity.