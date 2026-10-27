# VortexCut Studio 15.2 "Pro Update"

![VortexCut Studio 15.0 — Kdenlive Edition](preview-v15.0.png)

> Continuação direta da série 15: a 15.0 trouxe o mixer por trilha, a fila de
> renderização e as zonas de exportação (inspiração Kdenlive); a 15.1 protegeu
> o fluxo de trabalho com backups e fila persistente; a **15.2 dá controlo fino
> de áudio e prioridade ao que importa** — tudo com código 100% próprio.

## Novo na 15.2

### 🎛 Pan por trilha no Mixer
Cada canal do mixer ganhou um slider de pan (**Esquerda ← Centro → Direita**)
com panorâmica **equal-power** aplicada na exportação — a mesma técnica dos
editores profissionais. Desloque a narração para um lado, a música para o
outro, e o VU meter mostra o resultado em tempo real antes de exportar.

### ⚏ Prioridade na fila de renderização
Botões **↑/↓** em cada job pendente da fila. Está a renderizar três vídeos e o
cliente pediu urgência? Mande o dele para o topo com um clique, sem cancelar
nada. A ordem também sobrevive ao fecho do app (a fila é persistente desde a 15.1).

### ⭐ Favoritos exportáveis (JSON)
"Meus Favoritos" agora viaja com você: exporte todos os itens marcados com
estrela para um ficheiro `.json` e importe noutro PC — **juntando** aos
favoritos existentes (merge seguro) ou **substituindo** tudo. Ideal para
partilhar o seu kit de efeitos/transições entre máquinas ou com a equipa.

### 🎢 Speed Ramping com 13 presets
O editor de curva de velocidade (v11) ganhou **presets prontos** — entre eles
*Ski Hill*, *Bullet Time* e *Whip* — todos validados (tempo ordenado, fatores
dentro de 0.25x–4x). Aplique num clique e ajuste depois na curva.

### 🌊 +2 intros animadas: Onda Sonora e Constelação
A biblioteca de intros sobe para **36 animações**. *Onda Sonora* desenha
barras reativas para conteúdos de música/podcast; *Constelação* liga pontos
com linhas luminosas para aberturas tech/elegantes.

### 📤 Fila mostra o projeto de origem
Cada linha da fila de renderização indica de **que projeto** o job veio
("· projeto: NomeDoProjeto") — essencial agora que a fila persiste entre
sessões. Jobs restaurados de outro projeto continuam avisados.

## Já vinha da 15.1 "Pro Update"

- **🕘 Backups automáticos datados** — cópia do projeto a cada ~5 min em
  `~/.vortexcut/backups` (últimos 10), recuperável em Arquivo → "Abrir backup automático…".
- **🔊 Normalizar áudio na exportação** — pico seguro em 98 %, sem clipping duro (ganho máx. 4×).
- **↻ Fila persistente + Reenfileirar falhados** — a fila sobrevive ao fecho do app; 1 clique repete renders falhados.
- **⚏ Guias de enquadramento** — grade dos terços (Ctrl+G) e cruz central (Ctrl+Shift+G) no preview.

## Instalação

1. Abra a página [Releases](https://github.com/kenjunior01/VortexCutStudio/releases/latest).
2. Descarregue `VortexCutStudio_Setup.exe` (versão 15.2.0).
3. Execute e siga o assistente.

**Requisitos:** Windows 10/11 64 bits · o instalador já inclui o FFmpeg.

---

*VortexCut Studio — editor de vídeo desktop em Python + PySide6 + FFmpeg.*
