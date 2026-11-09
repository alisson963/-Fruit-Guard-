# 🍎 Fruit Guard V2

### Coleta inteligente de frutas no Roblox com Python e visão computacional

![Python](https://img.shields.io/badge/Python-3.11%20%7C%203.12-3776AB?style=flat-square&logo=python&logoColor=white)
![Windows](https://img.shields.io/badge/Plataforma-Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
![OpenCV](https://img.shields.io/badge/Visão%20Computacional-OpenCV-5C3EE8?style=flat-square)
![Status](https://img.shields.io/badge/Status-Beta-orange?style=flat-square)

**Fruit Guard** é um aplicativo desktop desenvolvido em Python que utiliza visão computacional para identificar frutas na tela de um jogo do Roblox e planejar movimentos automáticos com as teclas WASD.

O projeto explora reconhecimento de imagens, navegação inteligente, automação de teclado e desenvolvimento de interfaces gráficas.

![Interface do Fruit Guard V2](exemplos/preview_v2.png)

## ✨ Funcionalidades

- 🍓 **Detecção de frutas:** identifica frutas coloridas utilizando OpenCV.
- 🎯 **Busca inteligente:** seleciona alvos e calcula trajetórias para alcançá-los.
- 🎮 **Movimentação WASD:** executa movimentos direcionais e diagonais.
- 🔄 **Coleta contínua:** procura novas frutas após cada movimentação.
- 🛡️ **Delimitação de área:** permite definir cercas, obstáculos e margens de segurança.
- 📷 **Rastreamento visual:** acompanha o personagem e tenta compensar movimentos da câmera.
- 🖥️ **Interface gráfica:** painel intuitivo para configurar, iniciar, parar e acompanhar o funcionamento.

> **Status:** versão beta. A detecção e a navegação foram avaliadas com imagens e simulações locais. A movimentação real depende da calibração, da câmera e da aceitação dos comandos pelo jogo.

## 🛠️ Tecnologias

| Tecnologia | Aplicação |
|---|---|
| Python | Desenvolvimento principal |
| OpenCV | Visão computacional |
| NumPy | Processamento de dados e imagens |
| Tkinter | Interface gráfica |
| MSS | Captura de tela |
| Pillow | Manipulação de imagens |
| Psutil | Verificação de processos |
| Win32 SendInput | Simulação de teclas no Windows |

## 🚀 Instalação

**Requisitos:** Windows 10/11 e Python 3.11 ou 3.12.

1. Baixe o repositório usando **Code → Download ZIP**.
2. Extraia os arquivos para uma pasta.
3. Instale o Python, habilitando a opção **Add Python to PATH**.
4. Execute `INSTALAR_E_ABRIR.bat`.
5. Nas próximas vezes, execute `ABRIR.bat`.

Para instalar manualmente pelo PowerShell:

```powershell
py -3.12 -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe app.py
```

## 🎮 Como utilizar

1. Abra o Roblox e posicione o personagem na arena.
2. Pressione **F6** para capturar a tela.
3. Configure os quatro cantos do cercado, o personagem e os obstáculos.
4. Salve a calibração.
5. Pressione **F7** para iniciar a coleta.
6. Pressione **F8** para interromper o programa.

### ⌨️ Atalhos

| Tecla | Função |
|---|---|
| F6 | Capturar tela |
| F7 | Iniciar automação |
| F8 | Parar automação |

## 🧪 Testes

O projeto possui scripts de teste que não controlam o Roblox:

- `TESTAR_DETECCAO.bat` — reconhecimento de frutas.
- `TESTAR_MOVIMENTO_SEM_ROBLOX.bat` — simulação de navegação.
- `TESTAR_CAMERA_SEM_ROBLOX.bat` — acompanhamento de movimentos da câmera.

## 📁 Estrutura do projeto

```text
Fruit-Guard-Roblox/
├── app.py
├── vision.py
├── engine.py
├── controller.py
├── requirements.txt
├── INSTALAR_E_ABRIR.bat
├── ABRIR.bat
├── TESTAR_*.bat
└── exemplos/
    ├── preview_v2.png
    └── print_original.png
```

## 🗺️ Futuras atualizações

- [ ] Melhorar a precisão do rastreamento.
- [ ] Otimizar a movimentação entre frutas.
- [ ] Adicionar perfis para diferentes resoluções.
- [ ] Melhorar o reconhecimento em cenários variados.
- [ ] Expandir os testes e ferramentas de diagnóstico.

## ⚠️ Avisos

O Fruit Guard é um projeto experimental com finalidade educacional.

A identificação visual pode falhar e não há garantia de que o personagem permanecerá dentro da área delimitada. Recomenda-se supervisionar os testes e verificar as regras do jogo antes de usar automação.

Este projeto não possui vínculo oficial com o Roblox. As imagens e os elementos do jogo pertencem aos respectivos titulares.

## 💡 Sobre o projeto

Desenvolvido para explorar conhecimentos de **Python, visão computacional, automação e desenvolvimento de software**, com assistência de ferramentas de inteligência artificial.

**Gostou do projeto? Deixe uma ⭐ no repositório!**
