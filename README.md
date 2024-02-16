local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Stouks X [Versão Premium]", HidePremium = false, SaveConfig = false, ConfigFolder = "Blade Ball","Ninja Legends"})
local Tab = Window:MakeTab({
	Name = "Farm",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

OrionLib:MakeNotification({
	Name = "Script Blade Ball",
	Content = "Oi CuzCuz com Ovo:D",
	Image = "rbxassetid://4483345998",
	Time = 5
})

Tab:AddButton({
	Name = "Auto Farm",
	Callback = function()
      		print("button pressed")                 while true do
wait(0.0001)
game:GetService("ReplicatedStorage"):WaitForChild("RemoteEvents"):WaitForChild("GeneralAttack"):FireServer()
end
  	end    
})
OrionLib:Init()
