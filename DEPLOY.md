# 🚀 Guia Completo: Deploy no Vercel

## Pré-requisitos

- [Git](https://git-scm.com/) instalado
- [Node.js](https://nodejs.org/) instalado
- Conta no [GitHub](https://github.com)
- Conta no [Vercel](https://vercel.com) (pode criar gratuitamente)

---

## 📋 Passo 1: Preparar o Repositório Git

### 1.1 Abra o terminal na pasta do projeto

```bash
cd /caminho/para/cracha-app
```

### 1.2 Inicialize um repositório Git

```bash
git init
```

### 1.3 Configure suas credenciais Git

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com"
```

### 1.4 Adicione todos os arquivos

```bash
git add .
```

### 1.5 Crie o primeiro commit

```bash
git commit -m "Initial commit: Gerador de crachás da Futura Tecnologia"
```

---

## 🐙 Passo 2: Criar Repositório no GitHub

### 2.1 Acesse [github.com](https://github.com) e faça login

### 2.2 Clique no ícone **+** no canto superior direito

### 2.3 Selecione **"New repository"**

### 2.4 Preencha os dados:

- **Repository name**: `cracha-app`
- **Description**: Gerador de Crachás Corporativos - Futura Tecnologia
- **Public** ou **Private** (escolha sua preferência)
- Não marque "Initialize this repository"

### 2.5 Clique em **"Create repository"**

---

## 🔗 Passo 3: Enviar Código para GitHub

### 3.1 Na página do repositório, você verá um comando como este:

```bash
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/cracha-app.git
git push -u origin main
```

### 3.2 Copie e execute no terminal (dentro da pasta do projeto):

```bash
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/cracha-app.git
git push -u origin main
```

⚠️ **Substitua `SEU_USUARIO` pelo seu username do GitHub**

### 3.3 Se solicitado, entre com suas credenciais GitHub

---

## ☁️ Passo 4: Deploy no Vercel

### Opção A: Via Vercel Dashboard (Mais Fácil) ⭐

#### 4A.1 Acesse [vercel.com](https://vercel.com) e faça login

#### 4A.2 Clique em **"New Project"**

#### 4A.3 Clique em **"Import Git Repository"**

#### 4A.4 Conecte sua conta GitHub
- Clique em "Connect GitHub Account"
- Autorize o Vercel a acessar seus repositórios

#### 4A.5 Selecione o repositório `cracha-app`

#### 4A.6 Na página de configuração:
- **Project name**: `cracha-app` (ou escolha outro nome)
- **Framework**: "Other" (HTML estático)
- **Root directory**: `.` (raiz do projeto)

#### 4A.7 Clique em **"Deploy"**

✅ Pronto! Seu app estará disponível em um URL tipo:
```
https://cracha-app-xyz123.vercel.app
```

---

### Opção B: Via Vercel CLI

#### 4B.1 Instale o Vercel CLI:

```bash
npm i -g vercel
```

#### 4B.2 No terminal, dentro da pasta do projeto:

```bash
vercel
```

#### 4B.3 Siga as instruções:
- **Set up and deploy "~/cracha-app"?** → Pressione `y` (yes)
- **Which scope do you want to deploy to?** → Selecione sua conta
- **Link to existing project?** → `n` (no, é a primeira vez)
- **What's your project's name?** → `cracha-app` ou outro nome
- **In which directory is your code located?** → Pressione Enter (.)
- **Want to override the settings above?** → `n`

#### 4B.4 Após o deploy:
- Você receberá um URL temporário para preview
- Para ir ao ar (produção):

```bash
vercel --prod
```

✅ Seu app estará no ar!

---

## 🔄 Atualizações Futuras

Depois que o projeto está no Vercel, qualquer push para o GitHub é automaticamente deployado:

```bash
# Faça suas alterações locais
git add .
git commit -m "Descreva as mudanças"
git push

# Vercel automaticamente detecta e faz o deploy
# (você verá na dashboard do Vercel)
```

---

## 🌐 URL Final

Seu gerador de crachás estará disponível em:

```
https://seu-projeto.vercel.app
```

Compartilhe este link com sua equipe!

---

## 🆘 Troubleshooting

### Problema: "Permission denied (publickey)"

**Solução**: Configure SSH para GitHub
```bash
# Gere uma chave SSH
ssh-keygen -t ed25519 -C "seu.email@example.com"

# Adicione ao seu perfil GitHub em Settings > SSH Keys
```

### Problema: Vercel mostra erro 404

**Solução**: Verifique se o arquivo `vercel.json` está configurado corretamente (copie do projeto fornecido)

### Problema: Imagem da logo não aparece

**Solução**: A logo já está embutida em base64 no HTML. Se mesmo assim não aparecer, limpe o cache do navegador (Ctrl+Shift+Delete)

---

## 📞 Suporte

Para dúvidas ou problemas:
1. Verifique os logs no Vercel Dashboard (Deployments tab)
2. Abra uma issue no repositório GitHub
3. Entre em contato com o time de desenvolvimento

---

**Pronto para deploy!** 🎉
