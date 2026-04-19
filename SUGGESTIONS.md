# 🚀 Sugestões de Melhoria — Dr. Nelson Tupinambá

Com base na arquitetura atual e nos objetivos de alta conversão e autoridade, seguem as recomendações técnicas e de design.

## 1. Experiência do Usuário (UX) & Design

- **Micro-interações de Feedback:** Adicionar um estado visual de "carregando" ou feedback imediato ao clicar nos botões de WhatsApp para evitar cliques duplos.
- **Dark Mode Toggle:** Embora o tema escuro seja o padrão de autoridade, oferecer um seletor para tema claro pode melhorar a acessibilidade para usuários com certas condições visuais.
- **Skeleton Screens:** Implementar esqueletos de carregamento para a imagem principal (`dr-nelson.png`) e cards para melhorar a percepção de velocidade (LCP).

## 2. Performance & SEO

- **Otimização de Imagens:** Converter `dr-nelson.png` para o formato **WebP** com compressão otimizada. Isso pode reduzir o peso da imagem em até 70% sem perda de qualidade perceptível.
- **Lazy Loading Nativo:** Garantir que todas as imagens abaixo da dobra tenham o atributo `loading="lazy"`.
- **JSON-LD (Structured Data):** Adicionar um script de `schema.org` do tipo `LegalService` no `<head>` para ajudar o Google a entender que se trata de um escritório de advocacia, exibindo informações como endereço e telefone diretamente nos resultados de busca.

## 3. Conversão (CRO)

- **Prova Social Dinâmica:** Adicionar um link direto para as avaliações do Google Meu Negócio ou um widget que puxe as avaliações mais recentes.
- **FAQ com Acordeão:** Implementar uma seção de "Dúvidas Frequentes" para reduzir a fricção antes do contato inicial.
- **Sticky Call-to-Action:** No mobile, manter um botão flutuante discreto de WhatsApp que aparece apenas após o usuário rolar 50% da página.

## 4. Manutenção & Infraestrutura (DevOps)

- **PWA (Progressive Web App):** Adicionar um `manifest.json` básico para permitir que o site seja "instalado" como um aplicativo, melhorando o retorno de clientes recorrentes.
- **CI/CD - Automated Testing:** Adicionar um passo de teste de acessibilidade (Lighthouse CI) no GitHub Actions para garantir que novas atualizações não quebrem o contraste ou a navegação por teclado.

---

_Documento gerado automaticamente como parte do ciclo de melhoria contínua._
