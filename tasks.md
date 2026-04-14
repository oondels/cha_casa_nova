# Tarefas — Chá de Casa Nova

## Animações & Transições

- [x] Scroll Reveal — Intersection Observer no Hero (stagger: nome → subtítulo → data → botão)
- [x] Scroll Reveal — fade-in + translate-Y em todas as seções ao entrar no viewport
- [x] Scroll Reveal — gift cards com stagger (0 / 100ms / 200ms) fade + slide-up
- [x] Scroll Reveal — "Como Funciona": 3 passos em cascata da esquerda para direita
- [x] Scroll Reveal — seção Evento: texto entra da esquerda, imagem entra da direita
- [x] Separadores SVG wave/curve entre seções (substituir transições de cor abruptas)
- [x] Navbar: começa transparente, transição suave para `bg-surface/90 + sombra` ao scrollar 80px
- [x] Navbar: item ativo muda conforme seção visível (Intersection Observer)
- [x] Navbar: menu hambúrguer mobile com animação slide-down suave
- [x] Hero: efeito parallax suave no gradient ao mover o mouse
- [x] Hero: botão CTA com pulsação suave (keyframe scale 1 → 1.03 → 1, loop infinito)
- [x] Gift cards: glow ring sutil na borda ao hover (`box-shadow: 0 0 0 2px rgba(142, 76, 62, 0.2)`)
- [x] Gift cards: overlay de cor primária opacity 0 → 0.05 na imagem ao hover

## Funcionalidades

- [x] Lista de presentes: substituir cards hardcoded por array de dados em JS (mínimo 9–12 itens)
- [x] Lista de presentes: renderização dinâmica dos cards via JavaScript
- [x] Filtros de categoria: clicar no filtro filtra os cards (fade-out/scale-down nos excluídos, fade-in/scale-up nos incluídos)
- [x] Filtros de categoria: botão ativo com estilo visual distinto
- [x] Barra de progresso: cálculo dinâmico de "X de Y itens presenteados"
- [x] Barra de progresso: animação de preenchimento ao entrar no viewport
- [x] Modal "Presentear": abrir ao clicar no botão de card disponível
- [x] Modal "Presentear": exibir nome, imagem e valor do item
- [x] Modal "Presentear": botão "Abrir WhatsApp" com link pré-formatado
- [x] Modal "Presentear": animação de entrada (scale 0.95 → 1 + fade-in) e backdrop blur
- [x] Modal RSVP: formulário com Nome, Telefone, Nº de pessoas e restrição alimentar
- [x] Modal RSVP: validação dos campos obrigatórios
- [x] Modal RSVP: botão de envio abre WhatsApp com dados formatados
- [x] Modal RSVP: feedback visual de sucesso após envio

## Refinamentos Visuais

- [x] `scroll-margin-top: 80px` em todas as seções (compensar navbar sticky)
- [x] Corrigir typo `''Localização` → `Localização` na seção Evento
- [x] Botão "voltar ao topo": oculto por padrão, aparece com fade-in após scrollar 400px
- [x] Adicionar meta tags Open Graph (og:title, og:description, og:image)

## Mobile

- [x] Menu hambúrguer funcional no mobile
- [x] Modais "Presentear" e RSVP responsivos no mobile
