## [v7.0] - 2026-10-10

### Corrigido (falha crítica de usabilidade)
- **Navegação mobile inexistente.** O menu principal usava `hidden md:flex`, ou seja,
  ficava completamente oculto em telas abaixo de 768px, sem qualquer alternativa de
  acesso (sem botão hambúrguer). Resultado: usuários de celular não conseguiam navegar
  entre seções do site — apenas viam o cabeçalho sem menu algum.
- Esta falha foi identificada pelo Marcio (auditor do projeto) em revisão manual,
  e não pela IA responsável pela geração do código nas versões anteriores (v1 a v6).
  Registro mantido por honestidade de processo.

### Adicionado
- Botão de menu mobile (ícone ☰/✕) visível apenas abaixo do breakpoint `md`.
- Painel de navegação mobile com os mesmos 6 links do menu desktop.
- Atributos de acessibilidade: `aria-label`, `aria-expanded`.
- Fechamento automático do menu mobile ao selecionar qualquer link.

### Pendência ainda não resolvida
- Link "Verificar credenciamento oficial na lista da Marinha do Brasil" continua em
  `href="#"`, aguardando decisão do Marcio sobre destino real.