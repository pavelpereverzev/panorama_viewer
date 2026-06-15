# QGIS Panorama Viewer

<img width="590" height="398" alt="screen_pano" src="https://github.com/user-attachments/assets/b954ff35-d314-4a96-ac53-82fe020e4ee0" />


A QGIS plugin which allows to view panoramic images (photospheres, 360° photos) directly in QGIS. Built on [**Pannellum**](https://pannellum.org/) and [**Three.js**](https://threejs.org/) libraries.

## Features
- View 360° photos from local files or web URLs taken from layers' feature attributes
- Show direction sector relative to point on map
- Set custom initial viewing angle
- Choose between two rendering engines (Pannellum / Three.js)
- Fullscreen-like expanded view
- Open current panorama directly in browser

## Quick guide
1. Install plugin in QGIS.
2. Open a layer of any geometry type.
3. Add a text field in the attribute table.
4. Insert direct links to 360° photos (local files or web) into text field.
5. Open plugin, select Layer and Field with images links
7. Select an object on your map.
8. Click **View panorama** to see the 360° photo.

## Controls & Options

**Main Controls**

| Option | Description |
|--------|-------------|
| **Auto-update view** | Automatically loads panorama when selecting a new feature |
| **Show directions** | Draws a direction sector near the panorama point on the map |
| **Angle field** | Select a field containing the initial viewing angle for specific panoramas |
| **Viewer selector** | Choose between *Pannellum* or *Three.js* (Pannellum is unavailable on macOS, only Three.js shown) |

**Hidden Buttons** (bottom-right corner of the image widget, appear on hover)

<img width="122" height="48" alt="screen_pano_corned" src="https://github.com/user-attachments/assets/61f7b748-ed52-4b72-99e2-25c4bf1bf058" />


| Button | Action |
|--------|--------|
| <img width="16" height="16" alt="icon_1" src="https://github.com/user-attachments/assets/d6a0d453-aa7c-4d5d-8b50-8694cdce3f77" /> | Open the current panorama image in your web browser |
| <img width="16" height="16" alt="icon_2" src="https://github.com/user-attachments/assets/82b02ebc-cab4-423e-ae51-d0d66773be86" /> | Hide part of the plugin interface to expand the panorama viewer to maximum available size |

## Video preview

https://github.com/user-attachments/assets/b102d41b-f0cf-41ec-800f-f25a0aca2fd8

## Known issues

- works under QGIS 3.x.x versions with Qt5. Another QGIS versions with Qt6 has no specific components (Qt webkit tools) to run plugin.
- opening image in browser (using <img width="16" height="16" alt="icon_1" src="https://github.com/user-attachments/assets/d6a0d453-aa7c-4d5d-8b50-8694cdce3f77" /> button) may not working sometimes and freeze plugin.


