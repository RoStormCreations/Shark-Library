# <span style="color:#353fdf; font-family: Arial;">Shark</span> Library
### <span style="color:#353fdf">*Version* **0.1**</span>
##### made by @re_sistance
1. [ Description. ](#desc)
2. [ Usage tips. ](#usage)

<a name="desc"></a>
## 1. Making a window

sometext

<a name="usage"></a>
## 2. Usage tips

sometext
## Booting the Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/RoStormCreations/Shark-Library/refs/heads/main/V01.lua"))()
```
## Making a window
```lua
local Main = Library:Create("Shark","GameNameHere")
```
- Shark: Title of your UI.
- GameNameHere: The name of the game its for.

## Making a tab
```lua
local Preview = Main:CreateSection("Preview")
```

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