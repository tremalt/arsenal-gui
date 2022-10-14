local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Arsenal gui", "Sentinel")
--Player
local Player = Window:NewTab("Player")
local PlayerSection = Player:NewSection("Player")

PlayerSection:NewSlider("Walk speed", "makes u walk more fast", 500, 16, function(s) -- 500 (MaxValue) | 16 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

PlayerSection:NewSlider("Jumppower", "makes u jump more high", 350, 50, function(s) -- 350 (MaxValue) | 50 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

PlayerSection:NewButton("God Mode", "God Mode", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/trem2goated/god-mode-/main/README.md'))()
end)

PlayerSection:NewButton("God Mode", "God Mode", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/trem2goated/god-mode-/main/README.md'))()
end)

--MAIN
local Main = Window:NewTab("Main")
local MainSection = Main:NewSection("Main")

MainSection:NewButton("aimbot", "aimbot", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/UhtQSzgP'))()
end)

MainSection:NewButton("Esp", "Esp", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/trem2goated/new-esp./main/README.md'))()
end)
