# 🛣️ Roadmap - Childhood Balance

## Visão Geral

Este documento apresenta o plano de desenvolvimento em 4 fases principais, com metas claras e entregas esperadas.

---

## 📅 Fase 1: MVP - Core Gameplay (Semanas 1-4)

### Objetivos
- Estabelecer arquitetura base funcional
- Criar primeiro mapa jogável (cidade central)
- Implementar movimentação e câmera
- Sistema básico de diálogos
- 5 NPCs iniciais com rotinas

### Tarefas

#### Core Engine
- [x] Setup estrutura de pastas
- [ ] `game.js` - Loop principal do jogo
- [ ] `canvas.js` - Renderização base
- [ ] `input.js` - Sistema de entrada (teclado)
- [ ] `utils.js` - Funções utilitárias

#### Jogador
- [ ] `player.js` - Classe do jogador
- [ ] Movimentação 8-direcional
- [ ] Sprites base do personagem (4 direções)
- [ ] Animação de caminhada

#### Mundo
- [ ] `map.js` - Sistema de tilemap
- [ ] `camera.js` - Seguir jogador
- [ ] Primeiro mapa (cidade central) - 32x24 tiles
- [ ] Colisões base
- [ ] Transições entre mapas

#### NPCs
- [ ] `npc.js` - Classe base NPC
- [ ] 5 NPCs iniciais
- [ ] Rotinas simples (horários)
- [ ] Sistema de "ficar perto" de NPC

#### Diálogos
- [ ] `dialogue.js` - Sistema de diálogos
- [ ] `dialogue-box.js` - Interface
- [ ] Banco de diálogos iniciais
- [ ] Próximo/Anterior no diálogo

#### Interface
- [ ] `hud.js` - HUD básico
- [ ] `menu.js` - Menu principal
- [ ] Tela de título
- [ ] Pausa simples

### Entrega
- Game funcional com 1 mapa
- 5 NPCs conversáveis
- Movimentação fluida
- Menu principal e pausa

---

## 📅 Fase 2: Mecânicas Principais (Semanas 5-8)

### Objetivos
- Sistema de escolhas e consequências
- Reputação e relacionamentos
- Memória de decisões
- Eventos aleatórios
- 2 mapas adicionais

### Tarefas

#### Escolhas & Consequências
- [ ] `choices.js` - Sistema de escolhas (Reigns-like)
- [ ] `choice-panel.js` - Interface de escolhas
- [ ] Swipe/Click para escolher
- [ ] Banco de 50+ escolhas
- [ ] Consequências imediatas visíveis

#### Reputação
- [ ] `reputation.js` - Sistema de reputação social
- [ ] Reputação por NPC (0-100)
- [ ] Reputação geral (4 esferas)
- [ ] Diálogos mudam com reputação
- [ ] Visualização de status de reputação

#### Memória
- [ ] `memories.js` - Coleção de memórias
- [ ] Salvamento de decisões chave
- [ ] Tela de "lembranças"
- [ ] NPCs referenciam memórias

#### Eventos
- [ ] `events.js` - Sistema de eventos aleatórios
- [ ] 20+ eventos narrativos
- [ ] Eventos baseados em relacionamentos
- [ ] Randomização com pesos

#### Novos Mapas
- [ ] Mapa 2: Bairro residencial
- [ ] Mapa 3: Praia
- [ ] Conexões entre mapas
- [ ] Pontos de interesse em cada mapa

#### NPCs Expandidos
- [ ] 10 NPCs totais (5 novos)
- [ ] Relacionamentos entre NPCs
- [ ] Rotinas mais complexas
- [ ] Gossip (NPCs falam sobre outros)

#### Ciclo Dia/Noite
- [ ] `daynight.js` - Sistema de tempo
- [ ] 4 períodos: Manhã/Tarde/Noite/Madrugada
- [ ] Mudanças visuais (iluminação)
- [ ] NPCs em locais diferentes por hora

### Entrega
- 3 mapas conectados
- Sistema de escolhas funcional
- Reputação e relacionamentos
- 10 NPCs com comportamentos dinâmicos
- Ciclo dia/noite

---

## 📅 Fase 3: Profundidade Narrativa (Semanas 9-12)

### Objetivos
- Sistema de "máscaras sociais"
- Consequências ocultas reveladas
- Múltiplos finais
- Eventos secretos
- 3+ mapas adicionais

### Tarefas

#### Máscaras Sociais
- [ ] `social-masks.js` - Sistema de personalidades
- [ ] 4 máscaras principais (Conformista, Rebelde, Contemplativo, Líder)
- [ ] Máscara muda com escolhas
- [ ] NPCs reagem à máscara
- [ ] Diálogos exclusivos por máscara

#### Consequências Ocultas
- [ ] Sistema de "hidden consequences"
- [ ] Efeitos que aparecem após 2-5 eventos
- [ ] NPCs mudando de atitude gradualmente
- [ ] Cidades mudando visualmente
- [ ] Eventos "revelação" que desvendam consequências

#### Múltiplos Finais
- [ ] 5+ finais diferentes
- [ ] Desbloqueados por:
  - Máscaras sociais
  - Reputação geral
  - Memórias coletadas
  - Relacionamentos chave
- [ ] Créditos customizados por ending

#### Eventos Secretos
- [ ] 10+ eventos only-if condições
- [ ] Personagens secretos
- [ ] Locais desbloqueáveis
- [ ] Finais secretos

#### Novos Mapas
- [ ] Mapa 4: Fazenda/Área rural
- [ ] Mapa 5: Floresta (exploração)
- [ ] Mapa 6: Escola
- [ ] Mapa 7+: Áreas secretas

#### NPCs Expandidos
- [ ] 15+ NPCs totais
- [ ] Relacionamentos inter-NPC complexos
- [ ] Triângulos amorosos e conflitos
- [ ] Eventos de grupo

#### Inventory & Items
- [ ] `inventory.js` - Sistema de itens
- [ ] Coleção de recordações
- [ ] Itens que desbloqueiam diálogos
- [ ] Presentes para NPCs

### Entrega
- 7+ mapas exploráveis
- Sistema de máscaras sociais funcional
- Consequências ocultas em funcionamento
- 5+ finais únicos
- 15+ NPCs com dinâmicas complexas
- Eventos secretos

---

## 📅 Fase 4: Polish & Otimização (Semanas 13-16)

### Objetivos
- Qualidade visual refinada
- Áudio completo (música + SFX)
- Otimização de performance
- Responsividade mobile
- Experiência polida

### Tarefas

#### Pixel Art & Animações
- [ ] Sprites de 32x32 para todos NPCs
- [ ] 4 direções de movimento
- [ ] Animações de emote (emoções)
- [ ] Efeitos visuais (particulares, brilho)
- [ ] Tileset customizado para cada bioma
- [ ] UI icons pixel art

#### Áudio
- [ ] `audio-manager.js` - Gerenciador de áudio
- [ ] 6+ tracks de música ambiente
- [ ] 20+ sound effects
- [ ] Música dinâmica (muda com hora do dia)
- [ ] Volume control

#### Animações CSS
- [ ] `animations.css` - Transições suaves
- [ ] Menu fade-ins
- [ ] Diálogo typewriter effect
- [ ] Efeitos de hover
- [ ] Transições entre mapas

#### Performance
- [ ] Otimizar canvas rendering
- [ ] Cache de sprites
- [ ] Lazy loading de mapas
- [ ] Garbage collection
- [ ] FPS monitor

#### Mobile
- [ ] Touch input
- [ ] Responsive canvas
- [ ] Virtual d-pad (opcional)
- [ ] Menu mobile-friendly
- [ ] Teste em devices reais

#### Acessibilidade
- [ ] Suporte a teclado completo
- [ ] Contraste de cores adequado
- [ ] Sem piscar rápido
- [ ] Alt text em imagens

#### QA & Bugs
- [ ] Testes de gameplay completos
- [ ] Verificação de todos os finais
- [ ] Edge cases de interação
- [ ] Save/Load system (local storage)
- [ ] Documentação de bugs conhecidos

### Entrega
- Jogo visualmente polido
- Áudio imersivo
- Performance otimizada (60 FPS)
- Responsivo em mobile
- Pronto para release v1.0

---

## 🎯 Objetivos Por Fase

| Fase | Foco | NPCs | Mapas | Eventos | Status |
|------|------|------|-------|---------|--------|
| 1 | Core | 5 | 1 | 0 | Planejado |
| 2 | Mecânicas | 10 | 3 | 20+ | Planejado |
| 3 | Narrativa | 15+ | 7+ | 50+ | Planejado |
| 4 | Polish | 15+ | 7+ | 50+ | Planejado |

---

## 📊 Métricas de Sucesso

- ✅ Jogo rodando sem crashes
- ✅ Múltiplos finais alcançáveis
- ✅ 60 FPS em navegadores modernos
- ✅ NPCs com IA dinâmica visível
- ✅ Narrativa coerente e envolvente
- ✅ Comunidade engajada (issues, PRs)

---

## 🤝 Contribuição no Roadmap

Tem interesse em ajudar? Veja as issues abertas correspondentes a cada fase e comente se quer pegar uma tarefa.

Ver [CONTRIBUTING.md](CONTRIBUTING.md) para mais detalhes.

---

**Última atualização**: 17 de Maio, 2026