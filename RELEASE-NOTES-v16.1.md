# Release Notes — VortexCut Studio 16.1 "Photo Studio+"

*Data: 30 de outubro de 2026*

A versão 16.1 amplia o **Estúdio de Imagem** com mais recursos de nível
Photoshop, mantendo tudo em código 100% próprio (numpy + PySide6, sem
dependências novas).

## 🆕 Novo no Estúdio de Imagem

### 📈 Curvas interativas (Ctrl+M)
Editor de curvas completo: pontos arrastáveis, clique no vazio adiciona um
ponto, botão direito remove; canais **RGB / R / G / B** independentes; o
**histograma do canal** aparece ao fundo da curva; botões de reset por canal
e geral; **preview ao vivo** antes de aplicar.

### ☀☾◔✧ 4 pincéis de retoque
- **Clarear (D)** — pincel dodge
- **Escurecer (J)** — pincel burn
- **Desfoque local (K)**
- **Nitidez local (P)**

Todos com tamanho, dureza e opacidade na barra de ferramentas, respeitam a
seleção ativa e entram no histórico de desfazer.

### ⤡ Transformar camada (Ctrl+T)
Escala (5–300 %), rotação (−180°..180°), translação e espelhos H/V da
**camada ativa**, com fundo transparente, preview ao vivo e interpolação
bilinear (remapeamento afim em numpy puro).

### 🌈 Duotone / Mapa de gradiente
Mapeia a luminância para duas cores à escolha, com **4 presets prontos**
(Azul-noite, Sépia clássico, Ciano-Vaporwave, Verde-tinta) e preview ao vivo.

### 🖍 4 filtros artísticos
- **Cartoon** — posterização + contornos escuros (níveis e força ajustáveis)
- **Halftone** — pontos de jornal com célula e ângulo configuráveis
- **Lomo** — vinheta forte + saturação + curva em S
- **Brilho suave (Orton)** — glow em modo Screen (brilho e raio ajustáveis)

### ⊕⊖ Seleção: expandir / contrair
Cresce ou encolhe a seleção em pixels (área circular) — refina varinha/laço
antes de pintar ou filtrar. Implementado com filtro morfológico próprio.

### 📊 Histograma R·G·B
O dock "Cores & Histograma" passa a mostrar **Luminância, R, G, B ou
R·G·B em overlay**, com cores por canal.

## 🔧 Interno
- Engine `imgfilters`: +11 funções (`curvas`, `_lut_de_pontos`,
  `gradiente_mapa`, `duotone`, `cartoon`, `halftone`, `lomo`, `soft_glow`,
  `retouch`, `expand_mask`, `affine_warp`, `histograma_rgb`) — 74 checks no
  auto-teste.
- GUI `image_studio`: 19 ferramentas, 20 filtros registados, 70 checks no
  auto-teste.
- Nova suite de regressão `test_v16_1_integration.py` (75 checks); regressão
  total **17/17 suites** (~775 checks) verde.
- **Novo guia**: `GUIA-ESTUDIO-IMAGEM.md` — manual completo do Estúdio
  (ferramentas, camadas, curvas, filtros, atalhos e exportação).

## ⬇️ Instalação
1. Baixe `VortexCutStudio-Desktop-v16.1.zip` e extraia.
2. Rode `verificar_ambiente.py` para conferir as dependências.
3. Para o instalador Windows: `installer/CRIAR_INSTALADOR.bat`
   (Inno Setup 6 — gera o `.exe` no seu PC).
4. `LEIA-ME.md` e `INSTRUCOES_PYCHARM.md` atualizados para 16.1.
