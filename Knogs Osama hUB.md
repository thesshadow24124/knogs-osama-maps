local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Knogs Osama Maps", "BloodTheme")
local function callback(Text)
 if Text == "Button1 text" then
  print ("thanks!")
elseif Text == ("Button2 text") then
 print ("bnork")
 end
end

local NotificationBindable = Instance.new("BindableFunction")
NotificationBindable.OnInvoke = callback
--starter
game.StarterGui:SetCore("SendNotification",  {
 Title = "nort , welcome";
 Text = "don' forget to join our discord made by theshadow24124,oudgsds";
 Icon = "rbxthumb://type=Asset&id=12070397812&w=150&h=150";
 Duration = 22;
 Button1 = "thanks!";
 Button2 = "bnork";
 Callback = NotificationBindable;
})
--
local MapsTab = Window:NewTab("Maps")
local FeScriptTap = Window:NewTab("FE SCRIPT")
local originalscriptTap = Window:NewTab("normal script knogs")
local comingTap = Window:NewTab("coming")

local Section1 = MapsTab:NewSection("maps")

Section1:NewButton("blox fruit & king legacy and more... key", "key", function()
loadstring(game:HttpGet"https://raw.githubusercontent.com/xQuartyx/DonateMe/main/ScriptLoader")()
end)
Section1:NewButton("blox fruit no key", "no key", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/VEZ2/NEVAHUB/main/2'))()
end)
Section1:NewButton("blox fruit & king legacy no key", "no key", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/VEZ2/NEVAHUB/main/2'))()
end)
Section1:NewButton("pet simulator x no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Flxry/Main/MilkyHub/Pet%20Simulator%20X"))()
end)
Section1:NewButton("pet simulator x no key", "no key", function()
loadstring(game:HttpGet("https://milkup.info/script/PetSimulatorX/"))()
end)
Section1:NewButton("cars script it work in all car script key", "key", function()
loadstring(game:HttpGetAsync'https://raw.githubusercontent.com/GXNATION/Main-script/main/Main%20hub')();
end)
Section1:NewButton("bedwars no key", "no key", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/7GrandDadPGN/VapeV4ForRoblox/main/loadstring'))()
end)
Section1:NewButton("arsenal no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/CriShoux/OwlHub/master/OwlHub.txt"))();
end)
Section1:NewButton("Brooken Heven","Brooken Heven",function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/IceMael7/NewIceHub/main/Brookhaven"))()
end)
Section1:NewButton("muder mystery 2 no key", "no key", function()
loadstring(game:HttpGet(('https://raw.githubusercontent.com/Ethanoj1/EclipseMM2/master/Script'),true))()
end)
Section1:NewButton("muder mystery 2 two no key", "no key", function()
local a,b,c,d,e=loadstring,request or http_request or (http and http.request) or (syn and syn.request),assert,tostring,"https://api.eclipsehub.xyz/auth"c(a and b,"Executor not Supported")a(b({Url=e.."\?\107e\121\61"..d(mainKey),Headers={["User-Agent"]="Eclipse"}}).Body)()
end)
Section1:NewButton("granny no key only esp!", "no key", function()
--Granny script
---------------------------->> Customization <<----------------------------

KeyESP = true						EnemyESP = true
ToolESP = true						PlayerESP = false
TrapsESP = true						ExitsESP = true				
EnemyESP = true						InteractsESP = false

-------------------------------->> Code <<--------------------------------
----->> Do not edit below this line unless you know what you're doing <<-----

while wait(1) do -- ESP Loop
	
	local map = ""

	local function updateMap()
		if workspace.Map:FindFirstChild("House") then
			map = "House"
		elseif workspace.Map:FindFirstChild("HouseEz") then
			map = "HouseEz"
		elseif workspace.Map:FindFirstChild("House 2") then
			map = "House 2"
		elseif workspace.Map:FindFirstChild("House 2Ez") then
			map = "House 2Ez"
		elseif workspace.Map:FindFirstChild("House 3") then
			map = "House 3"
		elseif workspace.Map:FindFirstChild("House 3Ez") then
			map = "House 3Ez"
		elseif workspace.Map:FindFirstChild("School") then
			map = "School"
		elseif workspace.Map:FindFirstChild("Ski resort") then
			map = "Ski resort"
		else
			map = ""
		end
	end

	updateMap()
	
	if workspace.Map:FindFirstChild(map) then
		if KeyESP == true then
			for i, key in pairs(workspace.Map[map].Tools.Map:GetChildren()) do -- Key ESP
				if key.Name:find("key") then
					if not key:FindFirstChild("Highlight") then
						local Highlight = Instance.new("Highlight")
						local Billboard = Instance.new("BillboardGui")
						local Name = Instance.new("TextLabel")
						local NameStroke = Instance.new("UIStroke")

						Highlight.FillColor = Color3.fromRGB(255, 170, 0)
						Highlight.OutlineTransparency = 0.9
						Highlight.Parent = key

						Billboard.Parent = key.Handle
						Billboard.ExtentsOffset = Vector3.new(0, 2, 0)
						Billboard.Size = UDim2.new(0, 200, 0, 50)
						Billboard.AlwaysOnTop = true
						Billboard.LightInfluence = 0
						--			keyBillboard.MaxDistance = 50

						Name.Parent = Billboard
						Name.BackgroundTransparency = 1
						Name.TextScaled = true
						Name.Text = key.Name
						Name.TextColor3 = Color3.fromRGB(255, 255, 255)
						Name.Font = Enum.Font.Arial
						Name.Size = UDim2.new(1, 0, 1, 0)

						NameStroke.Parent = Name
						NameStroke.Thickness = 3
					end
				end
			end

		else

			for i, key in pairs(workspace.Map[map].Tools.Map:GetChildren()) do
				if key:FindFirstChild("Highlight") then
					if key.Name:find("key") then
						key.Highlight:Destroy()
						key.Handle.BillboardGui:Destroy()
					end
				end
			end
		end
		if ToolESP == true then
			for i, tool in pairs(workspace.Map[map].Tools.Map:GetChildren()) do -- Tool ESP
				if not tool.Name:find("key") then
					if not tool:FindFirstChild("Highlight") then
						local Highlight = Instance.new("Highlight")
						local Billboard = Instance.new("BillboardGui")
						local Name = Instance.new("TextLabel")
						local NameStroke = Instance.new("UIStroke")

						Highlight.FillColor = Color3.fromRGB(255, 255, 0)
						Highlight.OutlineTransparency = 0.9
						Highlight.Parent = tool

						Billboard.Parent = tool.Handle
						Billboard.ExtentsOffset = Vector3.new(0, 2, 0)
						Billboard.Size = UDim2.new(0, 200, 0, 50)
						Billboard.AlwaysOnTop = true
						Billboard.LightInfluence = 0
						--			keyBillboard.MaxDistance = 50

						Name.Parent = Billboard
						Name.BackgroundTransparency = 1
						Name.TextScaled = true
						Name.Text = tool.Name
						Name.TextColor3 = Color3.fromRGB(255, 255, 255)
						Name.Font = Enum.Font.Arial
						Name.Size = UDim2.new(1, 0, 1, 0)

						NameStroke.Parent = Name
						NameStroke.Thickness = 3
					end
				end
			end

		else

			for i, tool in pairs(workspace.Map[map].Tools.Map:GetChildren()) do
				if tool:FindFirstChild("Highlight") then
					if not tool.Name:find("key") then
						tool.Highlight:Destroy()
						tool.Handle.BillboardGui:Destroy()
					end
				end
			end
		end
		if InteractsESP == true then
			for i, interact in pairs(workspace.Map[map].Interacts:GetChildren()) do -- Interacts ESP
				if not interact:FindFirstChild("Highlight") then
					local Highlight = Instance.new("Highlight")

					Highlight.FillColor = Color3.fromRGB(255, 255, 255)
					Highlight.OutlineTransparency = 0.9
					Highlight.Parent = interact
				end
			end

		else

			for i, interact in pairs(workspace.Map[map].Interacts:GetChildren()) do
				if interact:FindFirstChild("Highlight") then
					interact.Highlight:Destroy()
				end
			end		

		end
		if TrapsESP == true then
			for i, trap in pairs(workspace.Map.Traps:GetChildren()) do -- Traps ESP
				if not trap:FindFirstChild("Highlight") then
					local Highlight = Instance.new("Highlight")
					local Billboard = Instance.new("BillboardGui")
					local Name = Instance.new("TextLabel")
					local NameStroke = Instance.new("UIStroke")

					Highlight.FillColor = Color3.fromRGB(255, 0, 0)
					Highlight.OutlineTransparency = 0.9
					Highlight.Parent = trap

					Billboard.Parent = trap.Base
					Billboard.ExtentsOffset = Vector3.new(0, 2, 0)
					Billboard.Size = UDim2.new(0, 200, 0, 50)
					Billboard.AlwaysOnTop = true
					Billboard.LightInfluence = 0
					--			keyBillboard.MaxDistance = 50

					Name.Parent = Billboard
					Name.BackgroundTransparency = 1
					Name.TextScaled = true
					Name.Text = trap.Name
					Name.TextColor3 = Color3.fromRGB(255, 0, 0)
					Name.Font = Enum.Font.Arial
					Name.Size = UDim2.new(1, 0, 1, 0)

					NameStroke.Parent = Name
					NameStroke.Thickness = 3
				end
			end

		else

			for i, trap in pairs(workspace.Map.Traps:GetChildren()) do
				if trap:FindFirstChild("Highlight") then
					trap.Highlight:Destroy()
					trap.Base.BillboardGui:Destroy()
				end
			end

		end
		if EnemyESP == true then
			if workspace.Map.Players:FindFirstChild("Enemy") then -- Enemy ESP
				if not workspace.Map.Players.Enemy:FindFirstChild("Highlight") then
					local Highlight = Instance.new("Highlight")
					local Billboard = Instance.new("BillboardGui")
					local Name = Instance.new("TextLabel")
					local NameStroke = Instance.new("UIStroke")

					Highlight.FillColor = Color3.fromRGB(255, 0, 0)
					Highlight.OutlineTransparency = 0.9
					Highlight.Parent = workspace.Map.Players.Enemy

					Billboard.Parent = workspace.Map.Players.Enemy.HumanoidRootPart
					Billboard.ExtentsOffset = Vector3.new(0, 2, 0)
					Billboard.Size = UDim2.new(0, 200, 0, 50)
					Billboard.AlwaysOnTop = true
					Billboard.LightInfluence = 0
					--			keyBillboard.MaxDistance = 50

					Name.Parent = Billboard
					Name.BackgroundTransparency = 1
					Name.TextScaled = true
					Name.Text = workspace.Map.Players.Enemy.Name
					Name.TextColor3 = Color3.fromRGB(255, 0, 0)
					Name.Font = Enum.Font.Arial
					Name.Size = UDim2.new(1, 0, 1, 0)

					NameStroke.Parent = Name
					NameStroke.Thickness = 3
				end
			end

		else

			if workspace.Map.Players:FindFirstChild("Enemy") then
				if workspace.Map.Players.Enemy:FindFirstChild("Highlight") then
					workspace.Map.Players.Enemy.Highlight:Destroy()
				end			
			end		
		end	
		if PlayerESP == true then
			for i, player in pairs(workspace.Map.Players:GetChildren()) do -- Player ESP
					if not player:FindFirstChild("Highlight") then
						local Highlight = Instance.new("Highlight")
						local Billboard = Instance.new("BillboardGui")
						local Name = Instance.new("TextLabel")
						local NameStroke = Instance.new("UIStroke")

						Highlight.FillColor = Color3.fromRGB(0, 170, 0)
						Highlight.OutlineTransparency = 0.9
						Highlight.Parent = player
						Billboard.Parent = player.HumanoidRootPart
						Billboard.ExtentsOffset = Vector3.new(0, 2, 0)
						Billboard.Size = UDim2.new(0, 200, 0, 50)
						Billboard.AlwaysOnTop = true
						Billboard.LightInfluence = 0
						--			keyBillboard.MaxDistance = 50

						Name.Parent = Billboard
						Name.BackgroundTransparency = 1
						Name.TextScaled = true
						Name.Text = player.Name
						Name.TextColor3 = Color3.fromRGB(0, 170, 0)
						Name.Font = Enum.Font.Arial
						Name.Size = UDim2.new(1, 0, 1, 0)

						NameStroke.Parent = Name
						NameStroke.Thickness = 3						
					end
				end

		else

			for i, player in pairs(workspace.Map.Players:GetChildren()) do
				if player:FindFirstChild("Highlight") then
					if not player.Name == "Enemy" then
						player.Highlight:Destroy()						
					end
				end			
			end		
		end	
		if TrapsESP == true then
			for i, exit in pairs(workspace.Map[map].WinPath:GetChildren()) do -- Exits ESP
				if not exit:FindFirstChild("Highlight") then
					local Highlight = Instance.new("Highlight")
					local Billboard = Instance.new("BillboardGui")
					local Name = Instance.new("TextLabel")
					local NameStroke = Instance.new("UIStroke")

					Highlight.FillColor = Color3.fromRGB(0, 255, 255)
					Highlight.OutlineTransparency = 0.9
					Highlight.Parent = exit

					Billboard.Parent = exit
					Billboard.ExtentsOffset = Vector3.new(0, 0, 0)
					Billboard.Size = UDim2.new(0, 200, 0, 50)
					Billboard.AlwaysOnTop = true
					Billboard.LightInfluence = 0
					--			keyBillboard.MaxDistance = 50

					Name.Parent = Billboard
					Name.BackgroundTransparency = 1
					Name.TextScaled = true
					Name.Text = exit.Name
					Name.TextColor3 = Color3.fromRGB(0, 255, 255)
					Name.Font = Enum.Font.Arial
					Name.Size = UDim2.new(1, 0, 1, 0)

					NameStroke.Parent = Name
					NameStroke.Thickness = 3
				end
			end

		else

			for i, exit in pairs(workspace.Map[map].WinPath:GetChildren()) do
				if exit:FindFirstChild("Highlight") then
					exit.Highlight:Destroy()
					exit.Base.BillboardGui:Destroy()
				end
			end

		end
	end
end
end)
Section1:NewButton("da hood no key", "no key", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/Scrvpter/Pluto/Lua/Loader.Lua', true))()
end)
Section1:NewButton("sharkbite 1 no key ban risk inf money", "no key", function()
loadstring(game:GetObjects("rbxassetid://3623753581")[1].Source)()
end)
Section1:NewButton("sharkbite 2 no key", "no key", function()
loadstring(game:HttpGet(('https://gist.githubusercontent.com/insuretya/13f489df942aa47cef31b3f86388d6f3/raw/cbdf238ed0c20786ac438296367ccf66a886c6da/sharkbite%2520cool.lua')))()
end)
Section1:NewButton("jailbreak no key don't let anyone see you", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/KuriWasTaken/MonkeyScripts/main/JailMonkey.lua"))()
end)
Section1:NewButton("doors no key don't let anyone see you", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Vynixius/main/Doors/Script.lua"))()
end)
Section1:NewButton("build a boat no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Vynixius/main/Build%20A%20Boat%20For%20Treasure/Script.lua"))()
end)
Section1:NewButton("piggy no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Vynixius/main/Piggy/Piggy"))()
end)
Section1:NewButton("works in all maps no key", "no key", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/1201for/V.G-Hub/main/V.Ghub'))()
end)
Section1:NewButton("Combat Warriors  no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/1f0yt/community/master/flare"))()
end)
Section1:NewButton("Combat Warriors 2 no key", "no key", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/frkfx/Combat-Warriors/main/Script"))();
end)
Section1:NewButton("tps football no key", "no key", function()

end)

local Section2 = FeScriptTap:NewSection("Fe Script On Knogs Osama first open knogs osama")

Section2:NewButton("FEYZ", "Knogs Osama Hub", function()
loadstring(game:HttpGet("https://pastebin.com/raw/bzmhRgKL"))();
end)
Section2:NewButton("Interaxis hub", "Knogs Osama Hub", function()
loadstring(game:HttpGet("https://pastebin.com/raw/bzmhRgKL"))();
end)
Section2:NewButton("Pendulum Hubs", "Knogs Osama Hub", function()
loadstring(game:HttpGet("https://pastebin.com/raw/bzmhRgKL"))();
end)

local Section3 = originalscriptTap:NewSection("Knogs Osama Hub and Version")

Section3:NewButton("Knogs Osama Hub", "Knogs Osama Hub", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
end)
Section3:NewButton("Knogs Osama Hub ??", "Knogs Osama Hub ??", function()

end)
