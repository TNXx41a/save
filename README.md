local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("TITLE", "DarkTheme")
local Tab = Window:NewTab("Madu")
local Section = Tab:NewSection("Section Name")
Section:NewButton("ShotCooldown", "ButtonInfo", function()
    print("Clicked")
    _G.YA = true
    while _G.YA do wait()
    game.Players.LocalPlayer.Backpack.BAUBAU.Configuration.RecoilDecay.Value = 0
    game.Players.LocalPlayer.Backpack.groza.Configuration.RecoilDecay.Value = 0
    game.Players.LocalPlayer.Backpack.UMP.Configuration.ShotCooldown.Value = 0
   game.Players.LocalPlayer.Backpack.UMP.Configuration.RecoilDecay.Value = 0
    game.Players.LocalPlayer.Backpack.xwx.Configuration.ShotCooldown.Value = 0
    game.Players.LocalPlayer.Backpack.xwx.Configuration.RecoilDecay.Value = 0
    game.Players.LocalPlayer.Backpack.M1014.Configuration.RecoilDecay = 0
    end
end)
