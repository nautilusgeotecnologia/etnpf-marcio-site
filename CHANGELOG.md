Changelog — ETNPF Marcio Site
Todas as alterações relevantes deste projeto são documentadas neste arquivo.

[7.2] - 2026-10-11
Adicionado
Página do simulado (/simulado): botão "Início" na tela de questão, permitindo ao aluno voltar para a tela de configuração/escolha de assuntos (com confirmação antes de descartar progresso em andamento).
Página do simulado (/simulado): botão "Início" na tela de resultado, com a mesma função de retorno à configuração.
Página do simulado (/simulado): cabeçalho institucional completo replicado (logo, menu desktop, menu mobile com botão hambúrguer), igual ao padrão usado na home e nas demais páginas do site, garantindo identidade visual e navegação consistentes em todo o site.
Script de toggle do menu mobile (btnMenuMobile / menuMobile) incorporado ao JS da página do simulado.
CSS do estado do menu mobile (#menuMobile / .aberto) incorporado ao <style> da página do simulado.

Ajustado
Links do menu de navegação do simulado (Curso Arrais, Documentação Náutica, Como Funciona, Sobre, Contato) alterados de âncoras locais (#cursos) para âncoras absolutas apontando para a home (/#cursos), já que a página do simulado está fora do index.html.
Script do Tailwind da página do simulado padronizado para https://myhub.ia.br/canvas-vendor/tailwind.js, alinhado ao CDN usado nas demais páginas do site.

Esclarecido / Pendente
Confirmado que o cadastro de alunos é armazenado no Supabase (banco Postgres), e não no front-end nem em localStorage.
Pendente: identificar e documentar o nome exato da tabela e os campos usados no cadastro de alunos — depende do trecho de código da página de cadastro (ex: supabase.from('nome_da_tabela').insert(...)) ser compartilhado para confirmação.

[7.1] - 2026-10-11
Corrigido
Link "Verificar credenciamento oficial na lista da Marinha do Brasil" (index.html): anteriormente apontava para href="#" (placeholder sem destino). Agora aponta para o PDF oficial da Marinha do Brasil (lista de estabelecimentos náuticos credenciados na CPSP), com abertura em nova aba (target="_blank") e atributo de segurança rel="noopener noreferrer".
Bug de visibilidade do link acima: o texto só aparecia ao passar o mouse (hover). Corrigido fixando a cor do texto (text-[#c9a227]) e o sublinhado (underline) como estado padrão, mantendo apenas a transição de cor no hover (hover:text-white) como efeito visual.

[7.0] - 2026-10-10
Adicionado
Página area-aluno.html: estrutura visual da área do aluno (header, menu, card de login), preparando o terreno para autenticação real na Fase 2.
Imagens institucionais do site: foto do instrutor (hero), sala de aula teórica, documentação de barco, colete salva-vidas, simulados online e sobre a escola.
Logos oficiais da ETNPF Marcio (versões 2018 e 2018a).

Planejado (Fase 2)
Autenticação real de aluno (login/senha).
Integração com banco de dados (Supabase ou Firebase) para simulados e histórico de desempenho.
Uso de variáveis de ambiente no painel do Cloudflare Pages para proteção de chaves de API (nunca versionadas no código).
