# Childhood Balance 🎮✨

> Um jogo pixel art 2D que explora o amadurecimento precoce, amizades, sonhos pessoais e a pressão social através de escolhas narrativas e consequências ocultas.

![Badge License](https://img.shields.io/badge/license-MIT-blue.svg)
![Badge Status](https://img.shields.io/badge/status-early%20development-yellow.svg)
![Badge Tech](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20JavaScript-brightgreen.svg)

## 📖 Visão do Projeto

**Childhood Balance** é um jogo narrativo 2D que aborda temas sensíveis como:
- Adultização social, emocional, financeira e psicológica
- Pressão escolar e familiar
- Construção de identidade e "máscaras sociais"
- Amizades e relacionamentos dinâmicos
- Preservação da infância vs. amadurecimento inevitável

A experiência é transmitida de forma **indireta, narrativa e moderada**, sem conteúdo explícito ou pesado, através de:
- Escolhas consequentes (estilo Reigns)
- NPCs vivos com memória de decisões
- Múltiplos finais baseados em caminhos
- Mundo semiaberto explorador

---

## 🎨 Inspirações

- **Reigns** - Sistema de escolhas swipe/card
- **Stardew Valley** - Exploração, NPCs dinâmicos, ciclo dia/noite
- **Pokémon** - Coleta, exploração, conexão com personagens
- **The Legend of Zelda: A Link to the Past** - Mundo conectado, segredos exploráveis

---

## 🎮 Características

### Exploração
- 🏙️ Cidades com prédios, lojas e ruas
- 🏘️ Bairros residenciais dinâmicos
- 🏖️ Praias e áreas rurais
- 🌲 Florestas secretas e exploráveis
- 🎓 Escolas, praças e locais memoráveis
- 🔓 Áreas desbloqueáveis por progresso

### NPCs & Relacionamentos
- Personagens únicos com nomes, rotinas próprias
- Sistema de reputação social
- Memória de todas as escolhas do jogador
- Diálogos que mudam conforme relacionamento
- Relações entre NPCs que evoluem
- Eventos aleatórios baseados em relacionamentos

### Gameplay
- 🎯 Movimentação livre 8-direcional
- 📋 Sistema de "máscaras sociais" (personalidades diferentes)
- 🎲 Consequências ocultas nas escolhas
- 🔄 Múltiplos finais desbloqueáveis
- 📔 Coleção de memórias (recordações chave)
- 🌙 Ciclo dia/noite com eventos sazonais

### Interface
- HUD minimalista
- Inventário de memórias
- Barra de "infância" (vs amadurecimento)
- Menus suaves com animações
- Efeitos visuais contemplativos

---

## 📁 Estrutura do Projeto

```
childhood-balance/
├── index.html                 # Arquivo principal HTML5
├── README.md                  # Este arquivo
├── ROADMAP.md                 # Plano de desenvolvimento
├── CONTRIBUTING.md            # Guia para colaboradores
├── CODE_OF_CONDUCT.md         # Código de conduta
│
├── /assets                    # Recursos do jogo
│   ├── /sprites              # Pixel art (NPCs, objetos, efeitos)
│   ├── /audio                # Música e sons (WebAudio/MP3)
│   └── /fonts                # Fontes customizadas
│
├── /scripts                   # Lógica do jogo modularizada
│   ├── game.js               # Orquestrador principal
│   ├── player.js             # Classe do jogador
│   ├── npc.js                # Sistema de NPCs
│   ├── map.js                # Sistema de mapas e tilemap
│   ├── dialogue.js           # Sistema de diálogos
│   ├── choices.js            # Sistema de escolhas (Reigns-like)
│   ├── reputation.js         # Sistema de reputação
│   ├── daynight.js           # Ciclo dia/noite
│   ├── events.js             # Sistema de eventos aleatórios
│   ├── memories.js           # Sistema de memórias/recordações
│   ├── inventory.js          # Inventário e itens
│   ├── social-masks.js       # Sistema de máscaras sociais
│   ├── audio-manager.js      # Gerenciador de áudio
│   ├── input.js              # Sistema de entrada (teclado/mouse)
│   ├── camera.js             # Sistema de câmera
│   ├── animation.js          # Sistema de animações
│   └── utils.js              # Funções utilitárias
│
├── /styles                    # CSS organizado
│   ├── main.css              # Estilos globais
│   ├── game.css              # Estilos do jogo
│   ├── ui.css                # Estilos da interface
│   ├── dialogue.css          # Estilos de diálogos
│   └── animations.css        # Animações CSS
│
├── /ui                        # Componentes de interface
│   ├── hud.js                # Head-up display
│   ├── menu.js               # Sistema de menus
│   ├── dialogue-box.js       # Caixa de diálogos
│   ├── choice-panel.js       # Painel de escolhas
│   ├── inventory.js          # Tela de inventário
│   └── settings.js           # Menu de configurações
│
├── /maps                      # Dados dos mapas (JSON)
│   ├── map-data.js           # Definições de mapas
│   ├── city.json             # Dados da cidade
│   ├── neighborhood.json     # Dados do bairro
│   ├── beach.json            # Dados da praia
│   ├── farm.json             # Dados da fazenda
│   ├── forest.json           # Dados da floresta
│   └── school.json           # Dados da escola
│
├── /dialogues                 # Sistema de diálogos
│   ├── npc-dialogues.js      # Banco de diálogos dos NPCs
│   ├── events-dialogues.js   # Diálogos de eventos
│   └── tutorial.js           # Diálogos do tutorial
│
└── /data                      # Dados do jogo (JSON)
    ├── npcs.json             # Definição de NPCs
    ├── choices.json          # Escolhas disponíveis
    ├── items.json            # Itens colecionáveis
    └── events.json           # Eventos aleatórios
```

---

## 🚀 Começando

### Requisitos
- Navegador moderno com suporte HTML5 Canvas
- Nenhuma dependência externa (vanilla JavaScript)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/lucianx71/childhood-balance.git
cd childhood-balance

# Abra em um servidor local (recomendado)
python3 -m http.server 8000
# ou
npx http-server

# Abra no navegador
# http://localhost:8000
```

### Executar
Simplesmente abra `index.html` no navegador ou acesse via servidor local.

---

## 🎯 Roadmap

Veja [ROADMAP.md](ROADMAP.md) para detalhes completos.

### Fase 1: MVP (Core Gameplay)
- [x] Estrutura base do projeto
- [ ] Sistema de movimentação e câmera
- [ ] Primeiro mapa (cidade central)
- [ ] 5 NPCs base com diálogos
- [ ] Sistema de escolhas simples
- [ ] Ciclo dia/noite básico

### Fase 2: Mecânicas Principais
- [ ] Sistema de reputação
- [ ] Memória de escolhas
- [ ] Eventos aleatórios
- [ ] Sistema de máscaras sociais
- [ ] 10+ NPCs com relacionamentos
- [ ] 3+ mapas conectados

### Fase 3: Profundidade Narrativa
- [ ] Consequências ocultas reveláveis
- [ ] Múltiplos finais
- [ ] Coleção de memórias
- [ ] Relacionamentos dinâmicos entre NPCs
- [ ] Eventos secretos

### Fase 4: Polish
- [ ] Animações refinadas
- [ ] Efeitos visuais
- [ ] Trilha sonora e SFX
- [ ] Otimização de performance
- [ ] Mobile responsivo

---

## 🛠️ Desenvolvimento

### Stack Técnico
- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Renderização**: Canvas 2D API
- **Arquitetura**: Modular, orientada a componentes
- **Assets**: Pixel art (aseprite/piskelapp)

### Padrões de Código
- Módulos ES6
- Nomes descritivos e self-documenting
- Comentários em português para clareza
- Funções puras quando possível

### Como Contribuir

Veja [CONTRIBUTING.md](CONTRIBUTING.md) para detalhes completos.

1. Fork o repositório
2. Crie uma branch (`git checkout -b feature/sua-feature`)
3. Commit suas mudanças (`git commit -m 'Add: descrição'`)
4. Push para a branch (`git push origin feature/sua-feature`)
5. Abra um Pull Request

---

## 📝 Código de Conduta

Este projeto segue um Código de Conduta para garantir um ambiente acolhedor e inclusivo. Veja [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE) - veja o arquivo LICENSE para detalhes.

---

## 🤝 Créditos

- **Criador**: lucianx71
- **Inspirações**: Reigns, Stardew Valley, Pokémon, The Legend of Zelda
- **Comunidade**: Contribuidores e testadores

---

## 💬 Contato & Comunidade

- 📧 Issues e Discussions no GitHub
- 🐛 Reporte bugs em [Issues](https://github.com/lucianx71/childhood-balance/issues)
- 💡 Sugira features em [Discussions](https://github.com/lucianx71/childhood-balance/discussions)

---

## 🎵 Temática

O jogo explora a questão central: **Como manter a esperança e autenticidade enquanto cresce em um mundo que exige conformidade?**

Cada escolha do jogador não é julgada como "certa" ou "errada", mas como reflexos genuínos de como lidamos com pressão, amizade, sonhos e identidade.

---

**Childhood Balance** • 2026 • Open Source • Made with ❤️