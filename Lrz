-- LRZ Hub com tela de carregamento
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Tela preta de carregamento
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

Frame.Parent = ScreenGui
Frame.Size = UDim2.new(1,0,1,0)
Frame.BackgroundColor3 = Color3.fromRGB(0,0,0)

TextLabel.Parent = Frame
TextLabel.Size = UDim2.new(1,0,1,0)
TextLabel.BackgroundTransparency = 1
TextLabel.TextColor3 = Color3.fromRGB(255,255,255)
TextLabel.TextScaled = true
TextLabel.Font = Enum.Font.SourceSansBold
TextLabel.Text = "LRZ Hub\nCarregando..."

-- Simulação de números carregando
for i = 1,100 do
    TextLabel.Text = "LRZ Hub\nCarregando... "..i.."%"
    wait(0.05)
end

-- Remove tela de carregamento
ScreenGui:Destroy()

-- Cria a janela principal do Hub
local Window = OrionLib:MakeWindow({
    Name = "LRZ Hub",
    HidePremium = false,
    SaveConfig = true,
    ConfigFolder = "LRZHub"
})

-- Abas principais (vazias, prontas para você adicionar funções)
local Funcoes = Window:MakeTab({
    Name = "Funções",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

local Visual = Window:MakeTab({
    Name = "Visual",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

local Misc = Window:MakeTab({
    Name = "Misc",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

-- Inicializa Hub
OrionLib:Init()
