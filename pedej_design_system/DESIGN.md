---
name: PedeJá Design System
colors:
  surface: '#fff8f6'
  surface-dim: '#f0d4cb'
  surface-bright: '#fff8f6'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff1ec'
  surface-container: '#ffe9e3'
  surface-container-high: '#ffe2d9'
  surface-container-highest: '#f9dcd3'
  on-surface: '#271813'
  on-surface-variant: '#5b4137'
  inverse-surface: '#3e2c26'
  inverse-on-surface: '#ffede7'
  outline: '#8f7066'
  outline-variant: '#e4beb2'
  surface-tint: '#a93800'
  primary: '#a53700'
  on-primary: '#ffffff'
  primary-container: '#ce4600'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb59b'
  secondary: '#815500'
  on-secondary: '#ffffff'
  secondary-container: '#feae20'
  on-secondary-container: '#6a4500'
  tertiary: '#005f9e'
  on-tertiary: '#ffffff'
  tertiary-container: '#0078c6'
  on-tertiary-container: '#fdfcff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#ffb59b'
  on-primary-fixed: '#380d00'
  on-primary-fixed-variant: '#812900'
  secondary-fixed: '#ffddb2'
  secondary-fixed-dim: '#ffb94d'
  on-secondary-fixed: '#291800'
  on-secondary-fixed-variant: '#624000'
  tertiary-fixed: '#d1e4ff'
  tertiary-fixed-dim: '#9dcaff'
  on-tertiary-fixed: '#001d35'
  on-tertiary-fixed-variant: '#00497c'
  background: '#fff8f6'
  on-background: '#271813'
  surface-variant: '#f9dcd3'
  primary-600: '#E04E0A'
  primary-400: '#FF7A3A'
  primary-100: '#FFF0E8'
  secondary-600: '#E89A10'
  secondary-400: '#FFC04D'
  secondary-100: '#FFF5E0'
  neutral-900: '#292929'
  neutral-700: '#4A4A4A'
  neutral-500: '#8A8A8A'
  neutral-300: '#D4D4D4'
  neutral-200: '#E8E8E8'
  neutral-100: '#F5F5F5'
  neutral-50: '#FAFAFA'
typography:
  h1:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  h3:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.5'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
  price-display:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '700'
    lineHeight: '1'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 24px
---

# PedeJá - Design System & Backlog
Documento central de design system, fluxos de usuario e especificacoes visuais para a plataforma PedeJá. Todas as telas, componentes e interacoes devem seguir rigorosamente as diretrizes deste documento.

## 1. Visao Geral da Marca
PedeJá e uma plataforma de encomendas e entregas de restaurantes, projetada para conectar clientes, restaurantes e entregadores numa experiencia unica, rapida e intuitiva.

### Atributos de Marca
| Atributo | Descricao |
| :--- | :--- |
| Energetica | Cores vibrantes que transmitem dinamismo e agilidade |
| Acessivel | Interface simples e intuitiva para qualquer usuario |
| Confiavel | Sistema robusto com transparencia em pedidos e pagamentos |
| Moderna | Design contemporaneo com foco em experiencia mobile-first |
| Apetitosa | Visual que estimula o desejo de pedir comida |

## 2. Paleta de Cores
### Cores Primarias
| Token | Hex | Uso |
| :--- | :--- | :--- |
| --primary-500 | #F95A0D | Cor principal - botoes CTA, header, acentos |
| --primary-600 | #E04E0A | Hover/estado ativo do primario |
| --primary-400 | #FF7A3AV | ersao mais clara para iluminacoes |
| --primary-100 | #FFF0E8 | Fundos sutis, backgrounds de secao |

### Cores Secundarias
| Token | Hex | Uso |
| :--- | :--- | :--- |
| --secondary-500 | #FBAC1D | Destaques, badges, precos, estrelas |
| --secondary-600 | #E89A10 | Hover do secundario |
| --secondary-400 | #FFC04D | Versao clara para iluminacoes |
| --secondary-100 | #FFF5E0 | Fundos de destaque, banners |

### Cores Neutras
| Token | Hex | Uso |
| :--- | :--- | :--- |
| --neutral-900 | #292929 | Texto principal, titulos |
| --neutral-700 | #4A4A4A | Texto secundario, descricoes |
| --neutral-500 | #8A8A8A | Texto terciario, placeholders |
| --neutral-300 | #D4D4D4 | Bordas, divisores |
| --neutral-200 | #E8E8E8 | Fundos de input, bordas suaves |
| --neutral-100 | #F5F5F5 | Fundos de secao, cards |
| --neutral-50 | #FAFAFA | Fundo da aplicacao |
| --white | #FFFFFF | Fundo de cards, superficies |

## 3. Tipografia
- Fonte principal: Inter (Google Fonts)
- Titulos: --neutral-900
- Texto descritivo: --neutral-700
- Precos: --secondary-500 (Peso 700)

## 4. Bordas e Sombras
- radius-sm: 8px
- radius-md: 12px
- radius-lg: 16px
- radius-xl: 24px
- radius-full: 9999px
- shadow-md: 0 4px 6px -1px rgba(0,0,0,0.08)

## 6. Componentes Base
### 6.1 Botoes
- Botao Primario: Fundo --primary-500, Texto --white, Radius radius-full (pill)
- Botao Secundario: Fundo --white, Texto --primary-500, Borda 2px solid --primary-500, Radius radius-full

### 6.3 Cards
- Card de Restaurante: Fundo --white, Radius radius-lg (16px), Sombra shadow-md. Imagem topo 16:9.
- Card de Item/Produto: Fundo --white, Radius radius-md (12px), Imagem 1:1.

### 6.5 Navegacao
- Bottom Navigation (Mobile): Fundo --white, Altura 64px, 4-5 items (Inicio, Busca, Pedidos, Perfil). Ativo --primary-500.