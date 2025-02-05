local allowedUsers = {
    ["RIPg5RCUxJaTOT"] = true,
    ["g5RCUxJa"] = true
}

game.Players.PlayerAdded:Connect(function(player)
    if not allowedUsers[player.Name] then
        player:Kick("คุณไม่ได้รับอนุญาตให้รันสคริปต์นี้")
    else
        _G.Key = 'YOUCAN'
        _G.Map  = 'build a boat'

loadstring(game:HttpGet(string.format('https://raw.githubusercontent.com/ADX0017/Build-a-boat-v1.5-BATA-/refs/heads/main/README.md', tostring(game.GameId))))();
    end
end)
