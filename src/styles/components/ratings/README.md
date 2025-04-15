# Rating Component

Um componente de avaliação flexível com suporte para estrelas interativas, meio-estrelas e diferentes estilos visuais.

## Variáveis Utilizadas

### Variáveis Core
- `--color-bg-tertiary`: Cor das estrelas vazias
- `--color-text-primary`: Cor do texto principal
- `--color-text-secondary`: Cor do texto secundário
- `--color-text-muted`: Cor do texto de informações adicionais
- `--color-accent`: Cor primária para variante primary

### Variáveis do Componente
- `--rating-size`: Tamanho das estrelas (default: 20px)
- `--rating-color`: Cor das estrelas ativas (default: #ffd700)
- `--rating-color-empty`: Cor das estrelas inativas
- `--rating-spacing`: Espaçamento entre estrelas

## Classes

### Classes Base
- `.rating`: Container principal
- `.rating__star`: Elemento de estrela individual
- `.rating__input`: Input nativo escondido (radio)
- `.rating__star--active`: Estado ativo da estrela
- `.rating__star--half`: Estado de meia estrela

### Variantes de Tamanho
- `.rating--xs`: Extra pequeno (16px)
- `.rating--sm`: Pequeno (20px)
- `.rating--md`: Médio (24px - padrão)
- `.rating--lg`: Grande (32px)
- `.rating--xl`: Extra grande (40px)

### Variantes de Estilo
- `.rating--interactive`: Permite interação do usuário
- `.rating--readonly`: Somente leitura
- `.rating--disabled`: Estado desativado
- `.rating--animated`: Com animação de entrada
- `.rating--compact`: Sem espaçamento entre estrelas
- `.rating--max-display`: Mostra pontuação máxima

### Variantes de Cor
- `.rating--primary`: Usa a cor de destaque
- `.rating--warning`: Usa a cor de aviso
- `.rating--success`: Usa a cor de sucesso

### Grupo com Labels
- `.rating-group`: Container com label e valor
- `.rating-group__label`: Label do grupo
- `.rating-group__value`: Valor numérico

### Rating com Texto
- `.rating-text`: Container para rating com texto
- `.rating-text__score`: Pontuação em texto
- `.rating-text__label`: Label da pontuação

## Exemplos de Uso

### Rating Básico (Somente Leitura)
```html
<div class="rating rating--readonly">
  <span class="rating__star rating__star--active"></span>
  <span class="rating__star rating__star--active"></span>
  <span class="rating__star rating__star--active"></span>
  <span class="rating__star"></span>
  <span class="rating__star"></span>
</div>
```

### Rating Interativo com Inputs Nativos
```html
<div class="rating rating--interactive">
  <input type="radio" name="rating" value="5" class="rating__input" id="star5">
  <label class="rating__star" for="star5"></label>
  
  <input type="radio" name="rating" value="4" class="rating__input" id="star4">
  <label class="rating__star" for="star4"></label>
  
  <input type="radio" name="rating" value="3" class="rating__input" id="star3">
  <label class="rating__star" for="star3"></label>
  
  <input type="radio" name="rating" value="2" class="rating__input" id="star2">
  <label class="rating__star" for="star2"></label>
  
  <input type="radio" name="rating" value="1" class="rating__input" id="star1">
  <label class="rating__star" for="star1"></label>
</div>
```

### Rating com Meio Ponto
```html
<div class="rating rating--readonly">
  <span class="rating__star rating__star--active"></span>
  <span class="rating__star rating__star--active"></span>
  <span class="rating__star rating__star--half"></span>
  <span class="rating__star"></span>
  <span class="rating__star"></span>
</div>
```

### Rating em Card
```html
<div class="rating-text">
  <span class="rating-text__score">4.8</span>
  <div class="rating rating--sm rating--readonly">
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--half"></span>
  </div>
  <span class="rating-text__label">32 avaliações</span>
</div>
```

### Rating com Label e Valor
```html
<div class="rating-group">
  <span class="rating-group__label">Avaliação</span>
  <div class="rating rating--primary rating--readonly">
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--active"></span>
    <span class="rating__star rating__star--half"></span>
    <span class="rating__star"></span>
  </div>
  <span class="rating-group__value">3.5</span>
</div>
```

## Melhores Práticas
- Use inputs nativos para ratings interativos para melhor acessibilidade
- Para ratings somente leitura, use apenas spans com classes adequadas
- Forneça sempre labels descritivos para os inputs de rating
- Use aria-label para descrever o propósito do rating quando necessário
- Mantenha a ordem dos inputs do maior para o menor valor
- Agrupe inputs relacionados com fieldset quando apropriado
- Use a variante correta de cor para indicar o contexto (success, warning, etc)
- Considere usar tooltips para mostrar descrições dos valores
- Em formulários, sempre use a versão com inputs nativos
- Para exibição de dados, use a versão somente leitura
- Mantenha consistência no uso das cores do tema
- Em layouts responsivos, use a classe rating--responsive