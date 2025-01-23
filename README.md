local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("ADX SCRPIT", "DarkTheme")
local Tab = Window:NewTab("Teleport ")
local Section = Tab:NewSection("Teleport team")
Section:NewButton("Green", "Green", function()
    local targetPosition = Vector3.new(-493.9684143066406, 17.96377182006836, 294.43988037109375)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
Section:NewButton("Blue", "Blue", function()
    local targetPosition = Vector3.new(404.459716796875, 18.21242904663086, 297.99072265625)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
Section:NewButton("Black", "Black", function()
    local targetPosition = Vector3.new(-496.7078857421875, 13.32424259185791, -59.68553161621094)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
Section:NewButton("yellow", "yellow", function()
    local targetPosition = Vector3.new(-503.6094055175781, 34.503814697265625, 640.1946411132812)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
Section:NewButton("while", "while", function()
    local targetPosition = Vector3.new(-52.48784637451172, -3.002993106842041, -502.1974792480469)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
Section:NewButton("magenta", "magenta", function()
    local targetPosition = Vector3.new(397.8524169921875, 33.60623550415039, 646.2332763671875)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)

local plr = game.Players.LocalPlayer

local Tab = Window:NewTab("Fram")
local Section = Tab:NewSection("Fram")
Section:NewButton("Nope", "Nope", function()
    plr.health = 0
end)
local Section = Tab:NewSection("Click to Fram")
Section:NewButton("fram", "fram", function()
    local TweenService = game:GetService("TweenService")
local player = game.Players.LocalPlayer
local flightTime = 45

local function flyToPosition(targetPosition)
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        local humanoidRootPart = player.Character.HumanoidRootPart
        local tweenInfo = TweenInfo.new(flightTime, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut)
        local goal = { CFrame = CFrame.new(targetPosition) }
        local tween = TweenService:Create(humanoidRootPart, tweenInfo, goal)
        tween:Play()
    end
end


local startPosition = Vector3.new(-68.53434753417969, 92.35619354248047, -272.0222473144531)
local endPosition = Vector3.new(-55.7065125, 80.739624, 8492.35645, 0, 0, -1, 0, 1, 0, 1, 0, 0)

if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
    player.Character.HumanoidRootPart.CFrame = CFrame.new(startPosition)
end

flyToPosition(endPosition)

wait(1)
local targetPosition = Vector3.new(-55.7065125, -315.739624, 9492.35645, 0, 0, -1, 0, 1, 0, 1, 0, 0)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
if character and character:FindFirstChild("HumanoidRootPart") then
    character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
end
end)
