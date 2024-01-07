# <img src="https://github.com/pizzaboxer/bloxstrap/raw/main/Images/Bloxstrap.png" width="28"/> Ultimate Fast Flags List 
##### Version: 4[.](https://github.com/GoingCrazyDude/fastflags-collection/blob/main/README.md)0.1 [1/7/2024]
* **106 Currently Listed**

 # How to use
* **Open the [Bloxstrap](https://github.com/pizzaboxer/bloxstrap) Menu**
* **Fast Flags >> Fast Flags Editor >> Import Json**
* **Paste in the JSON**
* **Then you should be good to go and save!**

 # List Navigation
* **[Rendering](https://github.com/devstacking/Epic-Fast-Flags-List#rendering)**
* **[Graphical](https://github.com/devstacking/Epic-Fast-Flags-List#graphical-settings)**
* **[UI](https://github.com/devstacking/Epic-Fast-Flags-List#user-interface)**
* **[QOL](https://github.com/devstacking/Epic-Fast-Flags-List#quality-of-life)**
* **[Textures](https://github.com/devstacking/Epic-Fast-Flags-List#textures)**
* **[Physics](https://github.com/devstacking/Epic-Fast-Flags-List#physics)**
* **[Other FFlags](https://github.com/devstacking/Epic-Fast-Flags-List#other-fflags)**
* **[Links](https://github.com/devstacking/Epic-Fast-Flags-List#links)**

<img src="https://github.com/devstacking/Epic-Fast-Flags-List/assets/106433721/0d16e448-4097-44ef-9eef-c445155a4bcb" width="888"/>

# Rendering API
### Metal
###### MacOS Only
```json
{
	"FFlagDebugGraphicsPreferMetal": "True"
}
```
### Vulkan
```json
{
	"FFlagDebugGraphicsDisableDirect3D11": "True",
	"FFlagDebugGraphicsPreferVulkan": "True"
}
```
### OpenGL
```json
{
	"FFlagDebugGraphicsDisableDirect3D11": "True",
	"FFlagDebugGraphicsPreferOpenGL": "True"
}
```
### DX10
```json
{
	"FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### DX11
```json
{
	"FFlagDebugGraphicsPreferD3D11": "True"
}
```
# Graphical Settings <sup>& other stuff</sup>
### idk
```json
{
	"DFFlagDebugEnableStreamingSolverVisualization": "True"
}
```
### Alternate Graphics Quality Selector
###### 1-21
```json
{
	"FFlagFixGraphicsQuality": "True"
}
```
### Disable Shadows
```json
{
	"FIntRenderShadowIntensity": "0"
}
```
### Set Fps Limit
```json
{
	"DFIntTaskSchedulerTargetFps": "9999"
}
```
### Enables Network Debug Tracker menu
##### Instructions: CTRL+F8
###### it's over.
```json
{
	"DFFlagDebugEnableInterpolationVisualizer": "True"
}
```
### Humanoid Outline
##### Draws an outline around every part and every humanoid
```json
{
	"DFFlagDebugDrawBroadPhaseAABBs": "False"
}
```
### Buggy ZPlane Camera *<sup>a.k.a xray</sup>*
```json
{
	"FIntCameraFarZPlane": "0"
}
```
### Preserve rendering quality with display setting
```json
{
	"DFFlagDisableDPIScale": "True"
}
```
```json
{
	"DFFlagDisableDPIScale": "True"
}
```
### Low Graphics Quality w/ Max Render Distance
###### Explanation: 1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider
```json
{
	"DFIntDebugFRMQualityLevelOverride": "1"
}
```
##### Heres 1-10 > 1-21
```
Low

1 = 1
2 = 2
3 = 6

High

4 = 7
5 = 11
6 = 14
7 = 15 
8 = 17
9 = 18
10 = 21
```
### Low Render Distance
###### *[21 Limit]*
```json
{
	"DFIntDebugRestrictGCDistance": "1"
}
```
### Disable Wind
```json
{
	"FFlagGlobalWindRendering": "False",
	"FFlagGlobalWindActivated": "False"
}
```
### Limits light updates
```json
{
	"FIntRenderLocalLightUpdatesMax": "8",
	"FIntRenderLocalLightUpdatesMin": "6"
}
```
### Disables fade in and fade out animation every light update
###### changes fade in ms!!
```json
{
	"FIntRenderLocalLightFadeInMs": "0"
}
```
### Makes avatars shiny 
###### [everything goes black on <3] ***[DFIntDebugFRMQualityLevelOverride is there to set your graphics to 10, You can change it to anything above 3: [Click here to view](https://github.com/devstacking/Epic-Fast-Flags-List/#heres-1-10--1-21) ]***
```json
{
	"DFIntRenderClampRoughnessMax": "-640000000",
	"DFIntDebugFRMQualityLevelOverride": "21"
}
```
### Disable PostFX
```json
{
	"FFlagDisablePostFx": "True"
}
```
### Pause Voxelizer/Disable Baked Shadows
```json
{
	"DFFlagDebugPauseVoxelizer": "True"
}
```
### Reduce Textures
```json
{
	"FFlagGraphicsGLTextureReduction": "True"
}
```
### Gray Sky
```json
{
	"FFlagDebugSkyGray": "True"
}
```
### Disable Player Shadows
```json
{
	"FIntRenderShadowIntensity": "0"
}
```
### Force LOD on Meshes
```json
{
	"DFIntCSGLevelOfDetailSwitchingDistance": "0",
	"DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
	"DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
	"DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Lighting Attenuation
```json
{
	"FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
###### Combine with [Lighting Attenuation](https://github.com/devstacking/Epic-Fast-Flags-List#lighting-attenuation) for better vision
```json
{
	"FFlagFastGPULightCulling3": "True"
}
```
### Frame Buffer
###### Explnation: 0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag
```json
{
	"DFIntMaxFrameBufferSize": "4"
}
```
### High Quality Textures 
###### *[1-3]*
```json
{
	"DFFlagTextureQualityOverrideEnabled": "True",
	"DFIntTextureQualityOverride": "3"
}
```
### Remove Grass
```json
{
	"FIntFRMMinGrassDistance": "0",
	"FIntFRMMaxGrassDistance": "0",
	"FIntRenderGrassDetailStrands": "0",
	"FIntRenderGrassHeightScaler": "0"
}
```
### Force MSAA 
###### *[0, 1, 2, 4, 8, 16]*
```json
{
	"FIntDebugForceMSAASamples": "4"
}
```
### ShadowMap Bias 
###### ***[Future & ShadowMap]***
```json
{
	"FIntRenderShadowmapBias": "75"
}
```
# User Interface
### Cleaner ESC Menu
###### [Link to Original Post](https://discord.com/channels/1099468797410283540/1189607691849564230)
```json
{
	"FFlagEnableAudioOutputDevice": "False",
	"FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0",
	"FFlagEnableAccessibilitySettingsInExperienceMenu2": "False"
}
```
### Hides gui
```json
{
	"FFlagDebugAdornsDisabled": "True"
}
```
### Dont Render UI
```json
{
	"FFlagDebugDontRenderUI": "True"
}
```
### V3 Menu
```json
{
	"FFlagEnableV3MenuABTest3": "True"
}
```
### Enable Audio Controller
```json
{
	"FFlagTrackerLodControllerDebugUI": "True"
}
```
### Disable Autocomplete
```json
{
	"FFlagEnableCommandAutocomplete": "False"
}
```
### Chrome UI TopBar
```json
{
	"FFlagEnableInGameMenuChrome": "True"
}
```
### Disable Bubble Chat
```json
{
    "FFlagEnableBubbleChatFromChatService": "False"
}
```
### Disable Selfview
```json
{
    "FFlagCoreGuiTypeSelfViewPresent": "False"
}
```
### Remove VC Bubble
```json
{
    "FFlagVoiceBetaBadge": "False"
}
```
### Pin Chat on Chrome UI
```json
{
    "FFlagEnableChromePinnedChat": "True"
}
```
### Hide guis
###### ***Instructions: Replace "ID" with any group ID that you are in.***
```json
{
	"DFIntCanHideGuiGroupId": "ID"
}
```
### Accessibility Settings 
###### [V1 & V4]
```json
{
	"FFlagEnableAccessibilityCounters": "True",
	"FFlagEnableAccessibilitySettingsAPIV2": "True",
	"FFlagEnableAccessibilitySettingsEffectsInCoreScripts2": "True",
	"FFlagEnableAccessibilitySettingsEffectsInExperienceChat": "True",
	"FFlagEnableAccessibilitySettingsInExperienceMenu2": "True",
	"FFlagEnableAccessibilitySettingsEffectsInLuaApp2": "True",
	"FFlagEnableAccessibilitySettingsEffectsInModules": "True",
	"FFlagEnableAccessibilitySettingsInAppShellSettings2": "True"
}
```
### Disable Fullscreen Title Bar
```json
{
	"FFlagInGameMenuV1FullScreenTitleBar": "False"
}
```
### Set Custom Font Size
```json
{
	"FIntFontSizePadding": "1"
}
```
### Remove Home Button
```json
{
	"FFlagInGameMenuHomeButton": "False"
}
```
# Quality Of Life 

### Disable ADs
```json
{
	"FFlagAdServiceEnabled": "False"
}
```

### Disable Telemetry 
###### *[This doesn't fully disable telemetry]*
```json
{
	"FFlagDebugDisableTelemetryEphemeralCounter": "True",
	"FFlagDebugDisableTelemetryEphemeralStat": "True",
	"FFlagDebugDisableTelemetryEventIngest": "True",
	"FFlagDebugDisableTelemetryPoint": "True",
	"FFlagDebugDisableTelemetryV2Counter": "True",
	"FFlagDebugDisableTelemetryV2Event": "True",
	"FFlagDebugDisableTelemetryV2Stat": "True"
}
```
### Scroll Speed
```json
{
	"FIntScrollWheelDeltaAmount": "140"
}
```
### Surf the web inside of Roblox
###### Click the Beta badge or the 13+ badge to open the webview browser.
```json
{
	"FFlagTopBarUseNewBadge": "True",
	"FStringTopBarBadgeLearnMoreLink": "https://google.com",
	"FStringVoiceBetaBadgeLearnMoreLink": "https://google.com"
}
```
# Textures
### No Textures
```json
{
    "FStringPartTexturePackTable2022": "{\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]}}",
    "FStringPartTexturePackTablePre2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
    "FStringTerrainMaterialTable2022": "",
    "FStringTerrainMaterialTablePre2022": ""
}
```
### Goofy Wood Textures
```json
{
    "FStringPartTexturePackTablePre2022": "{\"foil\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[238,238,238,255]},\"asphalt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[227,227,228,234]},\"basalt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[160,160,158,238]},\"brick\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[229,214,205,227]},\"cobblestone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,219,219,243]},\"concrete\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[225,225,224,255]},\"crackedlava\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[76,79,81,156]},\"diamondplate\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[210,210,210,255]},\"fabric\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[221,221,221,255]},\"glacier\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[225,229,229,243]},\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]},\"granite\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[210,206,200,255]},\"grass\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[196,196,189,241]},\"ground\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[165,165,160,240]},\"ice\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[235,239,241,248]},\"leafygrass\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[182,178,175,234]},\"limestone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[250,248,243,250]},\"marble\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[181,183,193,249]},\"metal\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[226,226,226,255]},\"mud\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[193,192,193,252]},\"pavement\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,218,219,236]},\"pebble\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[204,203,201,234]},\"plastic\":{\"ids\":[\"\",\"rbxassetid://9475422736\"],\"color\":[255,255,255,255]},\"rock\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[211,211,210,248]},\"corrodedmetal\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[206,177,163,180]},\"salt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[249,249,249,255]},\"sand\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,216,210,240]},\"sandstone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[241,234,230,246]},\"slate\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[235,234,235,254]},\"snow\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[239,240,240,255]},   \"credits\":{\"ids\":[\"pastelist/on/discord\",\"https://kits.ju.mp\"],\"color\":[238,238,238,255]},   \"wood\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[217,209,208,255]},\"woodplanks\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[207,208,206,254]}}"
}
```
### Troll Face Textures
```json
{
    "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://9475422736\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[207,208,206,254]}}",
    "FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://9475422736\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[207,208,206,254]}}"
}
```
### Black Textures
```json
{
    "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glass\u0022:{\u0022ids\u0022:[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\u0022color\u0022:[55, 55, 55, 255]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]}}",
    "FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glass\u0022:{\u0022ids\u0022:[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\u0022color\u0022:[55, 55, 55, 255]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]}}"
}
```
### Minecraft Textures
```json
{
	"FStringPartTexturePackTablePre2022": "{\"foil\":{\"ids\":[\"rbxassetid://9873266399\",\"rbxassetid://9438410239\"],\"color\":[238,238,238,255]},\"asphalt\":{\"ids\":[\"rbxassetid://9867974823\",\"rbxassetid://9844502433\"],\"color\":[227,227,228,234]},\"basalt\":{\"ids\":[\"rbxassetid://11545552824\",\"rbxassetid://11545440462\"],\"color\":[160,160,158,238]},\"brick\":{\"ids\":[\"rbxassetid://9924770651\",\"rbxassetid://9924770538\"],\"color\":[229,214,205,227]},\"cobblestone\":{\"ids\":[\"rbxassetid://9919719550\",\"rbxassetid://9438453972\"],\"color\":[218,219,219,243]},\"concrete\":{\"ids\":[\"rbxassetid://9924775913\",\"rbxassetid://9924775826\"],\"color\":[225,225,224,255]},\"crackedlava\":{\"ids\":[\"rbxassetid://9920485426\",\"rbxassetid://9438453972\"],\"color\":[76,79,81,156]},\"diamondplate\":{\"ids\":[\"rbxassetid://10237721036\",\"rbxassetid://9438453972\"],\"color\":[210,210,210,255]},\"fabric\":{\"ids\":[\"rbxassetid://9920517963\",\"rbxassetid://9438453972\"],\"color\":[221,221,221,255]},\"glacier\":{\"ids\":[\"rbxassetid://9920518995\",\"rbxassetid://9438453972\"],\"color\":[225,229,229,243]},\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]},\"granite\":{\"ids\":[\"rbxassetid://9920550720\",\"rbxassetid://9438453972\"],\"color\":[210,206,200,255]},\"grass\":{\"ids\":[\"rbxassetid://11152995545\",\"rbxassetid://9267183930\"],\"color\":[196,196,189,241]},\"ground\":{\"ids\":[\"rbxassetid://11546360009\",\"rbxassetid://11545533676\"],\"color\":[165,165,160,240]},\"ice\":{\"ids\":[\"rbxassetid://9920556429\",\"rbxassetid://9438453972\"],\"color\":[235,239,241,248]},\"leafygrass\":{\"ids\":[\"rbxassetid://11152995545\",\"rbxassetid://9267183930\"],\"color\":[182,178,175,234]},\"limestone\":{\"ids\":[\"rbxassetid://9920561624\",\"rbxassetid://9438453972\"],\"color\":[250,248,243,250]},\"marble\":{\"ids\":[\"rbxassetid://9873292869\",\"rbxassetid://9438453972\"],\"color\":[181,183,193,249]},\"metal\":{\"ids\":[\"rbxassetid://11546526557\",\"rbxassetid://11546431794\"],\"color\":[226,226,226,255]},\"mud\":{\"ids\":[\"rbxassetid://9920578676\",\"rbxassetid://9438453972\"],\"color\":[193,192,193,252]},\"pavement\":{\"ids\":[\"rbxassetid://11546539560\",\"rbxassetid://11546440685\"],\"color\":[218,218,219,236]},\"pebble\":{\"ids\":[\"rbxassetid://9920581197\",\"rbxassetid://9438453972\"],\"color\":[204,203,201,234]},\"plastic\":{\"ids\":[\"\",\"rbxassetid://9868015012\"],\"color\":[255,255,255,255]},\"rock\":{\"ids\":[\"rbxassetid://11546570730\",\"rbxassetid://11546456858\"],\"color\":[211,211,210,248]},\"corrodedmetal\":{\"ids\":[\"rbxassetid://11545623165\",\"rbxassetid://11545476330\"],\"color\":[206,177,163,180]},\"salt\":{\"ids\":[\"rbxassetid://9920590478\",\"rbxassetid://9438453972\"],\"color\":[249,249,249,255]},\"sand\":{\"ids\":[\"rbxassetid://11546588111\",\"rbxassetid://11546468464\"],\"color\":[218,216,210,240]},\"sandstone\":{\"ids\":[\"rbxassetid://9920596353\",\"rbxassetid://9438453972\"],\"color\":[241,234,230,246]},\"slate\":{\"ids\":[\"rbxassetid://9867974823\",\"rbxassetid://9844502433\"],\"color\":[235,234,235,254]},\"snow\":{\"ids\":[\"rbxassetid://11536062048\",\"rbxassetid://11108916253\"],\"color\":[239,240,240,255]},\"wood\":{\"ids\":[\"rbxassetid://9867974813\",\"rbxassetid://9844454989\"],\"color\":[217,209,208,255]},\"woodplanks\":{\"ids\":[\"rbxassetid://9867974813\",\"rbxassetid://9844454989\"],\"color\":[207,208,206,254]}}"
}
```
# Physics
### Physics FPS 
```json
{
	"FFlagDebugSimIntegrationStabilityTesting": "True"
}
```
### drunk
```json
{
	"DFIntGeometricStiffnessAlpha": "-100000"
}
```
### Breaks glitches stuff
###### All type of wallhops, longjumps, headhitters and probably more stop working
```json
{
	"DFFlagSimHumanoidPhysics": "True"
}
```
### Max Raycast Distance
###### Break legs collision from 2 to -inf, kinda break camera on values over 3
```json
{
	"DFIntRaycastMaxDistance": "0"
}
```
### Breaks movement on higher negative values
```json
{
	"FIntPGSAngularDampingPermilPersecond": "-10000"
}
```
### It allows you to fall quicker and ignore certain block designs
```json
{
	"FFlagHumanoidOnlySetCollisionsOnStateChangeDefaultIsEnabled": "False",
	"FFlagHumanoidParallelFasterSetCollision": "True"
}
```
### Gear Desync
```json
{
	"DFIntDataSenderRate": "-1"
}
```
### 9. Freezes character in any state, can cause crashes, basically stacks input data
```json
{
	"FFlagSimIslandizerManager": "False"
}
```
### Spin when moving
```json
{
	"DFIntRunningBaseOrientationP": "-14"
}
```
### Spin when falling
```json
{
	"DFIntRunningBaseOrientationP": "-14"
}
```
### Makes character upside down
```json
{
	"DFIntFreeFallBalanceP": "-9999"
}
```
### Makes character ragdoll forever
```json
{
	"DFIntGettingUpBalanceP": "0"
}
```
### Fake Lag
```json
{
	"DFIntS2PhysicsSenderRate": "1"
}
```
### Noclip 1
```json
{
	"DFFlagAssemblyExtentsExpansionStudHundredth": "-50"
}
```
### Noclip 2
```json
{
	"FIntPGSPenetrationMarginMax": "2147483647",
	"FIntPGSPenetrationMarginMin": "2147483647"
}
```
### Noclip Combo
```json
{
	"DFFlagAssemblyExtentsExpansionStudHundredth": "-40",
	"FIntPGSPenetrationMarginMax": "2147483647",
	"FIntPGSPenetrationMarginMin": "2147483647"
}
```
### Allows you to boounce when flicking
```json
{
	"DFIntNewRunningBaseAltitudeP": "49534"
}
```
### Ragdoll Loop 
###### only when you are already in a ragdoll state
```json
{
	"DFIntGettingUpBalanceD": "-110000"
}
```
### Become a ball
```
{
	"DFIntDefaultBalanceD": "-17575",
	"DFIntGeometricStiffnessAlpha": "-17575"
}
```
### Bounces character constantly at 0 
###### Jump to randomly bounce yourself high
```json
{
	"DFIntNewRunningBaseAltitudeD": "0"
}
```
### Super Jump Combo
```
this is not leaked yet
gatekept
```
### Very limited speed fflag that works only in a few games
###### one of them being Phantom Forces, and it makes you only slightly faster
```json
{
	"DFIntDebugSimPhysicsSteppingMethodOverride": "10000000"
}
```
### possible super jump blah bla vbla
```json
{
	"DFIntNewRunningBaseGravityReductionFactorHundredth": "1000"
}
```
### Set Hip Height
###### Very controllable bounce, only works with negative values, 0 allows you to hover
```json
{
	"DFIntMaxAltitudePDStickHipHeightPercent": "-200"
}
```
### Head Collisions R15
```json
{
	"FFlagMeshPartHeadsDefaultIsEnabled": "False"
}
```
### Noclip <sup>literally</sup>
```json
{
	"DFIntSHCellMinSizeAsBitShift": "4"
}
```
### Wallglide
```json
{
	"DFFlagUnstickForceAttackInTenths": "-4"
}
```
# other fflags
### Sounds use physical velocity and become distorted
```json
{
	"FFlagSoundsUsePhysicalVelocity": "True"
}
```
### Shows the state of a flag
```json
{
	"FStringDebugShowFlagState": "Value"
}
```
###### e.g
```json
{
	"FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName"
}
```

### MTU 
###### ***[Might Improve Ping]***
```JSON
{
	"DFIntConnectionMTUSize": "Value"
}
```
### No Internet Disconnect 
###### *[You will still be kicked but the message wont show.]*
```json
{
	"DFFlagDebugDisableTimeoutDisconnect": "True"
}
```
### Quick Game Launch 
###### *[BUGGY]*
```json
{
	"FFlagEnableQuickGameLaunch": "True"
}
```
### Allows you to change voice chat distance 
###### default: [Min 7 Max 80]
```json
{
	"DFIntVoiceChatRollOffMinDistance": "7",
	"DFIntVoiceChatRollOffMaxDistance": "80"
}
```
### Disable In-Game Purchases
```json
{
	"DFFlagOrder66": "True"
}
```
### Disable Chat
```json
{
	"FFlagDebugForceChatDisabled": "True"
}
```
### Limit audios that are being played
```json
{
	"DFIntMaxLoadableAudioChannelCount": "1"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
	"FFlagDebugHumanoidRendering": "True"
}
```
### Custom Disconnect Message
```json
{
	"FFlagReconnectDisabled": "True",
	"FStringReconnectDisabledReason": "You're stupid and I hate you"
}
```
### Display FPS
```json
{
	"FFlagDebugDisplayFPS": "True"
}
```
### Verified Badge
```json
{
	"FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified Badge on everyone
```json
{
	"FFlagOverridePlayerVerifiedBadge": "True"
}
```
### Applies cool colors to Unthemed Stuff
```json
{
	"FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Show Outlined Chunks
```json
{
	"FFlagDebugLightGridShowChunks": "True"
}
```
### Remove Disconnect Blur/Loading Blur
```json
{
	"FIntRobloxGuiBlurIntensity": "0"
}
```
### Disable Dynamic Heads Animations
```json
{
	"DFFlagEnableDynamicHeadByDefault": "False"
}
```
### Gray avatar
###### clientsided
```json
{
	"FFlagFailsafeHumanoid_3": "True"
}
```
### Automatically unmutes your mic on join
```json
{
	"FFlagDebugDefaultChannelStartMuted": "False"
}
```
### Overlay that shows what you type 
```json
{
	"FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### Disable Output Device
###### useless settings ngl
```json
{
	"FFlagEnableAudioOutputDevice": "False"
}
```
### opt-out Experience Language
###### Removes the Experience Language option in settings
```json
{
	"FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Exclusive Fullscreen
###### Alt + Delete
```json
{
	"FFlagHandleAltEnterFullscreenManually": "False"
}
```
### Lets you change the zoom out limit
###### infinite zoom out!!
```json
{
	"FIntCameraMaxZoomDistance": "9999"
}
```
### Limits number of animations being played
###### infinite zoom out!!
```json
{
	"DFIntMaxActiveAnimationTracks": "0"
}
```
# Links
### [Make Your Own Custom Roblox Textures](https://github.com/GoingCrazyDude/roblox-custom-textures/blob/main/README.md) *[Github Repo Link]*
### [MEGA FAG LIST](https://discord.com/channels/1099468797410283540/1139962301991104582/1170417533355036712) *[Bloxstrap Server]*
### [Bloxstrap](https://github.com/pizzaboxer/bloxstrap) *[Github Repo Link]*
### [NVIDIA Shaders Guide](https://github.com/catb0x/Roblox-Shaders-Guide) *[Github Repo Link]*
### [EnableAnselForRoblox](https://github.com/DED0026/EnableAnselForRoblox) *[Github Repo Link]*
### [potato fflags](https://github.com/catb0x/Roblox-Potato-FFlags) *[Github Repo Link]*
### [Fake Roblox Player Internal Patcher](https://github.com/devstacking/Roblox-Player-Internal-Patcher/releases/download/Release/FakeInternal.exe) *[Download Link]*

####  You've reached the bottom of the list! 

# List Information
* Creation Date: 9:46 PM 08/25/2023 
* Github Publish Date: 12/26/2023
###### [<sup>OG</sup>](https://rentry.org/uffl/)

##### FastFlags 2024®<sup>eal</sup>
##### Not affiliated with [Bloxstrap](https://github.com/pizzzaboxer/Bloxstrap)
