# Mind Maps System

## TODO: Implementar Sistema de Mapas Mentais

### Descrição
Sistema para criar e visualizar mapas mentais, permitindo organização hierárquica de conceitos e ideias.

### Funcionalidades Planejadas

#### Básicas
- [ ] Criar nó central
- [ ] Adicionar nós filhos/ramificações
- [ ] Editar texto dos nós
- [ ] Deletar nós
- [ ] Conectar nós

#### Intermediárias
- [ ] Personalizar cores e estilos de nós
- [ ] Adicionar ícones e emojis
- [ ] Expandir/colapsar ramificações
- [ ] Zoom e pan (navegação)
- [ ] Salvar e carregar mapas

#### Avançadas
- [ ] Exportar como imagem (PNG, SVG)
- [ ] Exportar como Markdown ou texto
- [ ] Importar de outros formatos
- [ ] Modo de apresentação
- [ ] Compartilhar mapas mentais
- [ ] Colaboração em tempo real
- [ ] TODO: Vincular com notas Cornell ou flashcards

### Estrutura de Dados

```javascript
// TODO: Definir estrutura de dados
const mindMapNode = {
  id: 'uuid',
  text: 'Conteúdo do nó',
  parentId: 'parent-uuid', // null para nó raiz
  children: [], // Array de IDs dos nós filhos
  position: { x: 0, y: 0 }, // Posição no canvas
  style: {
    color: '#ffffff',
    backgroundColor: '#3498db',
    fontSize: 14,
    icon: null,
  },
  metadata: {
    createdAt: 'timestamp',
    updatedAt: 'timestamp',
  },
};

const mindMap = {
  id: 'uuid',
  title: 'Título do Mapa Mental',
  rootNodeId: 'root-uuid',
  nodes: [], // Array de todos os nós
  createdAt: 'timestamp',
  updatedAt: 'timestamp',
  tags: ['tag1', 'tag2'],
};
```

### Bibliotecas a Considerar

TODO: Avaliar e escolher biblioteca para visualização:
- **D3.js**: Flexível, mas requer mais trabalho
- **vis.js**: Boa para grafos e redes
- **MindMap.js**: Específica para mapas mentais
- **Cytoscape.js**: Poderosa para visualizações de grafos

### Referências
- [Mind Mapping](https://en.wikipedia.org/wiki/Mind_map)
- [Tony Buzan's Mind Mapping](https://www.tonybuzan.com/about/mind-mapping/)
