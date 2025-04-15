# Stepper Component

Um componente versátil para criação de wizards, fluxos de etapas e processos multi-estágio com diferentes orientações e variantes visuais.

## Variáveis Utilizadas

### Variáveis Core
- `--color-accent`: Cor primária para etapas ativas
- `--color-bg-tertiary`: Cor de fundo das etapas inativas
- `--color-text-primary`: Cor do texto do título
- `--color-text-secondary`: Cor do texto da descrição
- `--color-text-muted`: Cor dos indicadores inativos

### Variáveis do Componente
- `--stepper-connector-size`: Espessura da linha conectora
- `--stepper-size`: Tamanho do indicador circular
- `--stepper-icon-size`: Tamanho do ícone dentro do indicador
- `--stepper-spacing`: Espaçamento entre etapas
- `--stepper-content-spacing`: Espaçamento entre indicador e conteúdo
- `--stepper-color`: Cor principal do stepper
- `--stepper-color-inactive`: Cor dos elementos inativos
- `--stepper-bg`: Cor de fundo dos indicadores
- `--stepper-transition`: Duração da transição

## Classes

### Classes Base
```html
<div class="stepper">
  <div class="stepper__step">
    <div class="stepper__indicator">
      <!-- Ícone ou Número -->
    </div>
    <div class="stepper__content">
      <h3 class="stepper__title">Título da Etapa</h3>
      <p class="stepper__description">Descrição da etapa</p>
    </div>
  </div>
</div>
```

### Estados das Etapas
- `.stepper__step--completed`: Etapa concluída
- `.stepper__step--active`: Etapa atual
- `.stepper__step--error`: Etapa com erro
- `.stepper__step--disabled`: Etapa desabilitada

### Orientações
- `.stepper`: Horizontal (padrão)
- `.stepper--vertical`: Vertical

### Tamanhos
- `.stepper--sm`: Pequeno
- `.stepper--md`: Médio (padrão)
- `.stepper--lg`: Grande

### Variantes Visuais
- `.stepper--alt`: Estilo alternativo com bordas
- `.stepper--minimal`: Versão minimalista
- `.stepper--numbered`: Com números em vez de ícones
- `.stepper--progress`: Com efeito de preenchimento
- `.stepper--filled`: Com fundo no conteúdo
- `.stepper--glass`: Com efeito glass morphism

### Classes de Comportamento
- `.stepper--interactive`: Permite clique nas etapas
- `.stepper--animated`: Com animações de transição
- `.stepper--responsive`: Adaptativo para mobile

## Exemplos de Uso

### Stepper Básico
```html
<div class="stepper">
  <div class="stepper__step stepper__step--completed">
    <div class="stepper__indicator">
      <svg class="stepper__indicator-icon">
        <path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41L9 16.17z"/>
      </svg>
    </div>
    <div class="stepper__content">
      <h3 class="stepper__title">Informações Pessoais</h3>
      <p class="stepper__description">Preencha seus dados básicos</p>
    </div>
  </div>
  
  <div class="stepper__step stepper__step--active">
    <div class="stepper__indicator">2</div>
    <div class="stepper__content">
      <h3 class="stepper__title">Endereço</h3>
      <p class="stepper__description">Informe seu endereço</p>
    </div>
  </div>
  
  <div class="stepper__step">
    <div class="stepper__indicator">3</div>
    <div class="stepper__content">
      <h3 class="stepper__title">Confirmação</h3>
      <p class="stepper__description">Revise seus dados</p>
    </div>
  </div>
</div>
```

### Stepper Vertical com Glass Effect
```html
<div class="stepper stepper--vertical stepper--glass">
  <!-- Mesma estrutura do exemplo anterior -->
</div>
```

### Stepper Interativo com Progress
```html
<div class="stepper stepper--interactive stepper--progress">
  <!-- Mesma estrutura do exemplo anterior -->
</div>
```

## Ordem dos Modificadores
Para melhor consistência, use os modificadores nesta ordem:
1. Orientação (--vertical)
2. Tamanho (--sm, --lg)
3. Variante Visual (--alt, --minimal, etc)
4. Comportamento (--interactive, --animated)
5. Estado (--completed, --active, etc)

## Melhores Práticas
- Use ícones consistentes para cada estado
- Mantenha descrições concisas
- Considere acessibilidade (aria-*)
- Indique progresso claramente
- Use cores semânticas para estados
- Mantenha feedback visual claro
- Prefira orientação vertical em mobile
- Use --interactive quando clicável
- Considere --glass em fundos com imagem
- Mantenha número adequado de etapas
- Use animações com moderação
- Forneça feedback de erro claro
- Teste responsividade
- Valide acessibilidade via teclado
- Mantenha estados sincronizados