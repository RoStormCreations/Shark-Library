# <span style="color:#353fdf; font-family: Arial;">Shark</span> Library
---
### <span style="color:#353fdf">*Version* **0.1**</span>
##### made by @re_sistance


<!-- Table of Contents -->

---
### *Contents*
##### | [ Loading the library ](#LibrarySection)
##### | [ Adding a frame ](#WindowSection)
##### | [ Adding a tab ](#TabSection)
##### | [ **Code Example** ](#ExampleSection)
---


<!-- Library Section-->

<a name="LibrarySection"></a>

## Booting the Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/RoStormCreations/Shark-Library/refs/heads/main/V01.lua"))()
```


<!-- Window Section -->

<a name="WindowSection"></a>

## Making a window
```lua
local Main = Library:Create("Shark","GameNameHere")
```

 - "Shark" = Title.
 - "GameNameHere" = Name of the game.

<!-- Tab Section -->

<a name="TabSection"></a>

## Making a tab
```lua
local Preview = Main:CreateSection("Preview")
```
 - Preview = Name of the tab.


<!-- Label Section -->

<a name="LabelSection"></a>

## Adding a label
```lua
Preview:CreateLabel("Text Label")
```


<!-- Button Section -->

<a name="ButtonSection"></a>

## Adding a button
```lua
Preview:CreateButton("Button Text", "Button Info", function()
    print("Wow, printed")
end)
```



<!-- Toggle Section -->

<a name="ToggleSection"></a>

## Adding a toggle
```lua
Preview:CreateToggle("Toggle Info", function(state)
    print(state)
end)
```


<!-- KeyBind Section -->

<a name="KeyBindSection"></a>

## Adding a keybind
```lua
Preview:CreateBind("Keybind Info", Enum.KeyCode.F, function()
    print("Keybind Was Pressed")
end)
```



<!-- TextBox Section -->

<a name="TextBoxSection"></a>

## Adding a TextBox
```lua
Preview:CreateTextBox("TextBox Info", "PlaceHolder", function(v)
print(v) 
end)
```




<!-- Slider Section -->

<a name="SliderSection"></a>

## Adding a slider / **(Walkspeed Example)**
```lua
Preview:CreateSlider(16, 500, "Slider Info", function(val)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = val
end)
```




<!-- Example Section -->

<a name="ExampleSection"></a>

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