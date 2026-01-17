# Flashcards System

## TODO: Implementar Sistema de Flashcards

### Descrição
Sistema de cartões de estudo com repetição espaçada para melhorar a retenção de conhecimento.

### Funcionalidades Planejadas

#### Básicas
- [ ] Criar novo flashcard (frente/verso)
- [ ] Editar flashcards existentes
- [ ] Organizar em decks/baralhos
- [ ] Modo de estudo/revisão

#### Intermediárias
- [ ] Algoritmo de repetição espaçada (Leitner ou SM-2)
- [ ] Rastreamento de progresso (acertos/erros)
- [ ] Estatísticas de desempenho
- [ ] Tags e categorização

#### Avançadas
- [ ] Flashcards com imagens
- [ ] Flashcards com múltipla escolha
- [ ] Modo de teste cronometrado
- [ ] Exportar/importar decks
- [ ] Compartilhar decks com outros usuários
- [ ] TODO: Integração com AI para gerar flashcards automaticamente

### Estrutura de Dados

```javascript
// TODO: Definir estrutura de dados
const flashcard = {
  id: 'uuid',
  deckId: 'deck-uuid',
  front: 'Pergunta ou conceito',
  back: 'Resposta ou explicação',
  createdAt: 'timestamp',
  lastReviewed: 'timestamp',
  nextReview: 'timestamp', // Baseado no algoritmo de repetição
  difficulty: 0, // 0-5, ajustado pelo usuário
  correctCount: 0,
  incorrectCount: 0,
  tags: ['tag1', 'tag2'],
  // TODO: Adicionar campos para algoritmo de repetição espaçada
};

const deck = {
  id: 'uuid',
  name: 'Nome do Deck',
  description: 'Descrição',
  cards: [], // Array de IDs de flashcards
  createdAt: 'timestamp',
  category: 'categoria',
  isPublic: false,
};
```

### Algoritmos de Repetição Espaçada

#### TODO: Implementar algoritmo
- **Leitner System**: Sistema simples de caixas
- **SM-2 (SuperMemo 2)**: Algoritmo mais sofisticado
- Considerar implementar ambos e permitir escolha do usuário

### Referências
- [Spaced Repetition](https://en.wikipedia.org/wiki/Spaced_repetition)
- [Leitner System](https://en.wikipedia.org/wiki/Leitner_system)
- [SuperMemo 2](https://www.supermemo.com/en/archives1990-2015/english/ol/sm2)
