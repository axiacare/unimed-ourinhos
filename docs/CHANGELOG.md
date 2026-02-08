# Changelog - Portal de Entregas Unimed Ourinhos

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
