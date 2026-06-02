# Design Specification - Website Advocacy Firm

**Data de Criação**: 2026-06-02  
**Status**: Visual Identity Definition  
**Objetivo**: Guia completo para design e desenvolvimento do website

---

## 📐 Paleta de Cores

| Elemento | Cor | Hex | Uso |
|----------|-----|-----|-----|
| Primário Escuro | Preto Profundo | #1A1A1A | Textos principais, backgrounds |
| Secundário Quente | Marrom Executivo | #8B6F47 | Highlights, borders |
| Acento Dourado | Ouro Refinado | #C8860B | CTAs, hovers, ênfase |
| Neutro Claro | Creme Quente | #F5F0E8 | Backgrounds claros, cards |
| Cinza Corporativo | Cinza Médio | #4A4A4A | Textos secundários |
| Cinza Suave | Cinza Leve | #E8E4DB | Separadores, borders sutis |

---

## 🔤 Tipografia

### Títulos (H1, H2, H3)
- **Fonte Principal**: Playfair Display (serif elegante)
- **Backup**: Lora
- **Tamanhos**:
  - H1: 48px | font-weight: 700 | line-height: 1.2
  - H2: 36px | font-weight: 600 | line-height: 1.3
  - H3: 28px | font-weight: 600 | line-height: 1.4

### Corpo e Subtítulos
- **Fonte Principal**: Inter (sans-serif contemporânea)
- **Backup**: Open Sans
- **Tamanhos**:
  - Corpo: 16px | font-weight: 400 | line-height: 1.6
  - Pequeno: 14px | font-weight: 400 | line-height: 1.5

---

## 🎨 Componentes Reutilizáveis

### Botões
- **Primário (CTA)**: Background #C8860B | Texto #FFFFFF | Padding 12px 32px | Border-radius 4px
- **Secundário**: Border 2px #8B6F47 | Texto #8B6F47 | Background transparent
- **Hover**: Shadow 0 4px 12px rgba(200, 134, 11, 0.3) | Escala 1.02

### Cards
- Background: #FFFFFF ou #F5F0E8
- Border-radius: 8px
- Shadow: 0 4px 12px rgba(0, 0, 0, 0.1)
- Padding: 24px
- Hover: Shadow 0 8px 24px rgba(0, 0, 0, 0.15)

### Dividers
- Cor: #E8E4DB
- Altura: 1px ou 2px
- Margem: 32px 0

### Icons
- Estilo: Minimalista monocromático
- Cor padrão: #8B6F47
- Tamanho: 24px (padrão) | 32px (destaque)

---

## 📱 Layout & Grid

- **Grid Base**: 8px
- **Container Max-width**: 1200px
- **Espaçamento Horizontal**: 40px em desktop, 20px em mobile
- **Espaçamento Vertical**: 64px entre seções (32px em mobile)

---

## 📄 Estrutura das Páginas

### 1. Home
```
┌─────────────────────────────────┐
│    HERO SECTION                 │
│  (Imagem/Gradiente + Overlay)   │
│  Headline + Subheadline + CTA   │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    SERVIÇOS (3 CARDS)           │
│  Titulo | Descrição | Ícone     │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    CTA SECUNDÁRIA               │
│  "Agende uma Consulta"          │
└─────────────────────────────────┘
```

**Hero**:
- Altura: 600px (desktop) / 400px (mobile)
- Imagem: Escritório/profissional + overlay escuro 60%
- Headline: H1 color #FFFFFF
- Subheadline: 18px color #E8E4DB
- CTA Button: Primário (#C8860B)

**Serviços**:
- Layout: 3 colunas (desktop) / 1 coluna (mobile)
- Cards com hover dourado
- Ícone 32px + H3 + Descrição 14px

---

### 2. Sobre
```
┌─────────────────────────────────┐
│    MISSÃO / VISÃO / VALORES     │
│  (Com ícones discretos)         │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    TEAM (Grid de fotos)         │
│  Nome | Cargo | Descrição       │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    HISTÓRICO / CREDIBILIDADE    │
│  Timeline ou números            │
└─────────────────────────────────┘
```

---

### 3. Serviços
```
┌─────────────────────────────────┐
│    GRID DE ÁREAS DE ATUAÇÃO     │
│  (4-6 cards com ícones)         │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    DESCRIÇÃO DETALHADA          │
│  (Expandível por clique)        │
└─────────────────────────────────┘
```

---

### 4. Casos de Sucesso
```
┌─────────────────────────────────┐
│    GALERIA / TIMELINE           │
│  (3-4 cards de cases)           │
│  Título | Desafio | Resultado   │
└─────────────────────────────────┘
```

**Cards**:
- Imagen destaque
- H3 + Descrição + CTA "Ler caso"
- Hover: Aumento suave de sombra

---

### 5. Blog
```
┌─────────────────────────────────┐
│    FILTROS POR CATEGORIA        │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    GRID DE POSTS (3 cols)       │
│  Imagem | Data | Título | Leia  │
└─────────────────────────────────┘
```

---

### 6. Contato
```
┌─────────────────────────────────┐
│    FORMULÁRIO (Form)            │
│  Nome | Email | Mensagem        │
│  Botão: "Enviar"                │
└─────────────────────────────────┘
        ↓
┌─────────────────────────────────┐
│    INFORMAÇÕES DE CONTATO       │
│  Tel | Email | Endereço | Mapa  │
└─────────────────────────────────┘
```

---

## ⚡ Padrões de Interação

### Transições
- Duração padrão: 200ms
- Easing: ease-in-out
- Propriedades: opacity, transform, box-shadow

### Hover States
1. **Buttons**: +15% brilho + sombra
2. **Cards**: +sombra + transform: translateY(-4px)
3. **Links**: color #C8860B + underline

### Loading States
- Spinner: Ícone giratório em #C8860B
- Feedback visual claro

---

## 📐 Breakpoints

| Device | Width | Padding |
|--------|-------|---------|
| Desktop | 1200px+ | 40px |
| Tablet | 768px - 1199px | 30px |
| Mobile | < 768px | 20px |

---

## 🖼️ Referências Visuais Utilizadas

- Escritório Moderno e Elegante com Design Executivo
- Decoração de escritório comercial
- Swiss luxury mansion interior
- Conceito: Executivo + Sofisticado + Iluminação Quente

---

## ✅ Checklist de Implementação

### Design Visual
- [ ] Paleta de cores aprovada
- [ ] Fontes no Figma carregadas
- [ ] Home page mockup completo
- [ ] Página secundária mockup
- [ ] Design system com componentes

### Desenvolvimento
- [ ] Estrutura HTML semântica
- [ ] CSS com variáveis de cores
- [ ] Responsividade mobile-first
- [ ] Otimização de imagens
- [ ] SEO base (meta tags, headings)

### Deploy
- [ ] Domínio configurado
- [ ] Hospedagem ativa
- [ ] HTTPS ativo
- [ ] Formulário de contato funcional
- [ ] Analytics integrado

---

**Próximo Passo**: Criar mockups no Figma seguindo esta especificação
