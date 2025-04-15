# Avatar Component

Um componente versátil para exibição de avatares de usuário e chips de perfil, com múltiplas variantes e estados.

## Variáveis Utilizadas

### Variáveis Core
- `--color-bg-secondary`: Background do profile chip
- `--color-bg-tertiary`: Background do avatar e bordas
- `--color-text-primary`: Cor do texto principal
- `--color-text-muted`: Cor do texto secundário e ícones
- `--color-accent`: Estados ativos e hover
- `--color-success`: Status online
- `--color-error`: Status ocupado
- `--color-warning`: Status ausente

### Variáveis do Componente
- `--avatar-size`: Tamanho do avatar (default: 40px)
- `--avatar-font-size`: Tamanho da fonte das iniciais
- `--avatar-border`: Espessura da borda (default: 2px)

## Classes

### Classes Base
- `.avatar`: Container principal do avatar
- `.avatar__image`: Imagem do avatar
- `.avatar__initials`: Iniciais do usuário (fallback)
- `.avatar__status`: Indicador de status

### Variantes de Tamanho
- `.avatar--xs`: Extra pequeno (24px)
- `.avatar--sm`: Pequeno (32px)
- `.avatar--md`: Médio (40px - padrão)
- `.avatar--lg`: Grande (48px)
- `.avatar--xl`: Extra grande (64px)

### Variantes de Estilo
- `.avatar--rounded`: Bordas levemente arredondadas
- `.avatar--square`: Bordas quadradas
- `.avatar--bordered`: Com borda
- `.avatar--interactive`: Com efeitos de hover

### Estados de Status
- `.avatar__status--online`: Online (verde)
- `.avatar__status--offline`: Offline (cinza)
- `.avatar__status--busy`: Ocupado (vermelho)
- `.avatar__status--away`: Ausente (amarelo)

### Grupo de Avatares
- `.avatar-group`: Container para grupo de avatares

### Profile Chip
- `.profile-chip`: Container do chip
- `.profile-chip__content`: Wrapper do conteúdo
- `.profile-chip__name`: Nome do usuário
- `.profile-chip__info`: Informação adicional
- `.profile-chip__action`: Botão de ação

### Variantes do Profile Chip
- `.profile-chip--compact`: Versão compacta
- `.profile-chip--accent`: Com cor de destaque
- `.profile-chip--glass`: Efeito glass morphism
- `.profile-chip--selected`: Estado selecionado
- `.profile-chip--responsive`: Adaptativo para mobile

## Exemplos de Uso

### Avatar Básico
```html
<div class="avatar">
  <img class="avatar__image" src="user.jpg" alt="User">
</div>
```

### Avatar com Iniciais
```html
<div class="avatar">
  <span class="avatar__initials">JD</span>
</div>
```

### Avatar com Status
```html
<div class="avatar">
  <img class="avatar__image" src="user.jpg" alt="User">
  <span class="avatar__status avatar__status--online"></span>
</div>
```

### Grupo de Avatares
```html
<div class="avatar-group">
  <div class="avatar"><img src="user1.jpg" alt="User 1"></div>
  <div class="avatar"><img src="user2.jpg" alt="User 2"></div>
  <div class="avatar"><img src="user3.jpg" alt="User 3"></div>
</div>
```

### Profile Chip
```html
<div class="profile-chip">
  <div class="avatar avatar--sm">
    <img class="avatar__image" src="user.jpg" alt="User">
  </div>
  <div class="profile-chip__content">
    <span class="profile-chip__name">John Doe</span>
    <span class="profile-chip__info">Online</span>
  </div>
  <button class="profile-chip__action">×</button>
</div>
```

### Profile Chip com Glass Effect
```html
<div class="profile-chip profile-chip--glass">
  <div class="avatar avatar--sm">
    <span class="avatar__initials">JD</span>
  </div>
  <div class="profile-chip__content">
    <span class="profile-chip__name">John Doe</span>
    <span class="profile-chip__info">Admin</span>
  </div>
</div>
```

## Melhores Práticas
- Use a classe `avatar--interactive` apenas quando o avatar for clicável
- Forneça uma imagem alternativa ou iniciais como fallback
- Mantenha as iniciais curtas (máximo 2 caracteres)
- Use status apenas quando necessário
- Em grupos de avatares, limite a quantidade para manter a legibilidade
- Para profile chips responsivos, use a classe `profile-chip--responsive`
- Considere usar `profile-chip--glass` em fundos com imagem ou gradiente