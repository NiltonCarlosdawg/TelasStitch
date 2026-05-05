# PedeJá - Backlog Técnico

## 1. Visão Geral do Projeto

**PedeJá** é uma plataforma de delivery que conecta clientes, restaurantes e entregadores numa experiência unificada de encomendas e entregas de comida.

### Atributos de Marca

| Atributo | Descrição |
| :--- | :--- |
| Energética | Cores vibrantes que transmitem dinamismo e agilidade |
| Acessível | Interface simples e intuitiva para qualquer usuário |
| Confiável | Sistema robusto com transparência em pedidos e pagamentos |
| Moderna | Design contemporâneo com foco em experiência mobile-first |
| Apetitosa | Visual que estimula o desejo de pedir comida |

---

## 2. Arquitetura do Sistema

### 2.1 Aplicações

| Aplicação | Plataforma | Propósito |
| :--- | :--- | :--- |
| **Mobile App** | iOS/Android | Cliente + Entregador |
| **Web Dashboard** | Web | Admin + Restaurante |

### 2.2 Estrutura Mobile App

```
Mobile/
├── src/
│   ├── app/                    # expo-router
│   │   ├── (auth)/            # Login, Seleção perfil
│   │   ├── (client)/          # Tab navigation Cliente
│   │   │   ├── index.tsx      # Home
│   │   │   ├── search.tsx    # Busca
│   │   │   ├── orders.tsx    # Pedidos
│   │   │   └── profile.tsx   # Perfil
│   │   ├── (delivery)/       # Tab navigation Entregador
│   │   │   ├── index.tsx     # Início
│   │   │   ├── orders.tsx    # Entregas disponíveis
│   │   │   └── earnings.tsx # Ganhos
│   │   ├── restaurant/[id]/ # Detalhes restaurante
│   │   └── cart/
│   ├── components/ui/
│   ├── features/client/
│   ├── features/delivery/
│   ├── services/api.ts
│   └── store/
```

### 2.3 Estrutura Web Dashboard

```
web-dashboard/
├── src/
│   ├── main.tsx
│   ├── App.tsx
│   ├── app/                  # React Router v7
│   │   ├── admin/           # /admin
│   │   │   └── page.tsx
│   │   ├── restaurant/      # /dashboard-restaurante
│   │   │   ├── menu/
│   │   │   └── orders/
│   │   ├── login/
│   │   └── layout.tsx
│   ├── components/ui/
│   ├── features/
│   ├── services/api.ts
│   └── store/
├── index.html
├── vite.config.ts
└── tailwind.config.js
```

---

## 3. Design System

### 3.1 Paleta de Cores

#### Cores Primárias

| Token | Hex | Uso |
| :--- | :--- | :--- |
| `--primary-500` | #F95A0D | Cor principal - botões CTA, header, acentos |
| `--primary-600` | #E04E0A | Hover/estado ativo do primário |
| `--primary-400` | #FF7A3A | Versão mais clara para iluminações |
| `--primary-100` | #FFF0E8 | Fundos sutis, backgrounds de seção |

#### Cores Secundárias

| Token | Hex | Uso |
| :--- | :--- | :--- |
| `--secondary-500` | #FBAC1D | Destaques, badges, preços, estrelas |
| `--secondary-600` | #E89A10 | Hover do secundário |
| `--secondary-400` | #FFC04D | Versão clara para iluminações |
| `--secondary-100` | #FFF5E0 | Fundos de destaque, banners |

#### Cores Neutras

| Token | Hex | Uso |
| :--- | :--- | :--- |
| `--neutral-900` | #292929 | Texto principal, títulos |
| `--neutral-700` | #4A4A4A | Texto secundário, descrições |
| `--neutral-500` | #8A8A8A | Texto terciário, placeholders |
| `--neutral-300` | #D4D4D4 | Bordas, divisores |
| `--neutral-200` | #E8E8E8 | Fundos de input, bordas suaves |
| `--neutral-100` | #F5F5F5 | Fundos de seção, cards |
| `--neutral-50` | #FAFAFA | Fundo da aplicação |
| `--white` | #FFFFFF | Fundo de cards, superf��cies |

### 3.2 Tipografia

| Estilo | Fonte | Tamanho | Peso | Line Height |
| :--- | :--- | :--- | :--- | :--- |
| `h1` | Inter | 32px | 700 | 1.2 |
| `h2` | Inter | 24px | 700 | 1.3 |
| `h3` | Inter | 20px | 600 | 1.4 |
| `body-lg` | Inter | 18px | 400 | 1.5 |
| `body-md` | Inter | 16px | 400 | 1.5 |
| `body-sm` | Inter | 14px | 400 | 1.4 |
| `label-caps` | Inter | 12px | 600 | 1 |
| `price-display` | Inter | 20px | 700 | 1 |

### 3.3 Espaçamento

| Token | Valor |
| :--- | :--- |
| `xs` | 4px |
| `sm` | 8px |
| `md` | 16px |
| `lg` | 24px |
| `xl` | 32px |
| `2xl` | 48px |

### 3.4 Bordas

| Token | Valor |
| :--- | :--- |
| `sm` | 8px |
| `md` | 12px |
| `lg` | 16px |
| `xl` | 24px |
| `full` | 9999px |

### 3.5 Componentes Base

#### Botões

- **Primário**: Fundo #F95A0D, Texto #FFFFFF, Radius full (pill)
- **Secundário**: Fundo #FFFFFF, Texto #F95A0D, Borda 2px solid #F95A0D, Radius full

#### Cards

- **Card de Restaurante**: Fundo #FFFFFF, Radius lg (16px), Sombra. Imagem topo 16:9
- **Card de Item/Produto**: Fundo #FFFFFF, Radius md (12px), Imagem 1:1

#### Navegação

- **Bottom Navigation**: Fundo #FFFFFF, Altura 64px, 4-5 items. Ativo #F95A0D.

---

## 4. Páginas Existentes (HTML)

### 4.1 Cliente

| Página | Arquivo | Descrição |
| :--- | :--- | :--- |
| Home 1 | pedej_home_1 | Página inicial |
| Home 2 | pedej_home_2 | Versão alternativa |
| Home 3 | pedej_home_3 | Versão alternativas |
| Home Angola 1 | pedej_home_angola_1 | Versão Angola |
| Home Angola 2 | pedej_home_angola_2 | Versão Angola |
| Home Dark Mode | pedej_home_dark_mode | Modo escuro |
| Restaurante 1 | pedej_restaurante_1 | Cardápio restaurante |
| Restaurante 2 | pedej_restaurante_2 | Versão alternativa |
| Restaurante Angola 1 | pedej_restaurante_angola_1 | Versão Angola |
| Restaurante Angola 2 | pedej_restaurante_angola_2 | Versão Angola |
| Restaurante Dark Mode | pedej_restaurante_dark_mode | Modo escuro |
| Carrinho 1 | pedej_carrinho_1 | Carrinho de compras |
| Carrinho 2 | pedej_carrinho_2 | Versão alternativa |
| Carrinho Angola | pedej_carrinho_angola | Versão Angola |
| Carrinho Dark Mode | pedej_carrinho_dark_mode | Modo escuro |
| Perfil 1 | pedej_perfil_e_configura_es | Perfil e configurações |
| Perfil 2 | pedej_perfil_angola | Versão Angola |
| Perfil 3 | pedej_sele_o_de_perfil | Seleção de perfil |
| Perfil 4 | pedej_configura_es_de_perfil | Configurações perfil |
| Perfil Dark Mode | pedej_perfil_dark_mode | Modo escuro |
| Acompanhamento 1 | pedej_acompanhamento_1 | Tracking pedido |
| Acompanhamento 2 | pedej_acompanhamento_2 | Versão alternativa |
| Acompanhamento Angola | pedej_acompanhamento_angola | Versão Angola |
| Acompanhamento Dark Mode | pedej_acompanhamento_dark_mode | Modo escuro |
| Filtro de Cozinhas | pedej_filtro_de_cozinhas | Filtros busca |
| Culinária Angolana | pedej_culin_ria_angolana | Culinária local |
| Lista Restaurantes Angola | pedej_lista_de_restaurantes_angola | Lista Angola |
| Favoritos Angola | pedej_favoritos_angola | Favoritos |
| Gerenciar Endereços | pedej_gerenciar_endere_os_angola | Endereços entrega |

### 4.2 Restaurante/Gestor

| Página | Arquivo | Descrição |
| :--- | :--- | :--- |
| Dashboard | pedej_dashboard_restaurante | Painel controle |
| Gerir Cardápio | pedej_gerir_card_pio | Gestão menu |
| Food Delivery Flow 1 | pedej_food_delivery_flow_1 | Fluxo entrega |
| Food Delivery Flow 2 | pedej_food_delivery_flow_2 | Fluxo entrega |
| Food Delivery Flow 3 | pedej_food_delivery_flow_3 | Fluxo entrega |

### 4.3 Entregador

| Página | Arquivo | Descrição |
| :--- | :--- | :--- |
| Início Entregador | pedej_in_cio_entregador | Dashboard entregador |
| Ganhos | pedej_ganhos_do_entregador | Rendimentos |

### 4.4 Admin

| Página | Arquivo | Descrição |
| :--- | :--- | :--- |
| Painel Admin | pedej_admin_painel | Administração |

---

## 5. Stack de Dependências

### 5.1 Mobile App

| Categoria | Dependência | Versão |
| :--- | :--- | :--- |
| **Core** | `expo` | ^53+ |
| | `expo-router` | ^4+ |
| | `react` | 19.x |
| | `react-native` | latest |
| **Navegação** | `@react-navigation/native` | ^7+ |
| | `@react-navigation/native-stack` | ^7+ |
| | `@react-navigation/bottom-tabs` | ^7+ |
| | `react-native-screens` | ^4+ |
| | `react-native-safe-area-context` | ^5+ |
| **UI** | `react-native-paper` | ^5+ |
| | `@expo/vector-icons` | built-in |
| | `expo-image` | ^2+ |
| | `lottie-react-native` | ^7+ |
| **Estado** | `@reduxjs/toolkit` | ^2+ |
| | `react-redux` | ^5+ |
| | `redux-thunk` | ^2+ |
| | `@tanstack/react-query` | ^5+ |
| | `axios` | ^1+ |
| | `@react-native-async-storage/async-storage` | ^2+ |
| **Animações** | `react-native-gesture-handler` | ^2+ |
| | `react-native-reanimated` | ^4+ |
| **Utils** | `expo-location` | ^18+ |
| | `expo-image-picker` | ^16+ |

### 5.2 Web Dashboard

| Categoria | Dependência | Versão |
| :--- | :--- | :--- |
| **Core** | `vite` | ^6+ |
| | `@vitejs/plugin-react` | ^4+ |
| | `react` | 19.x |
| | `react-dom` | 19.x |
| | `react-router-dom` | ^7+ |
| **UI** | `tailwindcss` | ^4+ |
| | `@tailwindcss/forms` | latest |
| | `clsx` | ^2+ |
| | `tailwind-merge` | ^2+ |
| **Estado** | `@reduxjs/toolkit` | ^2+ |
| | `react-redux` | ^5+ |
| | `redux-thunk` | ^2+ |
| | `@tanstack/react-query` | ^5+ |
| | `axios` | ^1+ |
| **Auth** | `next-auth` | ^4+ |
| | `@auth0/auth0-react` | ^3+ |
| **Utils** | `date-fns` | ^4+ |
| | `react-hook-form` | ^7+ |
| | `zod` | ^3+ |
| | `lucide-react` | ^0.400+ |

---

## 6. Fluxo de Funcionalidades

### 6.1 Cliente

1. **Home** → Search → Filtros → Lista Restaurantes
2. → Restaurante → Cardápio → Produto → Adicionar ao Carrinho
3. Carrinho → Checkout → Pedido
4. Acompanhamento → Detalhes Pedido
5. Perfil → Pedidos → Favoritos → Endereços → Configurações

### 6.2 Entregador

1. **Início** → Ver Entregas Disponíveis
2. → Aceitar Entrega → Detalhes Entrega
3. → Entregar → Confirmar → Ganhos

### 6.3 Restaurante/Gestor

1. **Dashboard** → Ver Pedidos Recebidos
2. → Gerir Cardápio → Adicionar/Editar Produtos
3. → Histórico de Pedidos

### 6.4 Admin

1. **Painel** → Gestão de Restaurantes
2. → Gestão de Entregadores
3. → Estatísticas

---

## 7. Prioridades de Desenvolvimento

### Fase 1: Mobile Cliente

- [ ] Configuração projeto Expo
- [ ] Theme/Design System (colors, typography, spacing)
- [ ] Componentes UI base (Button, Card, Input, BottomNav)
- [ ] HomeScreen
- [ ] RestaurantScreen
- [ ] CartScreen
- [ ] ProfileScreen

### Fase 2: Mobile Entregador

- [ ] DeliveryTab
- [ ] Início Entregador
- [ ] Entregas disponíveis
- [ ] Tela de Ganhos

### Fase 3: Web Dashboard Restaurante

- [ ] Configuração Vite + React
- [ ] Dashboard Restaurante
- [ ] Gestão de Cardápio
- [ ] Lista de Pedidos

### Fase 4: Web Dashboard Admin

- [ ] Painel Admin
- [ ] Gestão de Restaurantes
- [ ] Gestão de Entregadores
- [ ] Estatísticas

---

## 9. Estrutura de API (Backend)

### 9.1 Base URL

```
https://pedej-api-{hash}.herokuapp.com/api/v1
```

### 9.2 Headers Padrão

```javascript
{
  "Content-Type": "application/json",
  "Authorization": "Bearer {token}"
}
```

### 9.3 Endpoints

#### Auth

| Endpoint | Método | Descrição |
| :--- | :--- | :--- |
| `/auth/login` | POST | Login de usuário |
| `/auth/register` | POST | Registro de novo usuário |
| `/auth/profile` | GET | Obter perfil do usuário |
| `/auth/profile` | PUT | Atualizar perfil |

#### Restaurantes

| Endpoint | Método | Descrição |
| :--- | :--- | :--- |
| `/restaurants` | GET | Listar restaurantes |
| `/restaurants/{id}` | GET | Detalhes de restaurante |
| `/restaurants/{id}/products` | GET | Produtos do restaurante |
| `/restaurants/{id}/categories` | GET | Categorias do restaurante |

#### Pedidos

| Endpoint | Método | Descrição |
| :--- | :--- | :--- |
| `/orders` | POST | Criar novo pedido |
| `/orders` | GET | Listar pedidos do usuário |
| `/orders/{id}` | GET | Detalhes do pedido |
| `/orders/{id}/status` | PUT | Atualizar status do pedido |

#### Usuários

| Endpoint | Método | Descrição |
| :--- | :--- | :--- |
| `/users/addresses` | GET | Listar endereços |
| `/users/addresses` | POST | Adicionar endereço |
| `/users/profile` | PUT | Atualizar perfil |

#### Entregador

| Endpoint | Método | Descrição |
| :--- | :--- | :--- |
| `/deliveries/available` | GET | Listar entregas disponíveis |
| `/deliveries/{id}/accept` | POST | Aceitar entrega |
| `/deliveries/earnings` | GET | Ver ganhos |

### 9.4 Services (Frontend)

#### Mobile (src/services/api.ts)

```typescript
import axios from 'axios';

const BASE_URL = 'https://pedej-api-{hash}.herokuapp.com/api/v1';

const api = axios.create({
  baseURL: BASE_URL,
  headers: { 'Content-Type': 'application/json' },
});

api.interceptors.request.use((config) => {
  const token = await AsyncStorage.getItem('token');
  if (token) config.headers.Authorization = `Bearer ${token}`;
  return config;
});

// Auth API
export const authApi = {
  login: (credentials: any) => api.post('/auth/login', credentials),
  register: (data: any) => api.post('/auth/register', data),
  getProfile: () => api.get('/auth/profile'),
  updateProfile: (data: any) => api.put('/auth/profile', data),
};

// Restaurant API
export const restaurantApi = {
  list: (params?: any) => api.get('/restaurants', { params }),
  getById: (id: string) => api.get(`/restaurants/${id}`),
  getProducts: (id: string) => api.get(`/restaurants/${id}/products`),
  getCategories: (id: string) => api.get(`/restaurants/${id}/categories`),
};

// Order API
export const orderApi = {
  create: (data: any) => api.post('/orders', data),
  list: () => api.get('/orders'),
  getById: (id: string) => api.get(`/orders/${id}`),
  updateStatus: (id: string, status: string) => api.put(`/orders/${id}/status`, { status }),
};

// User API
export const userApi = {
  getAddresses: () => api.get('/users/addresses'),
  addAddress: (data: any) => api.post('/users/addresses', data),
  updateProfile: (data: any) => api.put('/users/profile', data),
};

// Delivery API
export const deliveryApi = {
  getAvailable: () => api.get('/deliveries/available'),
  acceptDelivery: (id: string) => api.post(`/deliveries/${id}/accept`),
  getEarnings: () => api.get('/deliveries/earnings'),
};

export default api;
```

#### Web (src/services/api.ts)

Estrutura idêntica ao Mobile, adaptados para ambiente web.

---

### 9.5 Autenticação

- Token JWT armazenado em AsyncStorage (Mobile) / localStorage (Web)
- Incluído em todas as requisições via interceptor
- Refresh token handled pelo backend

---

## 10. Referências

- Código existente: `./pedej_*` (34 páginas HTML)
- Design System: `./pedej_design_system/DESIGN.md`
- Dark Mode: `./pedej_dark/DESIGN.md`
- Vibrant Delivery: `./vibrant_delivery/DESIGN.md`
- Imagem API: `./IMG-20260504-WA0118.jpg`

---

*Documento gerado em: 2026-05-04*