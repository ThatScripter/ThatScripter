local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "3rd Jailbreaker",
   LoadingTitle = "3rd Jailbreaker Hub",
   LoadingSubtitle = "by @Staff",
   ConfigurationSaving = {
      Enabled = false,
      FolderName = nil,
      FileName = "3rd Hub"
   },
   Discord = {
      Enabled = true,
      Invite = "https://discord.gg/jqbxxvtAUQ",
      RememberJoins = true
   },
   KeySystem = true,
   KeySettings = {
      Title = "Jailbreak / Keys",
      Subtitle = "Join the Discord For the Key Link!",
      Note = "Join the server in the misc tab",
      FileName = "Key",
      SaveKey = false,
      GrabKeyFromSite = true,
      Key = {"https://pastebin.com/raw/ZqgyZ3Z9"}
   }
})

local MainTab = Window:CreateTab("Home", nil)
local MainSection = MainTab:CreateSection("Main")

Rayfield:Notify({
   Title = "The Script Has been executed!",
   Content = "A Clean Powerful GUI",
   Duration = 5,
   Image = nil,
   Actions = {
      Ignore = {
         Name = "Okay!",
         Callback = function()
         print("The user has been smart(:")
      end
   },
},
})

local Button = MainTab:CreateButton({
   Name = "Fly GUI",
   Callback = function()
       
loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
   end,
})

local Slider = MainTab:CreateSlider({
   Name = "Walkspeed Slider",
   Range = {0, 300},
   Increment = 1,
   Suffix = "Speed",
   CurrentValue = 16,
   Flag = "Slider1",
   Callback = function(Value)
        game.Players.LocalPlayer.Character.Humanoid.Walkspeed = (Value)
   end,
})

local Button = MainTab:CreateButton({
   Name = "Jailbreak Hub",
   Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/alohabeach/Main/master/Scripts/JailbreakAutoRob.lua"))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "Infinite Yield",
   Callback = function()
       loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
   end,
})
