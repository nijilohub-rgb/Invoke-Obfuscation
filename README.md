-- Esse é o único código que você vai ofuscar
local script_url = "https://pastebin.com/raw/K8athHSf"

local success, result = pcall(function()
    return game:HttpGet(script_url)
end)

if success then
    loadstring(result)()
else
    warn("Erro ao carregar o script: " .. tostring(result))
end
