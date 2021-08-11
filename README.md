
local ScreenGui = Instance.new("ScreenGui")
local LoginFrame = Instance.new("Frame")
local LoginTitle = Instance.new("TextLabel")
local username = Instance.new("TextBox")
local password = Instance.new("TextBox")
local Login = Instance.new("TextButton")
local main = Instance.new("Frame")
local label = Instance.new("TextLabel")
local Btools = Instance.new("TextButton")
local script2 = Instance.new("TextButton")
local gamez = Instance.new("TextButton")
local guiframe = Instance.new("Frame")
local labelgui = Instance.new("TextLabel")
local pfbutton = Instance.new("TextButton")
local proxl = Instance.new("TextButton")
local prisongui = Instance.new("TextButton")
local jailbreakgui = Instance.new("TextButton")
local goback = Instance.new("TextButton")


ScreenGui.Parent = game.CoreGui

LoginFrame.Name = "LoginFrame"
LoginFrame.Parent = ScreenGui
LoginFrame.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
LoginFrame.Position = UDim2.new(0.109895863, 0, 0.224074081, 0)
LoginFrame.Size = UDim2.new(0, 309, 0, 433)
LoginFrame.Active = true
LoginFrame.Draggable = true

LoginTitle.Name = "Login Title"
LoginTitle.Parent = LoginFrame
LoginTitle.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
LoginTitle.Size = UDim2.new(0, 309, 0, 50)
LoginTitle.Font = Enum.Font.SourceSans
LoginTitle.Text = "LOGIN"
LoginTitle.TextColor3 = Color3.fromRGB(213, 213, 213)
LoginTitle.TextScaled = true
LoginTitle.TextSize = 14.000
LoginTitle.TextWrapped = true

username.Name = "username"
username.Parent = LoginFrame
username.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
username.Position = UDim2.new(0.127721205, 0, 0.267898381, 0)
username.Size = UDim2.new(0, 229, 0, 50)
username.Font = Enum.Font.SourceSans
username.Text = "USERNAME"
username.TextColor3 = Color3.fromRGB(213, 213, 213)
username.TextScaled = true
username.TextSize = 14.000
username.TextWrapped = true

password.Name = "password"
password.Parent = LoginFrame
password.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
password.Position = UDim2.new(0.127721205, 0, 0.487297922, 0)
password.Size = UDim2.new(0, 230, 0, 50)
password.Font = Enum.Font.SourceSans
password.Text = "PASSWORD"
password.TextColor3 = Color3.fromRGB(213, 213, 213)
password.TextScaled = true
password.TextSize = 14.000
password.TextWrapped = true

Login.Name = "Login"
Login.Parent = LoginFrame
Login.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
Login.Position = UDim2.new(0.174757287, 0, 0.775981545, 0)
Login.Size = UDim2.new(0, 200, 0, 50)
Login.Font = Enum.Font.SourceSans
Login.Text = "LOGIN "
Login.TextColor3 = Color3.fromRGB(213, 213, 213)
Login.TextScaled = true
Login.TextSize = 14.000
Login.TextWrapped = true
Login.MouseButton1Down:connect(function()
	if username.Text == "Em_illys" and password.Text == "v1ishere" then 
		LoginFrame.Visible = false
		main.Visible = true
		guiframe.Visible = false
	end
end)

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
main.Position = UDim2.new(0.330208302, 0, 0.224074081, 0)
main.Size = UDim2.new(0, 726, 0, 360)
main.Visible = false
main.Active = true
main.Draggable = true

label.Name = "label"
label.Parent = main
label.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
label.Size = UDim2.new(0, 726, 0, 50)
label.Font = Enum.Font.SourceSans
label.Text = "Flare Admin v1 | made by Em_illys"
label.TextColor3 = Color3.fromRGB(255, 255, 255)
label.TextScaled = true
label.TextSize = 14.000
label.TextWrapped = true

Btools.Name = "Btools"
Btools.Parent = main
Btools.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
Btools.Position = UDim2.new(0.0330578499, 0, 0.213888884, 0)
Btools.Size = UDim2.new(0, 200, 0, 50)
Btools.Font = Enum.Font.SourceSans
Btools.Text = "BTOOLS"
Btools.TextColor3 = Color3.fromRGB(0, 0, 0)
Btools.TextScaled = true
Btools.TextSize = 14.000
Btools.TextWrapped = true
Btools.MouseButton1Down:connect(function()
	local tool1 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
	local tool2 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
	local tool3 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
	local tool4 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
	local tool5 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
	tool1.BinType = "Clone"
	tool2.BinType = "GameTool"
	tool3.BinType = "Hammer"
	tool4.BinType = "Script"
	tool5.BinType = "Grab"
end)

script2.Name = "script2"
script2.Parent = main
script2.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
script2.Position = UDim2.new(0.345730066, 0, 0.213888884, 0)
script2.Size = UDim2.new(0, 200, 0, 50)
script2.Font = Enum.Font.SourceSans
script2.Text = "CLICK T TO TP"
script2.TextColor3 = Color3.fromRGB(0, 0, 0)
script2.TextScaled = true
script2.TextSize = 14.000
script2.TextWrapped = true
script2.MouseButton1Down:connect(function()
	plr = game.Players.LocalPlayer

	hum = plr.Character.HumanoidRootPart

	mouse = plr:GetMouse()



	mouse.KeyDown:connect(function(key)

		if key == "t" then

			if mouse.Target then

				hum.CFrame = CFrame.new(mouse.Hit.x, mouse.Hit.y + 5, mouse.Hit.z)

			end

		end
	end)
end)

gamez.Name = "gamez"
gamez.Parent = main
gamez.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
gamez.Position = UDim2.new(0.0275482927, 0, 0.758333325, 0)
gamez.Size = UDim2.new(0, 681, 0, 50)
gamez.Font = Enum.Font.SourceSans
gamez.Text = "Game Script GUI"
gamez.TextColor3 = Color3.fromRGB(0, 0, 0)
gamez.TextScaled = true
gamez.TextSize = 14.000
gamez.TextWrapped = true
gamez.MouseButton1Down:connect(function()
	main.Visible = false
	guiframe.Visible = true
end)

guiframe.Name = "guiframe"
guiframe.Parent = ScreenGui
guiframe.BackgroundColor3 = Color3.fromRGB(48, 48, 48)
guiframe.Position = UDim2.new(0, 633, 0, 628)
guiframe.Size = UDim2.new(0, 301, 0, 388)
guiframe.Visible = false
guiframe.Active = true
guiframe.Draggable = true

labelgui.Name = "labelgui"
labelgui.Parent = guiframe
labelgui.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
labelgui.Size = UDim2.new(0, 301, 0, 50)
labelgui.Font = Enum.Font.SourceSans
labelgui.Text = "GUIS"
labelgui.TextColor3 = Color3.fromRGB(213, 213, 213)
labelgui.TextScaled = true
labelgui.TextSize = 14.000
labelgui.TextWrapped = true

pfbutton.Name = "pfbutton"
pfbutton.Parent = guiframe
pfbutton.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
pfbutton.Position = UDim2.new(0, 50, 0, 66)
pfbutton.Size = UDim2.new(0, 200, 0, 50)
pfbutton.Font = Enum.Font.SourceSans
pfbutton.Text = "Phantom Forces"
pfbutton.TextColor3 = Color3.fromRGB(0, 0, 0)
pfbutton.TextScaled = true
pfbutton.TextSize = 14.000
pfbutton.TextWrapped = true
pfbutton.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://bruh.keshsenpai.com/.lua"))()
end)

proxl.Name = "proxl"
proxl.Parent = guiframe
proxl.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
proxl.Position = UDim2.new(0, 50, 0, 140)
proxl.Size = UDim2.new(0, 200, 0, 50)
proxl.Font = Enum.Font.SourceSans
proxl.Text = "Project XL"
proxl.TextColor3 = Color3.fromRGB(0, 0, 0)
proxl.TextScaled = true
proxl.TextSize = 14.000
proxl.TextWrapped = true
proxl.MouseButton1Down:connect(function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/10540475/legogamestuff/main/projectxl'))()
end)

prisongui.Name = "prisongui"
prisongui.Parent = guiframe
prisongui.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
prisongui.Position = UDim2.new(0, 50, 0, 215)
prisongui.Size = UDim2.new(0, 200, 0, 50)
prisongui.Font = Enum.Font.SourceSans
prisongui.Text = "Prison Life"
prisongui.TextColor3 = Color3.fromRGB(0, 0, 0)
prisongui.TextScaled = true
prisongui.TextSize = 14.000
prisongui.TextWrapped = true
prisongui.MouseButton1Down:connect(function()
	loadstring(game:HttpGet(("https://raw.githubusercontent.com/i1nfinity/Project-X/master/Prison%20Breaker%20X"), true))()
end)

jailbreakgui.Name = "jailbreakgui"
jailbreakgui.Parent = guiframe
jailbreakgui.BackgroundColor3 = Color3.fromRGB(122, 122, 122)
jailbreakgui.Position = UDim2.new(0, 50, 0, 290)
jailbreakgui.Size = UDim2.new(0, 200, 0, 50)
jailbreakgui.Font = Enum.Font.SourceSans
jailbreakgui.Text = "Jail Break"
jailbreakgui.TextColor3 = Color3.fromRGB(0, 0, 0)
jailbreakgui.TextScaled = true
jailbreakgui.TextSize = 14.000
jailbreakgui.TextWrapped = true
jailbreakgui.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/opBandwidth/Magma-Core/main/Jailbreak/Main.lua"))()
end)

goback.Name = "goback"
goback.Parent = guiframe
goback.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
goback.Position = UDim2.new(0, 0, 0, 362)
goback.Size = UDim2.new(0, 301, 0, 26)
goback.Font = Enum.Font.SourceSans
goback.Text = "GO BACK"
goback.TextColor3 = Color3.fromRGB(213, 213, 213)
goback.TextScaled = true
goback.TextSize = 14.000
goback.TextWrapped = true
goback.MouseButton1Down:connect(function()
	guiframe.Visible = false
	main.Visible = true
end)
