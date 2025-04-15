# FluxCSS

Um sistema de tema CSS modular e completo com vários componentes e utilitários para aplicações web modernas.

## Índice

- [Variáveis Principais](#variáveis-principais)
- [Componentes](#componentes)
- [Instalação](#instalação)
- [Uso](#uso)
- [Contribuições](#contribuições)
- [Licença](#licença)

## Variáveis Principais

### Cores
```css
--color-bg-primary: #121212;
--color-bg-secondary: #1e1e1e;
--color-bg-tertiary: #2d2d2d;
--color-text-primary: #ffffff;
--color-text-secondary: rgba(255, 255, 255, 0.85);
--color-text-muted: rgba(255, 255, 255, 0.6);
--color-text-active: #000000;
--color-accent: #ffffff;
--color-success: #4caf50;
--color-error: #ff4d4d;
--color-warning: #ff9800;
--color-info: #2196f3;
```

### Tipografia
```css
--font-size-xs: 0.75rem;
--font-size-sm: 0.875rem;
--font-size-md: 1rem;
--font-size-lg: 1.125rem;
--font-size-xl: 1.25rem;
--font-size-2xl: 1.5rem;
```

### Espaçamento
```css
--spacing-xs: 0.25rem;
--spacing-sm: 0.5rem;
--spacing-md: 1rem;
--spacing-lg: 1.5rem;
--spacing-xl: 2rem;
--spacing-2xl: 3rem;
```

### Raio de Borda
```css
--border-radius-sm: 4px;
--border-radius-md: 6px;
--border-radius-lg: 8px;
--border-radius-full: 9999px;
```

### Sombras
```css
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
```

### Camadas de Z-index
```css
--z-negative: -1;
--z-elevate: 1;
--z-dropdown: 1000;
--z-sticky: 1020;
--z-fixed: 1030;
--z-modal-backdrop: 1040;
--z-modal: 1050;
--z-popover: 1060;
--z-tooltip: 1070;
--z-toast: 1080;
```

### Transições & Animações
```css
--transition-fast: 150ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-normal: 200ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-slow: 350ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-bounce: 500ms cubic-bezier(0.68, -0.55, 0.265, 1.55);
--animation-smooth: cubic-bezier(0.4, 0, 0.2, 1);
--animation-bounce: cubic-bezier(0.34, 1.56, 0.64, 1);
--animation-spring: cubic-bezier(0.68, -0.6, 0.32, 1.6);
```

## Componentes

- Acordeões
- Alertas
- Badges
- Breadcrumbs
- Botões
- Calendário
- Cartões
- Carrossel
- Paleta de Comandos
- Menu de Contexto
- Diálogo
- Dropdowns
- Upload de Arquivos
- Formulários
- Entradas
- Modais
- Navbar
- Notificações
- Paginação
- Select
- Sidebar
- Skeletons
- Slider
- Spinners
- Tabelas
- Abas
- Titlebar
- Toasts
- Tooltips
- Árvore

## Sistema de Layout

Breakpoints responsivos:
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;
```

### Variáveis Específicas de Componentes

#### Controles de Formulário
```css
--input-height: 2.5rem;
--input-spacing: 0.75rem;
--input-border-width: 1px;
--input-focus-ring-width: 2px;
```

#### Componentes de Layout
```css
--header-height: 4rem;
--sidebar-width: 16rem;
--sidebar-collapsed-width: 4rem;
```

## Instalação

1. Copie o diretório `src/styles` para o seu projeto.
2. Importe o arquivo CSS principal:

```css
@import 'caminho/para/styles/index.css';
```

## Uso

Cada componente é modular e pode ser importado separadamente. O arquivo principal `index.css` importa todos os componentes por padrão. Para usar componentes específicos, importe individualmente.

### Exemplo Básico
```html
<button class="btn btn-primary">Clique em Mim</button>
<div class="alert alert-success">Mensagem de Sucesso</div>
<div class="card">Conteúdo do Card</div>
```

## Contribuições

Sinta-se à vontade para contribuir enviando pull requests ou criando issues para bugs e solicitações de recursos.

## Licença

FluxCSS é disponibilizado sob uma **licença personalizada** e é oferecido **"no estado em que se encontra"**, sem garantias de qualquer tipo.

Você pode usá-lo em projetos **pessoais ou não comerciais**.

Para **uso comercial**, entre em contato: [esther@dmc.chat](mailto:esther@dmc.chat)