local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("LENOVO", "DarkTheme")
local Tab = Window:NewTab("Madu")
local Section = Tab:NewSection("Section Name")
Section:NewButton("Tp Item", "ButtonInfo", function()
    print("Clicked")
  _G.loop = true
  while _G.loop do wait()
    for i,v in pairs(game:GetService("Workspace").Items:GetDescendants()) do
        if v.Name == "TouchInterest" then
         game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
        end
    end
 end
end)
Section:NewButton("Stop", "ButtonInfo", function()
    print("Clicked")
     _G.loop = false
  while _G.loop do wait()
end
end)
