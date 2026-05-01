# Princesas de Crochê — Landing Page

Site de vendas estático, pronto para deploy na Vercel via GitHub.

## Estrutura

```
/
├── index.html      ← página completa
├── vercel.json     ← configuração da Vercel
├── .gitignore
└── README.md
```

## Como subir no GitHub + Vercel

### 1. Criar repositório no GitHub
1. Acesse [github.com](https://github.com) e clique em **New repository**
2. Dê um nome (ex: `princesas-croche`)
3. Deixe **Public** ou **Private** (os dois funcionam na Vercel)
4. Clique em **Create repository**

### 2. Enviar os arquivos
No terminal, dentro da pasta do projeto:
```bash
git init
git add .
git commit -m "primeiro deploy"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/princesas-croche.git
git push -u origin main
```

### 3. Conectar na Vercel
1. Acesse [vercel.com](https://vercel.com) e faça login com o GitHub
2. Clique em **Add New → Project**
3. Selecione o repositório `princesas-croche`
4. Nas configurações, deixe tudo padrão (Framework: **Other**)
5. Clique em **Deploy**

✅ Pronto! A Vercel gera um link público automaticamente.

### 4. Atualizações futuras
Cada `git push` para a branch `main` faz deploy automático na Vercel.
```bash
git add .
git commit -m "ajuste na página"
git push
```
