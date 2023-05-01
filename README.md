if game:GetService("CoreGui"):FindFirstChild("VERY HUB") then
  game:GetService("CoreGui"):FindFirstChild("VERY HUB"):Destroy()
end)
local UILib = loadstring(game:HttpGet('https://pastebin.com/raw/zj1Zd78z'))()

local win = UILib:Window("VERY HUB",Color3.fromRGB(44, 120, 224), Enum.KeyCode.RightControl)
local MainSection = win:Tab("Main")

MainSection:Button("auto", function()

end)

MainSection:Toggle("Farm",false, function(State)

end)

MainSection:Dropdown("Dropdown 1", {"1","2","3"}, function(String)

end)
MainSection:Slider("Slider",0,100,16,true, function(State)
    
end)

local Settings = win:Tab("Settings")
Settings:Label("UI Toggle Key:  Right-Ctrl")
Settings:Label("Credit : Paet")
Settings:Button("Copy Discord Invite", function()
    setclipboard("https://discord.gg/dY8rpSktyn")
    UILib:Notification("Notification", "Copied!", "Okay")
end)
Settings:Button("Copy Youtube", function()
   setclipboard("https://www.youtube.com/channel/UCpbG2pkTiPODfMOq_voRQDg/videos")
   UILib:Notification("Notification", "Copied!", "Okay")
end)
