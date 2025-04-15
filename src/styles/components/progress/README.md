# Progress Component

Um conjunto completo de componentes para exibição de progresso e estados de carregamento, incluindo barras de progresso lineares, circulares, spinners e loaders animados.

## Variáveis Utilizadas

### Variáveis Core
- `--color-accent`: Cor primária dos indicadores
- `--color-bg-tertiary`: Cor de fundo dos indicadores
- `--color-text-primary`: Cor do texto principal
- `--color-text-secondary`: Cor do texto secundário
- `--transition-normal`: Duração da transição padrão
- `--animation-smooth`: Timing function padrão

### Variáveis do Componente
- `--progress-height`: Altura da barra de progresso
- `--progress-color`: Cor da barra de progresso
- `--progress-bg`: Cor de fundo
- `--progress-duration`: Duração das animações
- `--progress-timing`: Timing function das animações
- `--progress-border-radius`: Borda arredondada
- `--circle-size`: Tamanho do progresso circular
- `--circle-thickness`: Espessura do círculo
- `--spinner-size`: Tamanho do spinner
- `--spinner-thickness`: Espessura do spinner
- `--spinner-speed`: Velocidade da animação
- `--dot-size`: Tamanho dos dots
- `--dot-speed`: Velocidade da animação dos dots
- `--pulse-size`: Tamanho do pulso
- `--pulse-speed`: Velocidade da animação do pulso

## Classes

### Barra de Progresso Linear
```html
<!-- Básica -->
<div class="progress">
  <div class="progress__bar" style="--value: 45%"></div>
</div>

<!-- Com Label -->
<div class="progress-group">
  <div class="progress-group__header">
    <span class="progress-group__label">Progresso</span>
    <span class="progress-group__value">45%</span>
  </div>
  <div class="progress">
    <div class="progress__bar" style="--value: 45%"></div>
  </div>
</div>

<!-- Indeterminada -->
<div class="progress progress--indeterminate">
  <div class="progress__bar"></div>
</div>

<!-- Listrada Animada -->
<div class="progress progress--striped progress--animated">
  <div class="progress__bar" style="--value: 65%"></div>
</div>
```

### Progresso Circular
```html
<!-- Básico -->
<div class="progress-circle" style="--circumference: 151; --offset: 45">
  <svg class="progress-circle__svg">
    <circle class="progress-circle__background" cx="50%" cy="50%" r="24"/>
    <circle class="progress-circle__progress" cx="50%" cy="50%" r="24"/>
  </svg>
</div>

<!-- Com Label -->
<div class="progress-circle" style="--circumference: 151; --offset: 45">
  <svg class="progress-circle__svg">
    <circle class="progress-circle__background" cx="50%" cy="50%" r="24"/>
    <circle class="progress-circle__progress" cx="50%" cy="50%" r="24"/>
  </svg>
  <span class="progress-circle__label">45%</span>
</div>
```

### Spinners e Loaders
```html
<!-- Spinner -->
<div class="spinner"></div>

<!-- Dots -->
<div class="dots">
  <div class="dots__dot"></div>
  <div class="dots__dot"></div>
  <div class="dots__dot"></div>
</div>

<!-- Pulse -->
<div class="pulse"></div>
```

## Variantes

### Tamanhos
- `.progress--sm`: Pequeno
- `.progress--md`: Médio (padrão)
- `.progress--lg`: Grande
- `.progress--xl`: Extra grande

### Cores
- `.progress--primary`: Cor de destaque
- `.progress--success`: Verde
- `.progress--warning`: Amarelo
- `.progress--error`: Vermelho
- `.progress--info`: Azul

### Estilos
- `.progress--rounded`: Bordas arredondadas
- `.progress--square`: Bordas quadradas
- `.progress--striped`: Com listras
- `.progress--animated`: Animação das listras
- `.progress--indeterminate`: Estado indeterminado
- `.progress--glass`: Efeito glass morphism

### Estados
- `.progress--disabled`: Estado desabilitado
- `.progress--responsive`: Adaptativo para mobile

## Tamanhos dos Spinners
- `.spinner--xs`: Extra pequeno (16px)
- `.spinner--sm`: Pequeno (24px)
- `.spinner--md`: Médio (32px - padrão)
- `.spinner--lg`: Grande (48px)
- `.spinner--xl`: Extra grande (64px)

## Tamanhos dos Dots
- `.dots--sm`: Pequeno (6px)
- `.dots--md`: Médio (8px - padrão)
- `.dots--lg`: Grande (10px)

## Tamanhos do Pulse
- `.pulse--sm`: Pequeno (16px)
- `.pulse--md`: Médio (24px - padrão)
- `.pulse--lg`: Grande (32px)

## Cálculo do Progresso Circular

Para o progresso circular, você precisa calcular o `circumference` e `offset`:

```javascript
const radius = 24; // Raio do círculo
const circumference = 2 * Math.PI * radius;
const offset = circumference - (progress / 100) * circumference;

// Aplicar no elemento
element.style.setProperty('--circumference', circumference);
element.style.setProperty('--offset', offset);
```

## Melhores Práticas
- Use sempre labels descritivos
- Forneça feedback visual adequado
- Mantenha consistência nas cores
- Use indeterminado para carregamentos
- Considere acessibilidade (aria-*)
- Adapte o tamanho ao contexto
- Anime com moderação
- Use glass effect com parcimônia
- Prefira spinners para carregamentos curtos
- Use barras para progresso mensurável
- Considere dots para carregamentos leves
- Mantenha animações suaves
- Forneça estados de fallback
- Teste em diferentes viewports