# Changelog — ETNPF Marcio Site

Todas as alterações relevantes deste projeto são documentadas neste arquivo.

## [7.1] - 2026-10-11

### Corrigido
- Link "Verificar credenciamento oficial na lista da Marinha do Brasil" (index.html):
  anteriormente apontava para `href="#"` (placeholder sem destino). Agora aponta
  para o PDF oficial da Marinha do Brasil (lista de estabelecimentos náuticos
  credenciados na CPSP), com abertura em nova aba (`target="_blank"`) e atributo
  de segurança `rel="noopener noreferrer"`.
- Bug de visibilidade do link acima: o texto só aparecia ao passar o mouse
  (hover). Corrigido fixando a cor do texto (`text-[#c9a227]`) e o sublinhado
  (`underline`) como estado padrão, mantendo apenas a transição de cor no hover
  (`hover:text-white`) como efeito visual.

## [7.0] - 2026-10-10

### Adicionado
- Página `area-aluno.html`: estrutura visual da área do aluno (header, menu,
  card de login), preparando o terreno para autenticação real na Fase 2.
- Imagens institucionais do site: foto do instrutor (hero), sala de aula
  teórica, documentação de barco, colete salva-vidas, simulados online e
  sobre a escola.
- Logos oficiais da ETNPF Marcio (versões 2018 e 2018a).

### Planejado (Fase 2)
- Autenticação real de aluno (login/senha).
- Integração com banco de dados (Supabase ou Firebase) para simulados e
  histórico de desempenho.
- Uso de variáveis de ambiente no painel do Cloudflare Pages para proteção
  de chaves de API (nunca versionadas no código).
