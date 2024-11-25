# <span style="color:#353fdf; font-family: Arial;">Shark</span> Library
---
### <span style="color:#353fdf">*Version* **0.1**</span>
##### made by @re_sistance


<!-- Table of Contents -->

---
### *Contents*
##### | [ Booting the library ](#LibrarySection)
##### | [ Making A Window ](#TabSection)
##### | [ **Code Example** ](#Example)
---


<!-- Library Section-->

<a name="LibrarySection"></a>

## Booting the Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/RoStormCreations/Shark-Library/refs/heads/main/V01.lua"))()
```


<!-- Window Section -->

## Making a window
```lua
local Main = Library:Create("Shark","GameNameHere")
```

```
Shark: Title of your UI.
GameNameHere: The name of the game its for.
```


<!-- Tab Section -->

## Making a tab
```lua
local Preview = Main:CreateSection("Preview")
```


<!-- Example Section -->

## Example
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/RoStormCreations/Shark-Library/refs/heads/main/V01.lua"))()
local Main = Library:Create("Shark","Fisch")

local Other = Main:CreateSection("Other")
local Preview = Main:CreateSection("Preview")

Preview:CreateLabel("Text Label")
Preview:CreateButton("Button Text", "Button Info", function()
    print("Wow, printed")
end)
Preview:CreateToggle("Toggle Info", function(state)
    print(state)
end)
Preview:CreateBind("Keybind Info", Enum.KeyCode.F, function()
    print("Keybind Was Pressed")
end)
Preview:CreateTextBox("TextBox Info", "PlaceHolder", function(v)
print(v) 
end)
Preview:CreateSlider(16, 500, "Slider Info", function(val)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = val
end)
```