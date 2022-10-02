if game.PlaceId == 10492057600 then
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "RAISE A SILLY CAT CUSTON SOUND!!!!", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})


local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})


local Section = Tab:AddSection({
	Name = "Section"
})



Tab:AddButton({
	Name = "COBRA SONG",
	Callback = function()
      		print("button pressed")
local args = {
    [1] = {
        ["Name"] = "hi",
        ["Description"] = "GAME!",
        ["Icon"] = "rbxassetid://10539319122",
        ["Artist"] = "by bot",
        ["Sound"] = "rbxassetid://5410081008"
    }
}

game:GetService("ReplicatedStorage").Events.changeSong:FireServer(unpack(args))

  	end    
})

Tab:AddButton({
	Name = "I'm gonna getcha! I am GOD!",
	Callback = function()
      		print("button pressed")
local args = {
    [1] = {
        ["Name"] = "hi",
        ["Description"] = "GAME!",
        ["Icon"] = "rbxassetid://10539319122",
        ["Artist"] = "by bot",
        ["Sound"] = "rbxassetid://8502101489"
    }
}

game:GetService("ReplicatedStorage").Events.changeSong:FireServer(unpack(args))

  	end    
})


OrionLib:Init()
