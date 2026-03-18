--[=[
 d888b  db    db d888888b      .d888b.      db      db    db  .d8b.  
88' Y8b 88    88   `88'        VP  `8D      88      88    88 d8' `8b 
88      88    88    88            odD'      88      88    88 88ooo88 
88  ooo 88    88    88          .88'        88      88    88 88~~~88 
88. ~8~ 88b  d88   .88.        j88.         88booo. 88b  d88 88   88    @uniquadev
 Y888P  ~Y8888P' Y888888P      888888D      Y88888P ~Y8888P' YP   YP  CONVERTER 
]=]

-- Instances: 16 | Scripts: 3 | Modules: 0 | Tags: 0
local G2L = {};

if getgenv().ws then
	getgenv().ws:Close()
	warn("Join Me Is Already Running")
	return
end

-- StarterGui.GameHopper
G2L["1"] = Instance.new("ScreenGui", game.CoreGui);
G2L["1"].ResetOnSpawn = false;
G2L["1"]["Name"] = [[GameHopper]];
G2L["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;


-- StarterGui.GameHopper.Main
G2L["2"] = Instance.new("Frame", G2L["1"]);
G2L["2"]["BorderSizePixel"] = 0;
G2L["2"]["BackgroundColor3"] = Color3.fromRGB(48, 48, 48);
G2L["2"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["2"]["Size"] = UDim2.new(0.31065, 0, 0.35133, 0);
G2L["2"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);
G2L["2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["2"]["Name"] = [[Main]];


-- StarterGui.GameHopper.Main.Bar
G2L["3"] = Instance.new("Frame", G2L["2"]);
G2L["3"]["BorderSizePixel"] = 0;
G2L["3"]["BackgroundColor3"] = Color3.fromRGB(76, 76, 76);
G2L["3"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["3"]["Size"] = UDim2.new(1.0006, 0, 0.10017, 0);
G2L["3"]["Position"] = UDim2.new(0.4997, 0, 0.05508, 0);
G2L["3"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["3"]["Name"] = [[Bar]];


-- StarterGui.GameHopper.Main.Bar.TextLabel
G2L["4"] = Instance.new("TextLabel", G2L["3"]);
G2L["4"]["TextWrapped"] = true;
G2L["4"]["BorderSizePixel"] = 0;
G2L["4"]["TextSize"] = 14;
G2L["4"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["4"]["TextScaled"] = true;
G2L["4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["4"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
G2L["4"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
G2L["4"]["BackgroundTransparency"] = 1;
G2L["4"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["4"]["Size"] = UDim2.new(0.90729, 0, 0.66641, 0);
G2L["4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["4"]["Text"] = [[Join Me by MoonVM]];
G2L["4"]["Position"] = UDim2.new(0.48, 0, 0.5, 0);


-- StarterGui.GameHopper.Main.Game
G2L["5"] = Instance.new("ScrollingFrame", G2L["2"]);
G2L["5"]["Active"] = true;
G2L["5"]["BorderSizePixel"] = 0;
G2L["5"]["TopImage"] = [[rbxasset://textures/ui/Scroll/scroll-middle.png]];
G2L["5"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["5"]["Name"] = [[Game]];
G2L["5"]["BottomImage"] = [[rbxasset://textures/ui/Scroll/scroll-middle.png]];
G2L["5"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["5"]["Size"] = UDim2.new(0.92955, 0, 0.78882, 0);
G2L["5"]["ScrollBarImageColor3"] = Color3.fromRGB(105, 105, 105);
G2L["5"]["Position"] = UDim2.new(0.5, 0, 0.55, 0);
G2L["5"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["5"]["BackgroundTransparency"] = 1;


-- StarterGui.GameHopper.Main.Game.UIGridLayout
G2L["6"] = Instance.new("UIGridLayout", G2L["5"]);
G2L["6"]["CellSize"] = UDim2.new(0, 340, 0, 45);
G2L["6"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


-- StarterGui.GameHopper.Main.Game.Frame
G2L["7"] = Instance.new("Frame", G2L["5"]);
G2L["7"]["BorderSizePixel"] = 0;
G2L["7"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
G2L["7"]["Size"] = UDim2.new(0.08065, 0, 0.15133, 0);
G2L["7"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);


-- StarterGui.GameHopper.Main.Game.Frame.UIListLayout
G2L["8"] = Instance.new("UIListLayout", G2L["7"]);
G2L["8"]["Padding"] = UDim.new(0, 4);
G2L["8"]["VerticalAlignment"] = Enum.VerticalAlignment.Center;
G2L["8"]["SortOrder"] = Enum.SortOrder.LayoutOrder;
G2L["8"]["FillDirection"] = Enum.FillDirection.Horizontal;


-- StarterGui.GameHopper.Main.Game.Frame.PlayerIcon
G2L["9"] = Instance.new("ImageLabel", G2L["7"]);
G2L["9"]["BorderSizePixel"] = 0;
G2L["9"]["BackgroundColor3"] = Color3.fromRGB(40, 40, 40);
-- [ERROR] cannot convert ImageContent, please report to "https://github.com/uniquadev/GuiToLuaConverter/issues"
G2L["9"]["Image"] = [[rbxasset://textures/ui/GuiImagePlaceholder.png]];
G2L["9"]["Size"] = UDim2.new(0.13006, 0, 0.67567, 0);
G2L["9"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["9"]["Name"] = [[PlayerIcon]];
G2L["9"]["Position"] = UDim2.new(0, 0, 0.42433, 0);


-- StarterGui.GameHopper.Main.Game.Frame.PlayerIcon.UIAspectRatioConstraint
G2L["a"] = Instance.new("UIAspectRatioConstraint", G2L["9"]);



-- StarterGui.GameHopper.Main.Game.Frame.UIPadding
G2L["b"] = Instance.new("UIPadding", G2L["7"]);
G2L["b"]["PaddingLeft"] = UDim.new(0, 9);


-- StarterGui.GameHopper.Main.Game.Frame.TextLabel
G2L["c"] = Instance.new("TextLabel", G2L["7"]);
G2L["c"]["TextWrapped"] = true;
G2L["c"]["BorderSizePixel"] = 0;
G2L["c"]["TextSize"] = 14;
G2L["c"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["c"]["TextScaled"] = true;
G2L["c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
G2L["c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
G2L["c"]["BackgroundTransparency"] = 1;
G2L["c"]["Size"] = UDim2.new(0.28244, 0, 0.68783, 0);
G2L["c"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["c"]["Text"] = [[Join ( wow3 ) Currently Playing Tower of goons]];
G2L["c"]["Position"] = UDim2.new(0.10394, 0, 0.18108, 0);


-- StarterGui.GameHopper.Main.Game.Frame.JoinRequest
G2L["d"] = Instance.new("TextButton", G2L["7"]);
G2L["d"]["TextWrapped"] = true;
G2L["d"]["BorderSizePixel"] = 0;
G2L["d"]["TextSize"] = 21;
G2L["d"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
G2L["d"]["BackgroundColor3"] = Color3.fromRGB(255, 56, 59);
G2L["d"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["d"]["Size"] = UDim2.new(0.16129, 0, 0.59283, 0);
G2L["d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["d"]["Text"] = [[Join]];
G2L["d"]["Name"] = [[JoinRequest]];
G2L["d"]["Position"] = UDim2.new(0.77581, 0, 0.40717, 0);


-- StarterGui.GameHopper.Main.Game.LocalScript
G2L["e"] = Instance.new("LocalScript", G2L["5"]);



-- StarterGui.GameHopper.Main.Game.LocalScript
G2L["f"] = Instance.new("LocalScript", G2L["5"]);



-- StarterGui.GameHopper.Main.UIDrag
G2L["10"] = Instance.new("LocalScript", G2L["2"]);
G2L["10"]["Name"] = [[UIDrag]];


-- StarterGui.GameHopper.Main.Game.LocalScript
local function C_e()
	local script = G2L["e"];
	local Frame = script.Parent.Frame
	local ChatHistory = script.Parent
	local Layout = script.Parent.UIGridLayout

	ChatHistory.CanvasSize = UDim2.new(0,0,0,0)

	local function Update()
		ChatHistory.CanvasSize = UDim2.new(0,0,0,Layout.AbsoluteContentSize.Y + 10)
	end

	Layout:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(Update)
end;
task.spawn(C_e);
-- StarterGui.GameHopper.Main.Game.LocalScript
local function C_f()
	local script = G2L["f"];
	local Frame = script.Parent.Frame
	Frame.Visible = false


	local Notice = function(Message, duration)
		game:GetService("StarterGui"):SetCore("SendNotification", {
			Title = "JoinMe",
			Text = Message,
			Duration = duration or 5
		})
	end

	local HttpService = game:GetService("HttpService")
	local Oplayer = game.Players.LocalPlayer
	local OurAPI = "https://text.pollinations.ai/openai"
	local http_func = http_request or request

	local function Prompt(message)
		local Data = {
			Url = OurAPI,
			Method = "POST",
			Headers = {
				["Content-Type"] = "application/json"
			},
			Body = HttpService:JSONEncode({
				messages = {
					{
						role = "user",
						content = message
					}
				}
			})
		}

		local Response = http_func(Data)
		local Decoded = HttpService:JSONDecode(Response.Body)
		return Decoded.choices[1].message.content
	end

	getgenv().ws = WebSocket.connect("wss://free.blr2.piesocket.com/v3/1?api_key=aG7mbYodMgQ518qbD1GkcVoZH40LtSQotd4KeQMO&notify_self=1")

	local Data = {
		["type"] = "join",
		["Game"] = game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name,
		["PlayerName"] = game.Players.LocalPlayer.Name,
		["UserId"] = game.Players.LocalPlayer.UserId,
		["ServerGameLink"] = game.PlaceId
	}

	local Encode = HttpService:JSONEncode(Data)
	ws:Send(Encode)

	ws.OnMessage:Connect(function(msg)
		local Decode = HttpService:JSONDecode(msg)

		local Clone = Frame:Clone()
		Clone.PlayerIcon.Image = "rbxthumb://type=AvatarHeadShot&id="..Decode.UserId.."&w=420&h=420"
		Clone.JoinRequest.Visible = false
		Clone.Parent = script.Parent
		Clone.TextLabel.Text = " please wait while we verify game info !"

		local PromptVerfiy = Prompt(
			"Please Verfiy and Research about this roblox game and verfiy if it is safe then return Yes if not then return No here is the game name "
				.. Decode.Game
		)

		if string.find(string.lower(PromptVerfiy), "yes") then
			Clone.TextLabel.Text = "Join ( "..Decode.PlayerName.." ) Currently Playing -> "..Decode.Game
		elseif string.find(string.lower(PromptVerfiy), "no") then
			Clone.TextLabel.Text = "Join ( "..Decode.PlayerName.." ) Currently Playing -> "..Decode.Game.. " this game wasnt verfied by our system join for your own risk !"
		end

		Clone.JoinRequest.Visible = true

		Clone.JoinRequest.MouseButton1Click:Connect(function()
			local JoinServerURL = "https://www.roblox.com/home?placeId="..Decode.ServerGameLink
			Clone.JoinRequest.Text = "Joining"
			local Success, err = pcall(function()
				game:GetService("TeleportService"):Teleport(Decode.ServerGameLink, Oplayer)
			end)
			if not Success then
				Notice("Executor or Game Doesnt Support Teleporting ! ")
				wait(1)
				Notice("Copied the Server link to your clipboard ")
				SetClipboard(JoinServerURL)
			else
				Notice("Joining Server")
			end
		end)

		Clone.Visible = true
	end)
end;
task.spawn(C_f);
-- StarterGui.GameHopper.Main.UIDrag
local function C_10()
	local script = G2L["10"];
	-- Made by Real_IceyDev (@lceyDex) --
	-- Simple UI dragger (PC Only/Any device that has a mouse) --

	local UIS = game:GetService('UserInputService')
	local frame = script.Parent
	local dragToggle = nil
	local dragSpeed = 0.25
	local dragStart = nil
	local startPos = nil

	local function updateInput(input)
		local delta = input.Position - dragStart
		local position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X,
			startPos.Y.Scale, startPos.Y.Offset + delta.Y)
		game:GetService('TweenService'):Create(frame, TweenInfo.new(dragSpeed), {Position = position}):Play()
	end

	frame.InputBegan:Connect(function(input)
		if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) then 
			dragToggle = true
			dragStart = input.Position
			startPos = frame.Position
			input.Changed:Connect(function()
				if input.UserInputState == Enum.UserInputState.End then
					dragToggle = false
				end
			end)
		end
	end)

	UIS.InputChanged:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
			if dragToggle then
				updateInput(input)
			end
		end
	end)
end;
task.spawn(C_10);

return G2L["1"], require;
