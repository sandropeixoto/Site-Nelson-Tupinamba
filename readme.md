# Landing Page: Dr. Nelson Tupinambá

## Visão Geral

Este é o site oficial do advogado Dr. Nelson Tupinambá, focado na captação e apresentação de serviços de excelência nas áreas de:

- Direito Trabalhista
- Direito Previdenciário
- Licitações e Contratos Públicos

O projeto foi criado visando a melhor experiência do usuário (UX), transmitindo autoridade jurídica por meio de uma identidade visual premium, com altíssima performance estrutural.

## Tecnologias e Padrões Aplicados

- **HTML5 Semântico:** Uma marcação voltada para SEO, limpa, estruturada com base nas sessões lógicas.
- **CSS Vanilla Robusto:**
  - Variáveis Nativas (Design Tokens) gerenciando toda a paleta.
  - Flexbox e CSS Grid para responsividade.
  - Sem uso de frameworks pesados, garantindo que o arquivo `.css` permaneça leve.
- **Javascript Moderno (Sem Libs Mágicas):** Animações suaves em rolagem (Scroll) construídas com a API nativa do `IntersectionObserver` do navegador. Elementos como fade-in no carregamento sem sobrecarregar a Thread principal.

## A Identidade Visual

- **Tonalidades Base:** Um fundo sofisticado e elegante **Deep Navy** (Azul Marinho Profundo, `#0F172A`) em alto contraste com o branco absoluto garantindo leitura total aos textos.
- **Destaque de Ação (Accent):** Tons de dourado premium (`#D4AF37`) utilizado restritamente para os principais Botões (`Call to Action`), divisores e ícones pontuais para trazer refinamento.
- **Tipografia:**
  - **Títulos:** _Playfair Display_ para seriedade e sofisticação.
  - **Textos Base:** _Inter_ garantindo perfeitamente a legibilidade nas descrições longas, tanto nos dispositivos móveis quanto monitores ultra-wide.

## Como Visualizar Localmente

Basta iniciar um servidor estático simples. Utilizando Node (NPM):

```bash
npx serve
```

Ou no VSCode, usando a extensão _Live Server_.

Acesse (usualmente): `http://localhost:3000`

## Próximos Passos

- Adicionar ou adequar, caso necessário, a foto primária (`dr-nelson.png`) na raíz.
- Revisão final de SEO e palavras-chaves (meta tags adicionais).
- Configuração do Google Analytics e Pixel no projeto na etapa de Deploy (ex: Vercel ou Cloudflare Pages).
