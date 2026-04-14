# Chá de Casa Nova — Landing Page

## Visão Geral

Landing page celebrativa para o **Chá de Casa Nova** de Hendrius & [Nome da Noiva], criada para reunir convidados, exibir a lista de presentes e facilitar a confirmação de presença no evento.

O projeto é uma **single-page application** com design elegante, animações suaves e experiência mobile-first.

---

##  Objetivo

Substituir o tradicional convite impresso por uma experiência digital bonita e funcional que:

- Apresenta o casal e a história deles
- Exibe a **lista de presentes** com status em tempo real (disponível / já presenteado)
- Permite filtrar presentes por categoria
- Informa os detalhes do evento
- Recebe confirmações de presença (RSVP)

---

##  Identidade Visual

| Atributo | Valor |
|---|---|
| **Estética** | Luxury editorial — revista de design de interiores meets celebração íntima |
| **Tom** | Romântico, aconchegante, sofisticado |
| **Background** | Creme quente `#FAF7F2` |
| **Acento primário** | Rosa antigo `#C9897A` |
| **Acento secundário** | Terracota `#8B4A3C` |
| **Verde sage** | `#9BAF9A` |
| **Dourado** | `#C9A96E` |
| **Tipografia display** | Serif elegante (ex: Playfair Display, Cormorant) |
| **Tipografia corpo** | Sans-serif limpa (ex: DM Sans, Jost) |

---

## Estrutura da Página

### 1. `Hero`
- Tela cheia com gradient mesh ou textura sutil
- Nome do casal em tipografia grande
- Subtítulo "Chá de Casa Nova" com ornamento decorativo
- Data e local do evento
- CTA: **"Ver Lista de Presentes"**
- Animação de entrada no headline

### 2. `Nossa História`
- Mensagem romântica do casal
- Layout lado a lado (foto + texto)
- Elementos ilustrativos decorativos (folhas, flores, casinha)

### 3. `Lista de Presentes`  (seção principal)
- Grid de cards (3 colunas desktop / 1-2 mobile)
- Cada card contém:
  - Ilustração / ícone do item
  - Nome do item
  - Categoria
  - Valor aproximado
  - Badge de status: `Disponível` ou `Já presenteado`
- Hover effect nos cards (lift + glow)
- **Filtros por categoria** em tabs no topo
- Barra de progresso: `X de Y itens já presenteados`

**Categorias:**
- Cozinha
- Quarto
- Sala
- Banheiro
- Decoração
- Eletrodomésticos

### 4. `Como Funciona`
- 3 passos visuais: Escolha um item → Avise-nos → Apareça na festa
- Ícone + texto curto para cada passo

### 5. `Detalhes do Evento`
- Data, horário, endereço
- Botão de RSVP / confirmação de presença

### 6. `Footer`
- Nome do casal + ícone de coração/casinha
- _"Feito com amor para nossa nova casa"_

---

## Interações & Animações

- Scroll suave entre seções
- Navbar sticky: transparente → sólida no scroll
- Cards de presente: lift + sombra no hover
- Botões: scale + transição de cor no hover
- Entrada animada dos elementos ao entrar na viewport (scroll-triggered)
- Botão flutuante "voltar ao topo"
- Textura grain/linho sutil no background

---

## Responsividade

- **Mobile-first**
- Grid de presentes: 1 coluna (mobile) → 2 colunas (tablet) → 3 colunas (desktop)
- Navbar colapsa em menu hambúrguer no mobile

---

## Lista de Presentes — Estrutura de Dados

Cada item da lista segue este modelo:

```json
{
  "id": "001",
  "name": "Jogo de Panelas",
  "category": "cozinha",
  "icon": "🍳",
  "estimatedValue": "R$ 350",
  "status": "available", // "available" | "gifted"
  "priority": "high" // "high" | "medium" | "low"
}
```

---

## Stack Técnica (prevista)

| Camada | Tecnologia |
|---|---|
| Framework | HTML/CSS/JS puro **ou** Vue 3 |
| Animações | CSS Animations + Intersection Observer API |
| Fontes | Google Fonts (Playfair Display + DM Sans) |
| Ícones | Lucide Icons ou SVG próprios |
| Deploy | Vercel / Netlify / GitHub Pages |

---

## Status do Projeto

- [x] Definição do design system e paleta de cores
- [x] Estrutura de seções definida
- [x] Prompt de design gerado para o Google Stitch
- [x] Design visual gerado no Stitch
- [x] Implementação do HTML/CSS base
- [ ] Componente de lista de presentes com filtros
- [ ] Lógica de status dos presentes
- [ ] RSVP funcional
- [ ] Responsividade completa
- [ ] Deploy

---

## Contexto

**Evento:** Chá de Casa Nova  
**Casal:** Hendrius & [Nome da Noiva]  
**Data do evento:** a definir  
**Prazo do projeto:** ~2 meses