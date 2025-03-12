# Skin Configuration Documentation

This readme explains most of the usage of `skin.json` file used in formatting gameplay and interface layouts in [osu!droid](https://github.com/osudroid/osu-droid).
For editing skin.json files i recommend using [Rian8337's](https://github.com/Rian8337) [Skin.json editor](https://rian8337.github.io/skin-json-editor/)


## Table Of Contents

1. [Overview](#overview)
2. [File Structure](#file-structure)
   - [Note](#Note)
   - [ComboColor](#combocolor)
   - [Slider](#slider)
   - [Cursor](#cursor)
   - [Utils](#utils)
   - [Color](#color)
   - [Fonts](#fonts)
   - [Layout](#layout)
3. [Usage](#usage)
4. [Contributing](#contributing)


## Overview
The `skin.json` file is a JSON-formatted configuration file that customizes the appearance and behavior of in-game elements. It includes settings for combo colors, slider appearance, cursor behavior, utility options, menu colors, fonts, and button layouts.


## File Structure

### Note
Most integers you see here are in osu!pixels not your screen resolution 

### ComboColor
Defines the color scheme for the HitCircles.

- **`forceOverride`**: `<boolean>`  
  Forces the specified colors to override per map combo colours.  
  ```json
  {
    "ComboColor": {
      "forceOverride": true
    }
  }
  ```

- **`colors`**: `<array>`  
  List of hex color codes for the hitcircle combo.  
  ```json
  {
    "ComboColor": {
      "colors": ["#F08C8C"]
    }
  }
  ```

### Slider
Customizes the appearance and behavior of sliders.

- **`sliderBorderWidth`**: `<float>`  
  Sets the width of the slider border.  
  ```json
  {
    "Slider": {
      "sliderBorderWidth": 5.2
    }
  }
  ```

- **`sliderBodyBaseAlpha`**: `<float>`  
  Sets the base transparency of the slider body (0.0 to 1.0).  
  ```json
  {
    "Slider": {
      "sliderBodyBaseAlpha": 0.6
    }
  }
  ```

- **`sliderBodyColor`**: `<string>`  
  Hex color code for the slider body.  
  ```json
  {
    "Slider": {
      "sliderBodyColor": "#050B23"
    }
  }
  ```

- **`sliderBorderColor`**: `<string>`  
  Hex color code for the slider border.  
  ```json
  {
    "Slider": {
      "sliderBorderColor": "#7387A0"
    }
  }
  ```

- **`sliderHintEnable`**: `<boolean>`  
  Enables or disables the slider hint.  
  ```json
  {
    "Slider": {
      "sliderHintEnable": true
    }
  }
  ```

- **`sliderHintAlpha`**: `<float>`  
  Sets the transparency of the slider hint (0.0 to 1.0).  
  ```json
  {
    "Slider": {
      "sliderHintAlpha": 0.2
    }
  }
  ```

- **`sliderHintColor`**: `<string>`  
  Hex color code for the slider hint.  
  ```json
  {
    "Slider": {
      "sliderHintColor": "#383838"
    }
  }
  ```

- **`sliderHintShowMinLength`**: `<integer>`  
  Minimum length for showing the slider hint.  
  ```json
  {
    "Slider": {
      "sliderHintShowMinLength": 1
    }
  }
  ```

### Cursor
Controls cursor behavior.

- **`rotateCursor`**: `<boolean>`  
  Enables or disables cursor rotation.  
  ```json
  {
    "Cursor": {
      "rotateCursor": true
    }
  }
  ```

- **`rotateCursorTrail`**: `<boolean>`  
  Enables or disables rotation of the cursor trail.  
  ```json
  {
    "Cursor": {
      "rotateCursorTrail": true 
    }
  }
  ```

### Utils
Miscellaneous utility settings.

- **`limitComboTextLength`**: `<boolean>`  
  Limits the length of combo text.  
  ```json
  {
    "Utils": {
      "limitComboTextLength": true
    }
  }
  ```

- **`comboTextScale`**: `<float>`  
  Scales the size of hitcircle combo text.  
  ```json
  {
    "Utils": {
      "comboTextScale": 0.8
    }
  }
  ```

- **`animationFramerate`**: `<integer>`  
  Sets the framerate for animations(recommended at 60).  
  ```json
  {
    "Utils": {
      "animationFramerate": 60
    }
  }
  ```

- **`layeredHitSounds`**: `<boolean>`  
  Whether hitnormal hitsounds should always be played.
  ```json
  {
    "Utils": {
      "layeredHitSounds": true
    }
  }
  ```

- **`spinnerFrequencyModulate`**: `<boolean>` 
  Whether spinnerspin hitsounds should pitch up as a spinner progresses.
  ```json
  {
    "Utils": {
      "spinnerFrequencyModulate": true
    }
  }
  ```

- **`disableKiai`**: `<boolean>`  
  Disables kiai flashes.  
  ```json
  {
    "Utils": {
      "disableKiai": false
    }
  }
  ```

### Color
Defines color settings for menu items.

- **`MenuItemDefaultColor`**: `<string>`  
  Hex color code for default menu item color.  
  ```json
  {
    "Color": {
      "MenuItemDefaultColor": "#3666A8"
    }
  }
  ```

- **`MenuItemOnTouchColor`**: `<string>`  
  Hex color code for menu item color on touch.  
  ```json
  {
    "Color": {
      "MenuItemOnTouchColor": "#3666A8"
    }
  }
  ```

- **`MenuItemVersionsDefaultColor`**: `<string>`  
  Hex color code for default version menu items.  
  ```json
  {
    "Color": {
      "MenuItemVersionsDefaultColor": "#3666A8"
    }
  }
  ```

- **`MenuItemVersionsSelectedColor`**: `<string>`  
  Hex color code for selected version menu items.  
  ```json
  {
    "Color": {
      "MenuItemVersionsSelectedColor": "#3666A8"
    }
  }
  ```

- **`MenuItemDefaultTextColor`**: `<string>`  
  Hex color code for default menu item text.  
  ```json
  {
    "Color": {
      "MenuItemDefaultTextColor": "#3666A8"
    }
  }
  ```

- **`MenuItemSelectedTextColor`**: `<string>`  
  Hex color code for selected menu item text.  
  ```json
  {
    "Color": {
      "MenuItemSelectedTextColor": "#FFFFFF"
    }
  }
  ```

### Fonts
Configures font settings for gameplay elements.

- **`comboPrefix`**: `<string>`  
  Prefix for combo font.  
  ```json
  {
    "Fonts": {
      "comboPrefix": "combo"
    }
  }
  ```

- **`scorePrefix`**: `<string>`  
  Prefix for score font.  
  ```json
  {
    "Fonts": {
      "scorePrefix": "score"
    }
  }
  ```

- **`hitCirclePrefix`**: `<string>`  
  Prefix for hit circle font.  
  ```json
  {
    "Fonts": {
      "hitCirclePrefix": "default"
    }
  }
  ```

- **`comboOverlap`**: `<integer>`  
  Sets overlap for combo text.  
  ```json
  {
    "Fonts": {
      "comboOverlap": 2
    }
  }
  ```

### Layout
Controls the layout of interface elements.

- **`useNewLayout`**: `<boolean>`  
  Enables the new layout system.  
  ```json
  {
    "Layout": {
      "useNewLayout": true
    }
  }
  ```

- **`BackButton`**: `<object>`  
  Configures the back button layout.  
  - **`w`**: `<integer>` - Width  
  - **`h`**: `<integer>` - Height  
  - **`scale`**: `<float>` - Scale factor  
  - **`x`**: `<integer>` - X position  
  - **`y`**: `<integer>` - Y position  
  ```json
  {
    "Layout": {
      "BackButton": {
        "w": 259,
        "h": 129,
        "scale": 1,
        "x": 0,
        "y": 0
      }
    }
  }
  ```

- **`ModsButton`**: `<object>`  
  Configures the mods button layout.  
  - **`w`**: `<integer>` - Width  
  - **`h`**: `<integer>` - Height  
  - **`scale`**: `<float>` - Scale factor  
  - **`x`**: `<integer>` - X position  
  - **`y`**: `<integer>` - Y position  
  ```json
  {
    "Layout": {
      "ModsButton": {
        "w": 94,
        "h": 129,
        "scale": 1,
        "x": 0,
        "y": 0
      }
    }
  }
  ```

- **`OptionsButton`**: `<object>`  
  Configures the options button layout.  
  - **`w`**: `<integer>` - Width  
  - **`h`**: `<integer>` - Height  
  - **`scale`**: `<float>` - Scale factor  
  - **`x`**: `<integer>` - X position  
  - **`y`**: `<integer>` - Y position  
  ```json
  {
    "Layout": {
      "OptionsButton": {
        "w": 338,
        "h": 402,
        "scale": 0.800000011920929,
        "x": 1010,
        "y": 0
      }
    }
  }
  ```

- **`RandomButton`**: `<object>`  
  Configures the random button layout.  
  - **`w`**: `<integer>` - Width  
  - **`h`**: `<integer>` - Height  
  - **`scale`**: `<float>` - Scale factor  
  - **`x`**: `<integer>` - X position  
  - **`y`**: `<integer>` - Y position  
  ```json
  {
    "Layout": {
      "RandomButton": {
        "w": 94,
        "h": 129,
        "scale": 1,
        "x": 353,
        "y": 0
      }
    }
  }
  ```
  

## Usage
To use skin.json:
1. Use a text editor/ide to make a skin.json or preferably use [Skin.json editor](https://rian8337.github.io/skin-json-editor/) by Rian8337.
2. Place it into your skin's folder(./osu!droid/Skins/your-skin/).
3. Check if everything works
4. Enjoy skinning(in osu!droid :trollhappy:)


## Contributing
Feel free to fork this repository and submit pull requests with improvements and error correction. Thank you!
