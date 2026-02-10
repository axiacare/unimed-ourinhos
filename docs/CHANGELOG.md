# Changelog - Portal de Entregas Unimed Ourinhos

## v2.5 — 2026-02-10

- **FEAT**: KPIs do Eixo 01 atualizados com números exatos: 2.852.907 lançamentos assistenciais e 8.184.951 unidades de procedimento.
- **FEAT**: Novo KPI "Unidades de Procedimento" adicionado aos destaques.
- **FIX**: Removido "Ticket Médio Geral" dos destaques (métrica sem valor para tomada de decisão).
- **FEAT**: Tooltips elegantes com hover nos KPI cards, exibindo breve explicação de cada indicador.
- **FIX**: Texto de contexto atualizado com terminologia precisa ("lançamentos assistenciais" e "unidades de procedimento").
- **DOCS**: Criado `conceitos_kpi_ourinhos.md` no repositório analytics com definições formais dos KPIs.
- **DOCS**: Atualizado `frontend_institucional.md` v9.2 com componente KPI Card com Tooltip.

## v2.4 — 2026-02-09

- **FIX**: Migração completa de domínio de `axcare.com.br` para `axcare.app` em todos os arquivos de ambos os repositórios.
- **FIX**: CNAME atualizado para `unimed094.axcare.app`.
- **FIX**: Todas as meta tags OpenGraph, links institucionais, favicons e referências de domínio atualizados.
- **FIX**: Links de footer (texto visível) atualizados de `axcare.com.br` para `axcare.app`.

## v2.3 — 2026-02-09

- **FIX (CRÍTICO)**: Corrigido o número da singular Unimed Ourinhos de `167` para `094` em todos os arquivos e repositórios. O domínio do portal foi alterado de `unimed167.axcare.com.br` para `unimed094.axcare.com.br`.
- **FIX**: Atualizado o arquivo `CNAME` para refletir o novo domínio.
- **FIX**: Corrigidas todas as meta tags OpenGraph (`og:url`, `og:image`) e `twitter:image` nos arquivos HTML.
- **FIX**: Corrigido o link do portal no `README.md` do repositório `axiacare/analytics`.

## v2.2 — 2026-02-08

- **FIX (CRÍTICO)**: Revisão completa de linguagem em 100% dos entregáveis. Removidos 14 trechos com linguagem prescritiva, opinativa ou que extrapolava o papel de consultor.
- **FIX**: Removido "comprometendo a gestão" do achado 6 do Sumário Executivo.
- **FIX**: Removido "caminho mais curto para o controle de custos" do achado 1.
- **FIX**: Substituído "desproporcionais" e "requerem" por linguagem neutra no achado 7.
- **FIX**: Substituído "devem" por "podem" em todas as implicações para a gestão.
- **FIX**: Reescrito parágrafo prescritivo sobre gestão de custos por procedimento (seção 4.1).
- **FIX**: Substituídos todos os usos de "requer" por "depende de", "será objeto de" ou "pode ser complementada".
- **FIX**: Removido adjetivo "expressivos" e "relevantes" de descrições de dados.
- **DOCS**: Criada `REGRA_LINGUAGEM_NEUTRA.md` no repositório analytics como padrão obrigatório.

## v2.1 — 2026-02-08

- **FIX**: Eixos 03 e 04 corrigidos para "Pendente" (roadmap e cards). Apenas o Eixo 02 é "Em Desenvolvimento".
- **FIX**: Nome contratual corrigido para "Unimed Ourinhos Cooperativa de Trabalho Médico" (nome oficial).
- **FEATURE**: Card do Eixo 02 agora possui diferenciação visual muito mais evidente: opacity 0.88, sem grayscale, borda azul lateral, sombra sutil e gradiente de fundo. Contraste claro com os Eixos 03/04 (opacity 0.45, grayscale 80%).

## v2.0 — 2026-02-08

- **FIX (CRÍTICO)**: Removidas previsões de datas inventadas nos cards dos Eixos 02, 03 e 04 ("Previsão: Mar/2026", "Abr/2026", "Mai/2026"). Essas datas nunca foram acordadas com o cliente.
- **FIX**: Tagline corrigida de "Cuidado em Saúde com Valor, na prática." para "Cuidados em Saúde com Valor" (acrônimo oficial CSV) em todas as 3 páginas.
- **FIX**: Status dos Eixos 03 e 04 corrigidos de "Pendente" para "Em Desenvolvimento" no roadmap e nos cards.
- **FIX**: Status dos Eixos 02, 03 e 04 corrigidos de "Em elaboração" para "Em Desenvolvimento" nos cards.
- **FEATURE**: Card do Eixo 02 agora possui visual intermediário (classe `in-progress`), mais "aceso" que os Eixos 03/04 (opacity 0.68 vs 0.45, grayscale 20% vs 80%).
- **DOCS**: Criada `REGRA_NAO_SUPOR_DADOS.md` no repositório analytics como padrão obrigatório.

## v1.9 — 2026-02-08

- **REFINEMENT (UX/CX)**: Realizada revisão completa de contraste e legibilidade em todas as páginas do portal (login, portal, eixo-01, flash-cards).
- **FIX**: Corrigido o contraste do texto "Cooperativa de Trabalho Médico de Ourinhos/SP" e "Registro ANS 31.129-4", que estava com opacidade muito baixa (rgba(255,255,255,0.3)) e agora está com opacidade adequada (rgba(255,255,255,0.6)).
- **FIX**: Corrigido o contraste da assinatura Spectra™ em todas as páginas, que estava com opacidade muito baixa (rgba(255,255,255,0.25) e opacity: 0.7) e agora está com opacidade adequada (rgba(255,255,255,0.5) e opacity: 1).
- **FIX**: Corrigido o contraste de diversos outros elementos de texto no footer e na tela de login, como o copyright, a tagline e os links.

## v1.8 — 2026-02-08

- **FEATURE**: Adicionada assinatura `Spectra™ • Inteligência Clínica para Operadoras de Saúde` em todas as páginas (login, portal, relatório Eixo 01, galeria de flash cards).
- **FEATURE**: A assinatura é clicável e direciona para `spectra.thera.tech`.
- **REFINEMENT**: O posicionamento da assinatura foi projetado para ser sutil e elegante, garantindo consistência visual e profissionalismo em todas as telas.
- **DOCS**: O padrão da assinatura foi documentado no `frontend_institucional.md` como v9.0 para replicação futura.

## v1.7 — 2026-02-08

- **FEATURE**: Carrossel de Flash Cards com auto-play, navegação por setas e dots, e barra de progresso.
- **FEATURE**: Timeline de Projeto com status visual de cada um dos 4 eixos.
- **FEATURE**: Seção de Boas-Vindas redesenhada com destaques visuais para termos-chave.
- **FEATURE**: Avisos elegantes com ícones SVG e cores contextuais.

## v1.6 — 2026-02-08

- **FEATURE**: Redesign premium v7.0 do interior do portal.
- **FEATURE**: Alinhamento visual completo do relatório Eixo 01 com o padrão do portal.
- **FIX**: Texto do footer do card de login atualizado conforme solicitação.

## v1.5 — 2026-02-08

- **FEATURE**: Redesign completo da parte interna (pós-login) com hero section, cards de eixo com barra lateral, fundos de seção alternados, e refinamentos visuais gerais.
- **FEATURE**: Adicionado badge "ENTREGA PARCIAL" no card do Eixo 01 para comunicar status com mais clareza.
- **FEATURE**: Adicionado botão "Solicitar Acesso" (mailto) na tela de login.

## v1.4 — 08/02/2026

- **Redesign Visual Completo (v5.0):**
  - **Contraste Ativo/Inativo:** Cards de eixo agora têm distinção visual clara (borda colorida, sombra, badge vs. opacidade, grayscale).
  - **Ícones Profissionais:** Ícones genéricos substituídos por SVGs contextuais para cada eixo.
  - **Toggle de Senha:** Adicionado ícone de olho no campo de senha para melhorar a usabilidade.
  - **Refinamentos Visuais:** Badges de status, tipografia, espaçamentos e footer aprimorados.
  - **Otimização Mobile:** Layout refinado em 4 breakpoints (desktop, 768px, 480px, 360px).


## Versão 1.3 (2026-02-08)

Esta atualização corrige um **erro crítico de informação sobre o período dos dados** em múltiplos artefatos.

### Correção Crítica

- **Período de dados corrigido**: Todos os documentos e flash cards afirmavam incorretamente que o período era "Faturamento: Abr/2020 a Ago/2025". O banco de dados não possui data de faturamento. As datas são de **atendimento**. O período de competência financeira dos arquivos recebidos é **Janeiro/2024 a Agosto/2025** (agosto parcial).
- **Flash Cards FC-01-001 e FC-01-003**: Geradas versões v2 com período corrigido. Versões v1 marcadas como obsoletas.
- **Relatório Eixo 01**: Período corrigido no HTML.
- **Portal e Galeria de Flash Cards**: Referências atualizadas para v2.

### Documentação

- Criada `NOTA_TECNICA_PERIODO_DADOS.md` no repositório analytics como referência obrigatória.

---

## Versão 1.2 (2026-02-08)

Esta atualização foca em **OpenGraph otimizado para WhatsApp** e **otimização avançada de mobile**.

### OpenGraph

- **Imagem OG redesenhada**: Nova imagem `og_unimed_ourinhos.png` (v3) otimizada para o formato compacto de preview do WhatsApp. Logo Unimed Ourinhos em destaque, "Portal de Entregas" em fonte grande, logos ICDS e AxiaCare na parte inferior.
- **Versão full-size**: Nova imagem `og_unimed_ourinhos_full.png` com layout editorial (duas colunas) para uso em apresentações e documentação.
- **Meta tags aprimoradas**: Adicionadas tags `og:image:width`, `og:image:height` e `og:image:type` para otimizar a leitura pelos crawlers. Cache-busting via parâmetro `?v=3`.

### Otimização Mobile

- **Breakpoint 360px**: Novo breakpoint para smartphones pequenos (Galaxy S, iPhone SE), com ajustes de padding, fontes e logos.
- **Flash Cards mobile**: Aspect-ratio ajustado para 3:4 em tablets, coluna única com largura máxima de 360px em smartphones.
- **Lightbox mobile**: Navegação reposicionada para dentro da viewport, botões de toque maiores (min-height 42px), imagem com max-height adaptativo.
- **Touch targets**: Botões de ação dos flash cards com min-height de 42px para conformidade com padrões de acessibilidade mobile.
- **Footer mobile**: Flex-wrap nos links para evitar overflow horizontal em telas estreitas.
- **Auth mobile**: Card de autenticação com margens laterais e botão com min-height de 48px.

---

## Versão 1.1 (2026-02-08)

Esta atualização foca em **consistência visual, usabilidade e correções de bugs** em todas as páginas do portal.

### Melhorias e Novas Features

- **Botão "Voltar ao Portal"**: Adicionado um botão de navegação proeminente e elegante na página do relatório do Eixo 01, permitindo que os usuários retornem facilmente à página inicial.
- **Alinhamento de Cards**: Os botões "Visualizar" e "Download" nos Flash Cards da página inicial agora estão perfeitamente alinhados na base dos cards, independentemente da altura do texto descritivo, graças à implementação de Flexbox.

### Correções de Consistência (Bug Fixes)

- **Unificação de Fontes**: Todas as páginas (Portal, Eixo 01, Flash Cards) agora utilizam a fonte padrão **Inter** via Google Fonts, eliminando o uso inconsistente de Roboto e Segoe UI.
- **Componentes Idênticos**: Headers e Footers foram completamente sincronizados entre todas as 3 páginas. Isso inclui:
    - **Logos Clicáveis**: Todas as logos no header e footer de todas as páginas agora são clicáveis e levam aos sites oficiais das respectivas entidades.
    - **Dimensionamento de Logos**: Os tamanhos das logos foram padronizados em todas as páginas e em todos os breakpoints (desktop, tablet, mobile), seguindo o `frontend_institucional.md` v4.0.
    - **CSS Unificado**: Estilos de CSS duplicados ou conflitantes foram removidos, especialmente nos arquivos do Eixo 01 e da galeria de Flash Cards.
- **Otimização Mobile**: A experiência em dispositivos móveis foi revisada e aprimorada, garantindo que a consistência visual se mantenha em telas menores.

### Infraestrutura

- **Cache de OpenGraph**: O problema de cache que exibia a imagem do Cloudflare em vez da imagem OpenGraph correta no WhatsApp foi diagnosticado. A remoção da camada de proteção do Cloudflare Access deve resolver o problema assim que o cache dos aplicativos for atualizado.
