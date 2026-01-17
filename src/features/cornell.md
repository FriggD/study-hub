# Cornell Notes System

## TODO: Implementar Sistema de Notas Cornell

### Descrição
Sistema de anotações estruturadas baseado no Método Cornell, dividindo a página em:
- Coluna de Notas (maior área, lado direito)
- Coluna de Palavras-chave/Questões (lado esquerdo)
- Área de Resumo (parte inferior)

### Funcionalidades Planejadas

#### Básicas
- [ ] Criar nova nota Cornell
- [ ] Editar notas existentes
- [ ] Salvar e carregar notas
- [ ] Estrutura de três seções (notas, keywords, resumo)

#### Intermediárias
- [ ] Adicionar tags e categorias
- [ ] Sistema de busca de notas
- [ ] Ordenação e filtros
- [ ] Exportar notas (PDF, Markdown)

#### Avançadas
- [ ] Vincular notas relacionadas
- [ ] Anexar imagens e arquivos
- [ ] Histórico de versões
- [ ] Colaboração (compartilhamento de notas)

### Estrutura de Dados

```javascript
// TODO: Definir estrutura de dados
const cornellNote = {
  id: 'uuid',
  title: 'Título da Nota',
  createdAt: 'timestamp',
  updatedAt: 'timestamp',
  mainNotes: 'Conteúdo principal...',
  keywords: 'Palavras-chave e questões...',
  summary: 'Resumo do conteúdo...',
  tags: ['tag1', 'tag2'],
  category: 'categoria',
  // TODO: Adicionar mais campos conforme necessário
};
```

### Referências
- [Método Cornell](https://en.wikipedia.org/wiki/Cornell_Notes)
