# Contexto Operacional — IA / Gemini (.gemini)

_Base De Conhecimento e Registro de Contexto Arquitetural para o Agente_

Este documento contém o estado do site e orientações rígidas sobre como atualizar e manter este repositório focando na metodologia definida de _Design Tokens_ baseados em _Atomic Design_ construídos para o projeto.

## Perfil da Solução

- **Cliente:** Dr. Nelson Tupinambá (Escritório de Advocacia)
- **Objetivo do Site:** Alta conversão, apresentação de autoridade e contato direto (Whatsapp de conversão no topo e rodapé).
- **Aparência Exigida:** Revolucionária. Não deve parecer um site amador, mas uma Landing Page elegante, construída em modo escuro/navy ou claro minimalista, mas optou-se pela agressividade profissional do Dark Theme c/ Gold Accent.

## Manutenção do Código — Regras para Agentes

1.  **HTML/CSS/JS (Vanilla-First):** O stack deste software é estaticamente forte.
    - **Não Instale Dependências JS.** As microinterações (hover nos botões, surgimentos nos `.card`, animações do `nav`) estão desenhadas no próprio CSS (`transform`, `opacity`, `transition`). O Javascript deve apenas lidar com o acionador (`observer.observe`).
    - **Variáveis Globais:** Todas as mudanças de cor ou espaçamento **SÃO OBRIGATORIAMENTE FEITAS** na raiz do documento `.css` sob a pseudo-classe `:root`. Não crie novas classes ou adicione cores injetadas na mão; obedeça a escala de cinzas `slate` da Tailwind (que transpomos manualmente).

2.  **Imagens:**
    - Estão organizadas no HTML apontando sempre relativo (ex: `src="dr-nelson.png"`).
    - A classe `.profile-img` gerencia tudo utilizando nativamente `object-fit: cover` e `aspect-ratio`. Jamais fixe altura de imagem no inline para não causar deformidades.

3.  **Layout System:** Tudo baseia-se em `.container`, `.cards-grid`, e `.section-padding`. Se for criar uma nova "Seção", basta respeitar a semântica: `<section class="nova-sessao section-padding">`.

4.  **Atualização Semântica Frequente:**
    Qualquer alteração visual requerída pelo usuário deve primeiro checar as variáveis da `:root`. No caso do histórico, um erro nas variáveis do background gerou impacto invisível num cabeçalho no passado, corrigido atribuindo estritamente a variável `--color-white: #ffffff`. Mantenha atenção nas cadeias de herança das variáveis CSS.
