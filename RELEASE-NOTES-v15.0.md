# VortexCut Studio 15.0 "Kdenlive Edition"

> Inspirada no Kdenlive (kde.org/kdenlive) — os recursos mais pedidos do editor profissional do KDE, agora no VortexCut Studio, com código 100% próprio.

![Pré-visualização da 15.0](preview-v15.0.png)

## Novidades

### 🎚 Mixer de áudio por trilha
- Um canal por trilha com fader de volume (0–200 %), botões **Mudo (M)** e **Solo (S)** — solo aditivo, como no Kdenlive.
- **VU meter estéreo L/R** com pico flutuante e **indicador de clipping** (novidade do Kdenlive 25.12).
- O volume/solo da trilha são aplicados também na **exportação final** (mixagem respeita ganho, mudo e solo).
- Atalho: `Ctrl+Shift+M`.

### 📤 Fila de renderização (jobs)
- Enfileire várias exportações e **continue a editar** — a fila corre os jobs em sequência, como no Kdenlive.
- Tabela com nome, preset, destino, estado (⏳ Na fila → ⚙ A renderizar → ✅ Concluído / ❌ Falhou / ⛔ Cancelado) e progresso.
- Cancelar job atual e limpar terminados com 1 clique. No diálogo de exportação: **"➕ Adicionar à fila"**.

### 🎯 Zona de exportação (Selected Zone)
- Exporte apenas o intervalo definido — ideal para testar um trecho sem renderizar tudo.
- `Ctrl+Shift+Z` · a zona fica salva no projeto (.vxc) e pré-selecionada no diálogo de exportação.

### 🎯 Multi-Export por Marcadores (Marker Zones)
- O recurso clássico do Kdenlive: cada **par de marcadores** da timeline define uma zona (1º→2º, 3º→4º…) e cada zona vira um **MP4 independente**.
- Perfeito para cortar e exportar vários clipes de um único projeto.

### 🎨 Operações de trilha (Kdenlive 26.08)
- **Cor da trilha** no cabeçalho da timeline (faixa colorida), **reordenar trilhas** para cima/baixo, silenciar/ocultar/bloquear.
- A altura das trilhas agora é persistida no projeto.

### ⭐ Favoritos universais da biblioteca
- Botão direito em qualquer card alterna a estrela; filtro **"⭐ Só favoritos"** em todas as abas.
- Persistência local em `~/.vortexcut/favoritos.json` (os favoritos de legendas da 12.1 continuam válidos).

### 🎬 Biblioteca expandida — 1080+ itens
- **+8 intros animadas**: Claquete de Cinema, Aurora Boreal, Circuito Vivo, Luz de Estádio, Papel Rasgado, Órbita em Foco, VHS 90, Torre Pixel.
- **+20 templates de edição**: Documentário, Tutorial com Passos, Notícias Urgentes, Unboxing, Viagem Cinemática, Treino Hype, Receita Rápida, Imóvel Premium, Casamento Suave, Review Tech, Stream Gamer, Clipe de Podcast, Lookbook Moda, Motivacional, Corporativo, Cover Musical, Antes e Depois, Sorteio da Loja, Trailer Épico, Pet Fofura.

## Qualidade
- 14 suítes de regressão — **~656 verificações verdes** (96 novas na v15).
- Compatibilidade total: projetos v7+ abrem normalmente; campos novos têm valores padrão.

## Verificação (SHA-256)

Depois de descarregar o instalador, confirme o hash no Windows:

```
certutil -hashfile VortexCutStudio_Setup.exe SHA256
```

SHA-256: *(a preencher com o valor do instalador desta release)*

## Notas

- Requisitos: Windows 10 ou 11, 64 bits.
- O instalador inclui FFmpeg 7.1.1 (essentials, gyan.dev) e as fontes necessárias.
- Não é necessária ligação à Internet para editar nem para exportar.
