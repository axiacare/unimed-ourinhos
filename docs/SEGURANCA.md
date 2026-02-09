# Avaliação de Segurança — GitHub Pages

**Data:** 2026-02-07  
**Responsável:** AxiaCare / Grupo CSV  
**Escopo:** Repositório `axiacare/unimed-ourinhos` publicado via GitHub Pages

---

## 1. Contexto

Este repositório é público e publicado via GitHub Pages no domínio `unimed094.axcare.app`. O conteúdo é estático (HTML, CSS, JavaScript client-side) e não possui backend, banco de dados ou autenticação server-side.

---

## 2. Proteção por Senha — Viabilidade Técnica

### Conclusão: Não viável nativamente

O GitHub Pages serve conteúdo estático. Não há mecanismo nativo para autenticação ou proteção por senha. Qualquer pessoa com a URL pode acessar o conteúdo publicado.

### Alternativas avaliadas

| Alternativa | Viabilidade | Complexidade | Limitações |
|-------------|-------------|--------------|------------|
| **Autenticação client-side (JavaScript)** | Baixa | Baixa | Senha exposta no código-fonte; proteção trivialmente contornável |
| **Serviço externo (Cloudflare Access, Auth0)** | Alta | Média | Requer infraestrutura externa e configuração adicional |
| **Repositório privado + GitHub Pages** | Média | Baixa | Requer GitHub Enterprise ou plano pago da organização |
| **Controle por obscuridade** | Média | Nenhuma | URLs longas e não indexadas; sem garantia de sigilo |
| **Publicação seletiva** | Alta | Nenhuma | Publicar apenas o que pode ser público; manter sensível no analytics |

### Recomendação

A abordagem mais segura e pragmática é a **publicação seletiva**: manter no repositório público apenas conteúdo que pode ser acessado por qualquer pessoa, e restringir conteúdo sensível ao repositório privado `axiacare/analytics`.

Caso proteção por senha seja necessária no futuro, a opção mais robusta é **Cloudflare Access** (já que o domínio utiliza Cloudflare para DNS), que permite adicionar autenticação sem alterar a infraestrutura do repositório.

---

## 3. Riscos Identificados

| Risco | Severidade | Mitigação |
|-------|-----------|-----------|
| Conteúdo público acessível a qualquer pessoa | Média | Publicação seletiva; curadoria humana obrigatória |
| Indexação por mecanismos de busca | Baixa | Arquivo `robots.txt` com restrições; `noindex` meta tags |
| Dados sensíveis publicados acidentalmente | Alta | Revisão obrigatória antes de cada commit; nenhum dado bruto no repositório |
| URLs compartilhadas sem controle | Baixa | Aceitável para conteúdo institucional |

---

## 4. Medidas Implementadas

1. **Arquivo `robots.txt`** — Solicita que mecanismos de busca não indexem o conteúdo
2. **Meta tag `noindex`** — Presente nas páginas HTML para reforçar não-indexação
3. **Curadoria humana** — Nenhum conteúdo é publicado sem decisão explícita do responsável técnico
4. **Separação de repositórios** — Dados brutos e código analítico permanecem em `axiacare/analytics` (privado)
5. **Nenhum dado pessoal** — O conteúdo publicado contém apenas análises agregadas, sem dados de beneficiários

---

## 5. Decisões Pendentes (Stakeholder Humano)

- Avaliar necessidade de Cloudflare Access para proteção adicional
- Definir política de retenção de conteúdo publicado
- Definir se relatórios futuros terão classificação de confidencialidade

---

*Documento de uso interno. Não constitui garantia de segurança absoluta.*
