-- Mod Menu Fake para treino
-- Feito por Yago

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local Description = Instance.new("TextLabel")

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

-- Frame principal
Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Frame.Size = UDim2.new(0, 250, 0, 300)
Frame.Position = UDim2.new(0.7, 0, 0.3, 0)

-- Título
Title.Parent = Frame
Title.Text = "Mod Menu"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.Size = UDim2.new(1, 0, 0, 40)
Title.BackgroundColor3 = Color3.fromRGB(50, 50, 50)

-- Descrição
Description.Parent = Frame
Description.Text = "Feito por Yago"
Description.TextColor3 = Color3.fromRGB(200, 200, 200)
Description.Size = UDim2.new(1, 0, 0, 30)
Description.Position = UDim2.new(0, 0, 0, 45)
Description.BackgroundTransparency = 1

-- Botões de exemplo (sem funções reais)
local buttons = {"ESP Linha e Nome", "Auto Farm Level", "Auto Farm Material"}
for i, btnName in ipairs(buttons) do
    local button = Instance.new("TextButton")
    button.Parent = Frame
    button.Text = btnName
    button.TextColor3 = Color3.fromRGB(255, 255, 255)
    button.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
    button.Size = UDim2.new(1, -20, 0, 30)
    button.Position = UDim2.new(0, 10, 0, 80 + (i - 1) * 40)
end
