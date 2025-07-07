-- CONFIGURAÇÕES
local keyURL = "https://lootdest.org/s?mL4PPK3f" -- link direto onde estará a key
local correctDecoded = "MI HUB UNLOCK"

-- Interface
local player = game.Players.LocalPlayer
local gui = Instance.new("ScreenGui", player:WaitForChild("PlayerGui"))
gui.Name = "MiHubKeyUI"
gui.ResetOnSpawn = false

local frame = Instance.new("Frame", gui)
frame.Size = UDim2.new(0, 350, 0, 180)
frame.Position = UDim2.new(0.5, -175, 0.5, -90)
frame.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
frame.BorderSizePixel = 0

-- Texto
local title = Instance.new("TextLabel", frame)
title.Size = UDim2.new(1, 0, 0, 40)
title.Position = UDim2.new(0, 0, 0, 0)
title.BackgroundTransparency = 1
title.Text = "🔐 MI HUB - KEY SYSTEM"
title.TextColor3 = Color3.new(1, 1, 1)
title.Font = Enum.Font.SourceSansBold
title.TextSize = 24

-- Caixa de digitar a key
local input = Instance.new("TextBox", frame)
input.Size = UDim2.new(0.8, 0, 0, 35)
input.Position = UDim2.new(0.1, 0, 0.35, 0)
input.PlaceholderText = "Digite a key..."
input.Text = ""
input.Font = Enum.Font.SourceSans
input.TextSize = 18
input.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
input.TextColor3 = Color3.new(1,1,1)

-- Botão de Validar
local checkBtn = Instance.new("TextButton", frame)
checkBtn.Size = UDim2.new(0.4, 0, 0, 35)
checkBtn.Position = UDim2.new(0.1, 0, 0.65, 0)
checkBtn.Text = "Validar"
checkBtn.Font = Enum.Font.SourceSansBold
checkBtn.TextSize = 18
checkBtn.BackgroundColor3 = Color3.fromRGB(0, 170, 0)
checkBtn.TextColor3 = Color3.new(1, 1, 1)

-- Botão de Copiar Link
local copyBtn = Instance.new("TextButton", frame)
copyBtn.Size = UDim2.new(0.4, 0, 0, 35)
copyBtn.Position = UDim2.new(0.5, 10, 0.65, 0)
copyBtn.Text = "Obter Key 🔗"
copyBtn.Font = Enum.Font.SourceSansBold
copyBtn.TextSize = 18
copyBtn.BackgroundColor3 = Color3.fromRGB(0, 85, 170)
copyBtn.TextColor3 = Color3.new(1, 1, 1)

-- Função de decodificar a key (simples, exemplo: reverso + base64)
local function decodeKey(encoded)
    -- Simples exemplo: reverter e decodificar base64 (você pode inventar outra lógica)
    local base64decode = function(data)
        local b = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
        data = string.gsub(data, "[^" .. b .. "=]", "")
        return (data:gsub(".", function(x)
            if x == "=" then return "" end
            local r,f="",(b:find(x)-1)
            for i=6,1,-1 do r=r..(f%2^i - f%2^(i-1) > 0 and "1" or "0") end
            return r;
        end):gsub("%d%d%d?%d?%d?%d?%d?%d?", function(x)
            if #x ~= 8 then return "" end
            local c=0
            for i=1,8 do c=c + (x:sub(i,i)=="1" and 2^(8-i) or 0) end
            return string.char(c)
        end))
    end

    local reversed = encoded:reverse()
    return base64decode(reversed)
end

-- Evento Validar
checkBtn.MouseButton1Click:Connect(function()
    local inputKey = input.Text
    local success, decoded = pcall(decodeKey, inputKey)

    if success and decoded == correctDecoded then
        frame:Destroy()
        -- Aqui você carrega o Mi Hub:
        loadstring(game:HttpGet("https://raw.githubusercontent.com/cubodegelo1116/mi-hub-brookhaven-real/refs/heads/main/MI%20BROOKHAVEN"))()
    else
        input.Text = "❌ Key inválida ou expirada!"
    end
end)

-- Evento Copiar Link
copyBtn.MouseButton1Click:Connect(function()
    setclipboard(keyURL)
    copyBtn.Text = "Copiado!"
    task.wait(2)
    copyBtn.Text = "Obter Key 🔗"
end)
