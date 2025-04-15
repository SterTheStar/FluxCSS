# Timeline Component

Um componente para exibir eventos ou atividades em ordem cronológica.

## Variáveis Utilizadas

### Variáveis Core
- `--color-text-primary`: Cor do título
- `--color-text-secondary`: Cor da descrição
- `--color-text-muted`: Cor da data
- `--color-bg-primary`: Fundo dos itens no tema moderno
- `--color-bg-secondary`: Fundo padrão dos itens
- `--color-border`: Cor da linha do timeline e bordas
- `--color-accent`: Cor de destaque (dots, conectores)
- `--color-success`: Cor alternativa para dots no tema colorido
- `--color-warning`: Cor alternativa para dots no tema colorido
- `--border-radius-md`: Borda dos cards
- `--shadow-sm`: Sombra dos cards
- `--spacing-xs`: Espaçamento pequeno
- `--spacing-sm`: Espaçamento médio-pequeno
- `--spacing-md`: Espaçamento médio
- `--spacing-lg`: Espaçamento grande
- `--spacing-xl`: Espaçamento extra grande
- `--spacing-xxl`: Espaçamento duplo extra grande
- `--transition-fast`: Velocidade da animação
- `--color-accent-rgb`: Valores RGB da cor de destaque (para sombras)
- `--color-border-rgb`: Valores RGB da cor da borda (para transparência)
- `--border-radius-full`: Borda circular para conectores
- `--shadow-md`: Sombra média para efeitos de hover

## Classes

### Classes Base
- `.timeline`: Container principal
- `.timeline__item`: Item individual do timeline
- `.timeline__dot`: Marcador circular
- `.timeline__content`: Container do conteúdo
- `.timeline__title`: Título do evento
- `.timeline__date`: Data do evento
- `.timeline__description`: Descrição do evento

### Variantes
- `.timeline--alternate`: Layout alternado (esquerda/direita)
- `.timeline--connected`: Dots conectados com linhas e efeitos de profundidade
- `.timeline--modern`: Visual moderno com hover effects e gradientes
- `.timeline--compact`: Layout mais compacto
- `.timeline--colored`: Dots e conectores com cores alternadas

## Exemplos de Uso

```html
<!-- Timeline Básico -->
<div class="timeline">
  <div class="timeline__item">
    <div class="timeline__dot"></div>
    <div class="timeline__content">
      <h3 class="timeline__title">Título do Evento</h3>
      <div class="timeline__date">10 Jan 2024</div>
      <p class="timeline__description">Descrição do evento aqui</p>
    </div>
  </div>
</div>

<!-- Timeline Alternado -->
<div class="timeline timeline--alternate">
  <div class="timeline__item">
    <!-- Mesma estrutura do exemplo básico -->
  </div>
  <div class="timeline__item">
    <!-- Mesma estrutura do exemplo básico -->
  </div>
</div>

<!-- Timeline Moderno com Cores -->
<div class="timeline timeline--modern timeline--colored">
  <div class="timeline__item">
    <!-- Mesma estrutura do exemplo básico -->
  </div>
</div>

<!-- Timeline Conectado Moderno -->
<div class="timeline timeline--connected timeline--modern">
  <div class="timeline__item">
    <div class="timeline__dot"></div>
    <div class="timeline__content">
      <h3 class="timeline__title">Título do Evento</h3>
      <div class="timeline__date">10 Jan 2024</div>
      <p class="timeline__description">Descrição do evento aqui</p>
    </div>
  </div>
</div>

<!-- Timeline Combinado com Cores -->
<div class="timeline timeline--modern timeline--connected timeline--colored">
  <div class="timeline__item">
    <!-- Mesma estrutura do exemplo básico -->
  </div>
</div>
```

## Funcionalidades
- Layout vertical padrão
- Layout alternado (esquerda/direita)
- Marcadores conectados
- Efeitos de hover
- Variantes de cores
- Design responsivo
- Versão compacta para conteúdos densos
- Suporte a conteúdo rico nos cards
- Efeitos de profundidade com sombras e gradientes
- Conectores animados e responsivos
- Transições suaves em interações
- Suporte a backdrop-filter para efeitos de vidro

## Boas Práticas
- Use o layout alternado apenas quando houver espaço suficiente
- Mantenha os textos concisos para melhor legibilidade
- Considere usar a versão compacta para muitos itens
- Combine variantes para criar estilos únicos
- Use cores consistentes com sua identidade visual
- Garanta contraste adequado entre textos e fundos
- Aproveite os efeitos de profundidade para criar hierarquia visual
- Use gradientes e sombras com moderação
- Considere a performance ao usar múltiplos efeitos visuais

## Comportamento Responsivo
Em telas menores que 640px:
- Layout alternado se converte em layout vertical
- Mantém a legibilidade do conteúdo
- Preserva todas as informações importantes
- Adapta espaçamentos para melhor visualização mobile