# 🤝 Guia de Contribuição

Obrigado por se interessar em contribuir para **Childhood Balance**! Este documento descreve como você pode ajudar a fazer deste jogo algo especial.

---

## 📋 Código de Conduta

Este projeto segue um [Código de Conduta](CODE_OF_CONDUCT.md) para garantir um ambiente seguro e acolhedor. Leia-o antes de contribuir.

---

## 🎯 Como Contribuir

### 1. Reportar Bugs

Encontrou um problema? Abra uma [Issue](https://github.com/lucianx71/childhood-balance/issues) com:

- **Título descritivo**: "[BUG] Jogador não colide com NPCs"
- **Descrição clara**: O que acontece vs. o que deveria acontecer
- **Passos para reproduzir**: Como você fez o bug acontecer
- **Ambiente**: Navegador, SO, dispositivo
- **Screenshots/GIFs**: Se aplicável

### 2. Sugerir Features

Tem uma ideia? Abra uma [Issue](https://github.com/lucianx71/childhood-balance/issues) com:

- **Título**: "[FEATURE] Sistema de amizade visual"
- **Descrição**: Por que isso seria legal?
- **Exemplo**: Como deveria funcionar?
- **Alternativas**: Outras abordagens que você pensou

### 3. Código

Quer contribuir com código? Ótimo!

#### Setup

```bash
# Fork o repositório (clique em Fork no GitHub)
git clone https://github.com/SEU-USERNAME/childhood-balance.git
cd childhood-balance
git remote add upstream https://github.com/lucianx71/childhood-balance.git
```

#### Criar Branch

```bash
# Sempre crie uma branch nova
git checkout -b feature/sua-feature
# ou
git checkout -b fix/seu-bug
```

**Nomes de branch:**
- Features: `feature/nome-descritivo`
- Bugs: `fix/nome-descritivo`
- Documentação: `docs/nome-descritivo`
- Performance: `perf/nome-descritivo`

#### Código

**Padrões:**
- Use JavaScript vanilla (sem frameworks)
- Nomes descritivos em português
- Funções puras quando possível
- Máximo 80 caracteres por linha
- Indentação com 2 espaços

**Exemplo bom:**
```javascript
/**
 * Calcula distância entre dois pontos
 * @param {Object} ponto1 - {x, y}
 * @param {Object} ponto2 - {x, y}
 * @returns {number} Distância euclidiana
 */
function calcularDistancia(ponto1, ponto2) {
  const dx = ponto2.x - ponto1.x;
  const dy = ponto2.y - ponto1.y;
  return Math.sqrt(dx * dx + dy * dy);
}
```

#### Commits

**Mensagens claras:**
```
feat: adicionar sistema de reputação
fix: corrigir colisão de jogador com NPCs
docs: atualizar README com instruções
refactor: otimizar renderização de canvas
test: adicionar testes de diálogo
style: formatar código conforme padrão
```

**Use imperative mood:**
- ✅ "Add feature" (não "Added feature")
- ✅ "Fix bug" (não "Fixed bug")

#### Pull Request

```bash
# Antes de enviar, sincronize com upstream
git fetch upstream
git rebase upstream/main

# Push sua branch
git push origin feature/sua-feature
```

**Abra PR com:**
- Título descritivo
- Descrição do que mudou
- Closes #123 (se fecha uma issue)
- Screenshots/GIFs se visual
- Checklist:
  - [ ] Testei localmente
  - [ ] Segui padrão de código
  - [ ] Atualizei documentação
  - [ ] Não quebrei nada existente

### 4. Documentação

Melhorias na documentação são muito bem-vindas!

- README.md - Informações gerais
- ROADMAP.md - Plano de desenvolvimento
- Comentários no código - Explicar lógica complexa
- Wikis - Guias de desenvolvimento

### 5. Sprites & Assets

Tem talento em pixel art?

**Diretrizes:**
- Resolução: 32x32 pixels (base)
- Paleta: Max 16 cores primárias
- Estilos: Pixel art limpo, sem anti-aliasing
- Formatos: PNG com transparência

**NPCs:**
- 4 sprites (cima, baixo, esquerda, direita)
- Animação de caminhada (4 frames)
- Emotes (feliz, triste, neutro, confuso)

**Tilesets:**
- Urbano, rural, praia, floresta
- Consistência com paleta geral

**Envie via:**
- Pull Request com arquivo em `/assets/sprites/`
- ou crie uma Issue com screenshot

---

## 📂 Estrutura de Pastas

```
/
├── /assets          # Sprites, áudio, fontes
├── /scripts         # Lógica do jogo modularizada
├── /styles         # CSS organizado por componente
├── /ui             # Componentes de interface
├── /maps           # Dados de mapas (JSON)
├── /dialogues      # Sistema de diálogos
├── /data           # Dados de NPCs, itens, eventos
└── index.html      # Arquivo principal
```

---

## 🔧 Desenvolvimento Local

### Servidor Local

**Python:**
```bash
python3 -m http.server 8000
```

**Node:**
```bash
npx http-server
```

**Node + Reload automático:**
```bash
npx http-server -c-1  # sem cache
```

Abra: http://localhost:8000

### Dev Tools

- Chrome DevTools (F12)
- Console para logs
- Network tab para assets
- Performance profiling

---

## ✅ Checklist Antes de Submeter

- [ ] Código roda sem erros
- [ ] Testei em Chrome/Firefox/Safari
- [ ] Sem console warnings ou errors
- [ ] Segui padrão de código
- [ ] Adicionei comentários em código complexo
- [ ] Atualizei documentação relevante
- [ ] Commits com mensagens claras
- [ ] Sem arquivos desnecessários
- [ ] Performance aceitável (60 FPS)

---

## 🚀 Tipos de Contribuição Bem-Vindos

✅ Bug fixes
✅ Novas features
✅ Melhorias de código
✅ Documentação
✅ Pixel art & assets
✅ Música & sons
✅ Testes
✅ Performance optimization
✅ Ideias & feedback

---

## 💬 Comunicação

### GitHub
- **Issues**: Bug reports, features, discussões
- **Discussions**: Ideias, perguntas, brainstorm
- **PRs**: Para propostas de código

### Comunidade
- Seja respeitoso
- Abra à feedback
- Reconheça contribuições de outros
- Aprenda com erros

---

## 📚 Recursos Úteis

- [Canvas API MDN](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [Game Dev Articles](https://www.gamedev.net/)
- [Pixel Art Tips](https://lospec.com/pixel-art-tutorials/)
- [JavaScript Modern](https://javascript.info/)

---

## 🎓 Aprendizado

Primeira vez contribuindo em open source?

- Comece por [good first issues](https://github.com/lucianx71/childhood-balance/issues?q=label%3A%22good+first+issue%22)
- Leia o código existente
- Não tenha medo de perguntar
- Pequenas PRs são OK

---

## 🏆 Reconhecimento

Contribuidores são listados em:
- README.md
- CONTRIBUTORS.md
- Créditos do jogo
- GitHub contributors page

---

## ❓ Dúvidas?

- Abra uma [Discussion](https://github.com/lucianx71/childhood-balance/discussions)
- Comente em uma Issue
- Crie uma Issue com [QUESTION] no título

---

**Obrigado por fazer parte da comunidade Childhood Balance!** 🎮✨

Esperamos seu código, arte e ideias!