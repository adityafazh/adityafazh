local Tween = game:GetService("TweenService")
local Char = game.Players.LocalPlayer.Character

while true do
   for _,v in pairs(game.Workspace:GetDescendants()) do
       if v.name == "Chest1" or v.name == "Chest2" then
           wait(2)
           Char.HumanoidRootPart.CFrame = v.CFrame:Lerp(v.CFrame, 0)
       end
   end
end
