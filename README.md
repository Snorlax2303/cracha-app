# Gerador de CrachÃ¡s - Microset

AplicaÃ§Ã£o web para gerar crachÃ¡s corporativos da Microset e etiquetas de bloqueio/perigo prontas para impressÃ£o.

## ðŸš€ CaracterÃ­sticas

- **Logo da Futura** integrado ao design do crachÃ¡
- **Design moderno** com gradientes e efeitos visuais
- **Foto circular** com anel gradiente e sombra realista
- **Campos customizÃ¡veis**: Nome, CPF, Cargo
- **PrÃ©-visualizaÃ§Ã£o em tempo real** (live preview)
- **Pronto para impressÃ£o** em 645Ã—1024px (300 DPI)
- **Totalmente offline** apÃ³s carregar
- **Responsivo** (funciona em mobile)

## ðŸ› ï¸ Stack

- HTML5 Canvas para renderizaÃ§Ã£o do crachÃ¡
- CSS3 com variÃ¡veis (design tokens)
- JavaScript vanilla (sem dependÃªncias)
- Tipografia: Plus Jakarta Sans + JetBrains Mono
- Hospedado no Vercel (serverless)

## ðŸ“¦ InstalaÃ§Ã£o Local

```bash
# Clone o repositÃ³rio
git clone https://github.com/seu-usuario/cracha-app.git
cd cracha-app

# Instale as dependÃªncias (opcional, apenas para dev server)
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

Abra `http://localhost:3000` no navegador.

## ðŸŒ Deploy no Vercel

### OpÃ§Ã£o 1: Vercel CLI (Recomendado)

```bash
# Instale o Vercel CLI
npm i -g vercel

# Dentro da pasta do projeto
vercel

# Siga os prompts para conectar sua conta GitHub e fazer deploy
```

### OpÃ§Ã£o 2: GitHub + Vercel Dashboard

1. **Envie para GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/seu-usuario/cracha-app.git
   git push -u origin main
   ```

2. **Conecte ao Vercel**
   - Acesse [vercel.com](https://vercel.com)
   - Clique em "New Project"
   - Selecione "Import Git Repository"
   - Escolha seu repositÃ³rio
   - Clique em "Deploy"

### OpÃ§Ã£o 3: Drop-in Deploy (Mais Simples)

```bash
# Sem Git, apenas deploy direto
vercel --prod
```

## ðŸ“ Como Usar

1. **Carregue a foto** do colaborador (clique ou arraste)
2. **Preencha o nome** completo
3. **Insira o CPF** ou documento
4. **(Opcional)** Adicione o cargo/funÃ§Ã£o
5. **Clique em "Baixar crachÃ¡"** para exportar como JPG

## ðŸŽ¨ PersonalizaÃ§Ã£o

Para mudar cores, fontes ou layout, edite as variÃ¡veis CSS no `<style>`:

```css
:root {
  --brand: #0F4C75;      /* Cor primÃ¡ria */
  --brand-2: #1E88A8;    /* Cor secundÃ¡ria */
  --accent: #F59E0B;     /* Cor de destaque */
  /* ... */
}
```

## ðŸ“„ Estrutura do Projeto

```
cracha-app/
â”œâ”€â”€ index.html          # AplicaÃ§Ã£o completa (HTML + CSS + JS)
â”œâ”€â”€ package.json        # Metadados do projeto
â”œâ”€â”€ vercel.json         # ConfiguraÃ§Ã£o de deploy
â”œâ”€â”€ .gitignore          # Arquivos a ignorar no Git
â””â”€â”€ README.md           # Este arquivo
```

## ðŸ”’ SeguranÃ§a

- Nenhum dado Ã© enviado para servidores (tudo Ã© processado no navegador)
- Logo embutido em base64 (sem requisiÃ§Ãµes HTTP)
- Sem cookies, sem tracking, sem anÃ¡litica

## ðŸ“± Compatibilidade

- âœ… Chrome/Edge (latest)
- âœ… Firefox (latest)
- âœ… Safari (latest)
- âœ… Mobile browsers

## ðŸ“„ LicenÃ§a

MIT - Use livremente em seus projetos!

## ðŸ‘¥ Autor

**Futura Tecnologia** - Desenvolvido com â¤ï¸

---

**Precisa de ajuda?** Abra uma issue ou entre em contato.

