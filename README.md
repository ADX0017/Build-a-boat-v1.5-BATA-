local TweenService = game:GetService("TweenService")
local player = game.Players.LocalPlayer
local flightTime = 40

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
