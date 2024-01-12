#FreeFedox on helix discord

![Helix Snippets Preview](images/helix-preview.gif)

![Helix Snippets Preview](images/helix-logo.png
)
# Helix Snippets Extension

## Overview

The Helix Snippets extension provides a set of code snippets for the Helix programming language. Easily insert common code patterns and improve your development efficiency with this Visual Studio Code extension.

## Features

- **Snippet Library:** A collection of useful snippets for Helix development.
- **Easy Insertion:** Quickly insert code snippets with just a few keystrokes.
- **Visual Studio Code Integration:** Seamlessly integrates with Visual Studio Code for a smooth coding experience.

## Usage

1. Install the Helix Snippets extension from the Visual Studio Code Marketplace.
2. Open a LUA file.
3. Type the snippet prefix and press `Tab` to insert the snippet.

## Contributors

1. Fedox (Started project)
2. Winkarst (Added fcking lot stuff into it)

## Snippet Examples

### helix.plugin

```lua
local PLUGIN = PLUGIN

PLUGIN.name = "NAME"
PLUGIN.description = "DESCRIPTION"
PLUGIN.author = "AUTHOR"
PLUGIN.schema = "SCHEMA"
```

### helix.item

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.price = 1
ITEM.category = "CategoryName"
ITEM.noBusiness = false
ITEM.factions = {"faction1", "faction2"}
ITEM.classes = {"class1", "class2"}
ITEM.flag = "flags"

ITEM.iconCam = {pos = Vector(0, 0, 0), ang = Angle(0, 0, 0), fov = 70}

ITEM.functions.Option = {
    name = "OptionName",
    OnClick = function(item)
        -- OnClick functionality here
    end,
    OnRun = function(item)
        -- OnRun functionality here
        return false
    end,
    OnCanRun = function(item)
        -- OnCanRun checks here
    end,
}

function ITEM:GetName()
    return self.name
end

function ITEM:GetDescription()
    return self.description
end
```

### helix.item.outfit

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.outfitCategory = "CATEGORY"
ITEM.newSkin = 1
ITEM.bodyGroups = {
    ["BODYGROUPNAME"] = 1,
}
ITEM.replacements = "MODEL"
```

### helix.item.pacoutfit

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.outfitCategory = "CATEGORY"
ITEM.pacData = {}
```

### helix.item.bag

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.invWidth = 1
ITEM.invHeight = 1
```

### helix.item.ammo

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.ammo = "AMMO"
ITEM.ammoAmount = 1
```

### helix.item.weapon

```lua
ITEM.name = "NAME"
ITEM.description = "DESCRIPTION"
ITEM.model = "MODEL"
ITEM.width = 1
ITEM.height = 1
ITEM.class = "WEAPONCLASS"
ITEM.weaponCategory = "CATEGORY"
```
