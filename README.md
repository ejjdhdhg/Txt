local Players = game:GetService("Players")
local player = Players.LocalPlayer
local gui = Instance.new("ScreenGui", player.PlayerGui)

-- Container para os botões
local container = Instance.new("Frame", gui)
container.Size = UDim2.new(0, 400, 0, 50)
container.Position = UDim2.new(0, 10, 0, 10)
container.BackgroundTransparency = 1

-- Layout para organizar os botões
local layout = Instance.new("UIListLayout", container)
layout.FillDirection = Enum.FillDirection.Horizontal
layout.Padding = UDim.new(0, 10)

-- Funções dos botões
local function createButton(name, color, callback)
    local button = Instance.new("TextButton", container)
    button.Size = UDim2.new(0, 90, 0, 40)
    button.Text = name
    button.BackgroundColor3 = color
    button.MouseButton1Click:Connect(callback)
    return button
end

-- Botão 1: Mensagem na tela
createButton("TP PG GAS", Color3.new(0.2, 0.8, 0.2), function()
Coloque este LocalScript em StarterPlayerScripts ou StarterGui
local player = game.Players.LocalPlayer
local targetCFrame = CFrame.new(-480.26, 8.82, -39.61) -- Edite X, Y, Z aqui!

local function teleportar()
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = targetCFrame
    end
end

-- Teleporta assim que o personagem carregar
player.CharacterAdded:Connect(function()
    task.wait(0.5) -- Pequena espera para garantir o carregamento
    teleportar()
end)

-- Teleporta imediatamente se já estiver no jogo
if player.Character then
    teleportar()
end
   -- The function that takes place when the button is pressed
   end,
})
    

-- Botão 2: Mudar cor do céu
createButton("ENTREGAR 1", Color3.new(0, 0.5, 1), function()
-- Coloque este LocalScript em StarterPlayerScripts ou StarterGui
local player = game.Players.LocalPlayer
local targetCFrame = CFrame.new(-807.32, 13.58, 51.87) -- Edite X, Y, Z aqui!

local function teleportar()
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = targetCFrame
    end
end

-- Teleporta assim que o personagem carregar
player.CharacterAdded:Connect(function()
    task.wait(0.5) -- Pequena espera para garantir o carregamento
    teleportar()
end)

-- Teleporta imediatamente se já estiver no jogo
if player.Character then
    teleportar()
end
   -- The function that takes place when the button is pressed
   end,
})
    

-- Botão 3: Mensagem no Output
createButton("ENTREGAR 2", Color3.new(1, 0.2, 0.2), function()
  Coloque este LocalScript em StarterPlayerScripts ou StarterGui
local player = game.Players.LocalPlayer
local targetCFrame = CFrame.new(-67.01, 11.71, 657.30) -- Edite X, Y, Z aqui!

local function teleportar()
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = targetCFrame
    end
end

-- Teleporta assim que o personagem carregar
player.CharacterAdded:Connect(function()
    task.wait(0.5) -- Pequena espera para garantir o carregamento
    teleportar()
end)

-- Teleporta imediatamente se já estiver no jogo
if player.Character then
    teleportar()
end
   -- The function that takes place when the button is pressed
   end,
})

-- Botão 4: Input de texto
createButton("ENTREGAR 3", Color3.new(1, 0.5, 0), function()
Coloque este LocalScript em StarterPlayerScripts ou StarterGui
local player = game.Players.LocalPlayer
local targetCFrame = CFrame.new(-243.95, 11.65, -101.78) -- Edite X, Y, Z aqui!

local function teleportar()
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = targetCFrame
    end
end

-- Teleporta assim que o personagem carregar
player.CharacterAdded:Connect(function()
    task.wait(0.5) -- Pequena espera para garantir o carregamento
    teleportar()
end)

-- Teleporta imediatamente se já estiver no jogo
if player.Character then
    teleportar()
end
   -- The function that takes place when the button is pressed
   end,
})


    
    input.FocusLost:Connect(function(enterPressed)
        if enterPressed then
            print("Texto digitado:", input.Text)
            input:Destroy()
        end
    end)
end)
