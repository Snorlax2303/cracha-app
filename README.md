# Gerador de Crachás - Futura Tecnologia

Aplicação web para gerar crachás corporativos profissionais em alta resolução (300 DPI).

## 🚀 Características

- **Logo da Futura** integrado ao design do crachá
- **Design moderno** com gradientes e efeitos visuais
- **Foto circular** com anel gradiente e sombra realista
- **Campos customizáveis**: Nome, CPF, Cargo
- **Pré-visualização em tempo real** (live preview)
- **Pronto para impressão** em 645×1024px (300 DPI)
- **Totalmente offline** após carregar
- **Responsivo** (funciona em mobile)

## 🛠️ Stack

- HTML5 Canvas para renderização do crachá
- CSS3 com variáveis (design tokens)
- JavaScript vanilla (sem dependências)
- Tipografia: Plus Jakarta Sans + JetBrains Mono
- Hospedado no Vercel (serverless)

## 📦 Instalação Local

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/cracha-app.git
cd cracha-app

# Instale as dependências (opcional, apenas para dev server)
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

Abra `http://localhost:3000` no navegador.

## 🌐 Deploy no Vercel

### Opção 1: Vercel CLI (Recomendado)

```bash
# Instale o Vercel CLI
npm i -g vercel

# Dentro da pasta do projeto
vercel

# Siga os prompts para conectar sua conta GitHub e fazer deploy
```

### Opção 2: GitHub + Vercel Dashboard

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
   - Escolha seu repositório
   - Clique em "Deploy"

### Opção 3: Drop-in Deploy (Mais Simples)

```bash
# Sem Git, apenas deploy direto
vercel --prod
```

## 📝 Como Usar

1. **Carregue a foto** do colaborador (clique ou arraste)
2. **Preencha o nome** completo
3. **Insira o CPF** ou documento
4. **(Opcional)** Adicione o cargo/função
5. **Clique em "Baixar crachá"** para exportar como JPG

## 🎨 Personalização

Para mudar cores, fontes ou layout, edite as variáveis CSS no `<style>`:

```css
:root {
  --brand: #0F4C75;      /* Cor primária */
  --brand-2: #1E88A8;    /* Cor secundária */
  --accent: #F59E0B;     /* Cor de destaque */
  /* ... */
}
```

## 📄 Estrutura do Projeto

```
cracha-app/
├── index.html          # Aplicação completa (HTML + CSS + JS)
├── package.json        # Metadados do projeto
├── vercel.json         # Configuração de deploy
├── .gitignore          # Arquivos a ignorar no Git
└── README.md           # Este arquivo
```

## 🔒 Segurança

- Nenhum dado é enviado para servidores (tudo é processado no navegador)
- Logo embutido em base64 (sem requisições HTTP)
- Sem cookies, sem tracking, sem análitica

## 📱 Compatibilidade

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## 📄 Licença

MIT - Use livremente em seus projetos!

## 👥 Autor

**Futura Tecnologia** - Desenvolvido com ❤️

---

**Precisa de ajuda?** Abra uma issue ou entre em contato.
