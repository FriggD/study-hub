# Gamification System

## TODO: Implementar Sistema de Gamificação

### Descrição
Sistema de gamificação saudável para incentivar constância, foco e engajamento nos estudos, sem criar dependência ou ansiedade.

### Princípios

- **Motivação Intrínseca**: Foco no aprendizado, não apenas em pontos
- **Progresso Visual**: Feedback claro sobre evolução
- **Recompensas Significativas**: Conquistas que reflitam esforço real
- **Sem Punições**: Falhas não penalizam, apenas oportunidades de melhoria
- **Saúde Mental**: Evitar FOMO, comparação tóxica ou vício

### Funcionalidades Planejadas

#### Sistema de Pontos (XP)
- [ ] Ganhar XP por atividades:
  - Criar nota Cornell: 10 XP
  - Revisar flashcards: 5 XP por deck
  - Completar sessão de estudo: 20 XP
  - Criar mapa mental: 15 XP
  - Completar revisão agendada: 25 XP
- [ ] Multiplicadores por consistência
- [ ] Visualização de XP total e histórico

#### Sistema de Níveis
- [ ] Níveis baseados em XP acumulado
- [ ] Títulos por nível (Iniciante, Estudante, Dedicado, Mestre, etc.)
- [ ] Desbloquear funcionalidades ou temas por nível
- [ ] Animações de subida de nível

#### Conquistas (Achievements)
- [ ] Conquistas por marcos:
  - "Primeira Nota": Criar primeira nota Cornell
  - "Estudioso": 7 dias de streak
  - "Dedicado": 30 dias de streak
  - "Maratonista": Estudar 10 horas em uma semana
  - "Revisor": Revisar 100 flashcards
  - "Mestre dos Mapas": Criar 5 mapas mentais
- [ ] Badges visuais
- [ ] Conquistas secretas/raras
- [ ] TODO: Conquistas sazonais ou de eventos

#### Streaks (Sequências)
- [ ] Contador de dias consecutivos de estudo
- [ ] Visualização de calendário de atividade (estilo GitHub)
- [ ] Proteção de streak (1-2 dias de tolerância)
- [ ] Histórico de melhor streak
- [ ] Notificação suave para manter streak

#### Desafios (Opcional)
- [ ] Desafios diários/semanais
- [ ] Objetivos personalizáveis
- [ ] Progresso em tempo real
- [ ] Recompensas ao completar desafios

### Estrutura de Dados

```javascript
// TODO: Definir estrutura de dados
const userGamification = {
  userId: 'user-uuid',
  xp: 0,
  level: 1,
  currentStreak: 0,
  longestStreak: 0,
  lastActivity: 'timestamp',
  achievements: [
    {
      id: 'achievement-id',
      unlockedAt: 'timestamp',
      notified: true,
    },
  ],
  statistics: {
    totalNotesCreated: 0,
    totalFlashcardsReviewed: 0,
    totalMindMapsCreated: 0,
    totalStudyMinutes: 0,
  },
};

const achievement = {
  id: 'uuid',
  name: 'Nome da Conquista',
  description: 'Descrição do que foi conquistado',
  icon: 'icon-name',
  rarity: 'common|rare|epic|legendary',
  condition: {
    type: 'streak|count|time',
    target: 7, // Exemplo: 7 dias de streak
  },
  xpReward: 50,
  secret: false,
};

const challenge = {
  id: 'uuid',
  title: 'Desafio Semanal',
  description: 'Revise 50 flashcards esta semana',
  type: 'daily|weekly|monthly',
  startDate: 'timestamp',
  endDate: 'timestamp',
  progress: 0,
  target: 50,
  xpReward: 100,
};
```

### Níveis e XP

TODO: Definir progressão de níveis (exemplos):
- Nível 1: 0 XP
- Nível 2: 100 XP
- Nível 3: 250 XP
- Nível 4: 500 XP
- Nível 5: 1000 XP
- ... (curva exponencial ou logarítmica)

### Considerações de Design

#### O que FAZER
- ✅ Celebrar progresso e conquistas
- ✅ Visualizar evolução de forma clara
- ✅ Fornecer feedback positivo
- ✅ Permitir desativar gamificação se desejado
- ✅ Foco na jornada, não na competição

#### O que EVITAR
- ❌ Tabelas de líderes públicas (pode criar ansiedade)
- ❌ Punições por inatividade
- ❌ Comparação forçada com outros
- ❌ Notificações excessivas ou agressivas
- ❌ FOMO (Fear of Missing Out)

### TODO: Integração com AI
- Sugestões personalizadas de desafios
- Análise de padrões para motivação
- Recomendações de metas realistas

### Referências
- [Gamification in Education](https://en.wikipedia.org/wiki/Gamification_of_learning)
- [Self-Determination Theory](https://en.wikipedia.org/wiki/Self-determination_theory)
- [Duolingo's Gamification (estudo de caso)](https://blog.duolingo.com/)
