# Changelog - Portal de Entregas Unimed Ourinhos

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
