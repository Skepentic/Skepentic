local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
    Name = "JingJok Hub",
    LoadingTitle = "JingJok Tom Ler JengJeng",
    LoadingSubtitle = "Kdor300cm",
    ConfigurationSaving = {
       Enabled = true,
       FileName = "GayScriptLol"
    },
    Discord = {
       Enabled = false,
       Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
       RememberJoins = false -- Set this to false to make them join the discord every time they load it up
    },
    KeySystem = false, -- Set this to true to use our key system
    KeySettings = {
       Title = "Untitled",
       Subtitle = "Key System",
       Note = "No method of obtaining the key is provided",
       FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
       SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
       GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
       Key = {"Hello"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
    }
 })


--value

_G.Kill_Aura = true

--Functions
function Awakeningexpert()
    local args = {
        [1] = "AwakeningChanger",
        [2] = "Check"
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki5()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 5
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki4()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 4
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki3()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 3
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki2()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 2
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki1()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 1
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Busohaki0()
    local args = {
        [1] = "ChangeBusoStage",
        [2] = 0
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Statrefund()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","1")
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","2")
end

function TitleGui()
    local args = {
        [1] = "getTitles"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end

function ColorGui()
    game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end
  

function Kill_Aura()
    spawn(function()
        while wait() do
            if _G.Kill_Aura then
                for i,v in pairs(game.Workspace.Enemies:GetDescendants()) do
                    if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                        pcall(function()
                            repeat wait(.1)
                                v.Humanoid.Health = 0
                                v.HumanoidRootPart.CanCollide = false
                                sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                            until not _G.Kill_Aura  or not v.Parent or v.Humanoid.Health <= 0
                        end)
                    end
                end
            end
        end
    end)
end
                
function Devilfruitshop()
    local args = {
        [1] = "GetFruits"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
end

function Rollfruit()
    local args = {
        [1] = "Cousin",
        [2] = "Buy"
    }
    
    game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
end

function Pirateteam()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam","Pirates")
end
    
function Marineteam()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam","Marines")
end
    
function Godhuman()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman")
end

function SuperHuman()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
end

function ElectricClaw()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
end

function DragonTalon()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
end

function SharkmanKarate()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
end

function DeathStep()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
end


function CyborgRace()
    local args = {
        [1] = "CyborgTrainer",
        [2] = "Buy"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end

function GhoulRace()
    local args = {
        [1] = "Ectoplasm",
        [2] = "BuyCheck",
        [3] = 4
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    local args = {
        [1] = "Ectoplasm",
        [2] = "Change",
        [3] = 4
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end




--Tabs
 local Tab1 = Window:CreateTab("Main") -- Title, Image
 local Tab2 = Window:CreateTab("Mics")
 local Tab3 = Window:CreateTab("Dungeon")
 local Tab4 = Window:CreateTab("Open Gui Stuff")
 local Section = Tab3:CreateSection("Raid")
 local Section = Tab2:CreateSection("BuyRace")
 local Section = Tab1:CreateSection("MainScript")


--Buttons
 local Button = Tab1:CreateButton({
    Name = "Roll da Fruite",
    Callback = function()
            Rollfruit()
    end,
 })

 local Button = Tab2:CreateButton({
    Name = "Cyborg Race (2,500 frag)",
    Callback = function()
            CyborgRace()
    end,
 })

local Button = Tab2:CreateButton({
    Name = "Ghoul Race (100 ectopalsm must have given HellTorch)",
    Callback = function()
            GhoulRace()
    end,
})

local Button = Tab2:CreateButton({
    Name = "Godhuman",
    Callback = function()
            Godhuman()
    end,
})

local Button = Tab2:CreateButton({
    Name = "Superhuman",
    Callback = function()
            SuperHuman()
    end,
})

local Button = Tab2:CreateButton({
    Name = "SharkmanKarate",
    Callback = function()
            SharkmanKarate()
    end,
})

local Button = Tab2:CreateButton({
    Name = "DragonTalon",
    Callback = function()
            DragonTalon()
    end,
})

local Button = Tab2:CreateButton({
    Name = "ElectricClaw",
    Callback = function()
            ElectricClaw()
    end,
})

local Button = Tab2:CreateButton({
    Name = "DeathStep",
    Callback = function()
            DeathStep()
    end,
})

local Button = Tab1:CreateButton({
    Name = "PirateTeamChange",
    Callback = function()
            Pirateteam()
    end,
})

local Button = Tab1:CreateButton({
    Name = "MarineTeamChange",
    Callback = function()
            Marineteam()
    end,
})

local Button = Tab4:CreateButton({
    Name = "devil fruit shop",
    Callback = function()
            Devilfruitshop()
    end,
})

local Button = Tab4:CreateButton({
    Name = "Open Color Gui",
    Callback = function()
            ColorGui()
    end,
})
local Button = Tab4:CreateButton({
    Name = "Open Title Gui",
    Callback = function()
            TitleGui()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Stat Refund",
    Callback = function()
            Statrefund()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki First Stage",
    Callback = function()
            Busohaki0()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki Stage1",
    Callback = function()
            Busohaki1()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki Stage2",
    Callback = function()
            Busohaki2()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki Stage3",
    Callback = function()
            Busohaki3()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki Stage4",
    Callback = function()
            Busohaki4()
    end,
})

local Button = Tab1:CreateButton({
    Name = "Buso Haki Stage5",
    Callback = function()
            Busohaki5()
    end,
})

local Button = Tab4:CreateButton({
    Name = "Open Awakening Expert",
    Callback = function()
            Awakeningexpert()
    end,
})
--Toggle
local Toggle = Tab3:CreateToggle({
    Name = "Kill_Aura",
    CurrentValue = false,
    Flag = "Kill_Aura", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
    Callback = function(Value)
            Kill_Aura()
    -- The variable (Value) is a boolean on whether the toggle is true or false
    end,
 })



