ESSA LIBARY FOI FEITA POR GAGADEV DONO DO DRAK HUB
# NOSSO DISCORD : https://discord.gg/Wb6xmQHSN 

# INSTALAÇÃO 
local draklib = loadstring(game:HttpGet("https://raw.githubusercontent.com/gaga123308/Draklibary/refs/heads/main/main.lua"))()({

# NAME
    Title = "Drak Hub",
    SubTitle = "v1.0"
})

# ABAS
local Tab1 = draklib:CreateTab("Home", "10709751939")

# CARD DISCORD
Tab1:CreateDiscord({
	Title = "nome",
	Link = "https://discord.gg/seu-convite",
	ImageId = "seu id *não precisa colocar rbx do o id"
})
# BUTÃO AND TOGGLE 
Tab1:CreateButton({
	Name = "Nome do Botão",
	Script = "print('Botão clicado!')"
})

# segunda opção 
 Tab1:CreateButton({
	Name = "Nome do Botão",
	Description = "Descrição do que o botão faz",
	Script = 'loadstring(game:HttpGet(""))()'
})

Tab1:CreateToggle({
	Name = "Nome do Toggle",
	Default = false,
	Callback = function(estado)
		print("Status do Toggle:", estado) -- 'estado' retorna true (ligado) ou false (desligado)
	end
})

# Drompdow 
Tab1:CreateDropdown({
	Name = "Nome do Dropdown",
	Options = {"Opção 1", "Opção 2", "Opção 3"},
	Default = "Opção 1",
	Callback = function(escolha)
		print("Você selecionou:", escolha)
	end
})
se quiser colocar nomes de usuário coloque o código ali ou pede uma ia

# TOGGLE AND TEXTBOX AND PARÁGRAFO 
Tab1:CreateTextbox({
	Name = "Digite algo",
	PlaceholderText = "Escreva aqui...",
	Callback = function(texto)
		print("O usuário digitou:", texto)
	end
})

Tab1:CreateParagraph({
	Title = "Aviso Importante",
	Content = "test"
})

Tab1:CreateSlider({
	Name = "Velocidade (WalkSpeed)",
	Min = 16,
	Max = 100,
	Default = 16,
	Callback = function(valor)
		print("Valor selecionado no Slider:", valor)
		-- Exemplo prático aplicando no personagem:
		-- game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = valor
	end
})

# SECAO
Tab1:CreateSection("Seção de Configurações")

# Exemplo 
link : loadstring(game:HttpGet("https://raw.githubusercontent.com/gaga123308/Draklibaryexemple/refs/heads/main/exemple"))()
