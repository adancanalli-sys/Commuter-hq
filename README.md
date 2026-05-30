# 🚲 Commuter HQ — PWA

App para controle de VT, VR e manutenção de bike. Funciona offline e pode ser instalado no celular.

---

## 🚀 Como colocar no ar (Vercel — gratuito, ~5 minutos)

### Passo 1 — Criar conta grátis
1. Acesse [github.com](https://github.com) e crie uma conta (se não tiver)
2. Acesse [vercel.com](https://vercel.com) e entre com a conta do GitHub

### Passo 2 — Subir o código
1. No GitHub, clique em **"New repository"**
2. Dê o nome `commuter-hq` e clique em **"Create repository"**
3. No seu computador, abra o terminal na pasta do projeto e rode:
```bash
git init
git add .
git commit -m "primeiro commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/commuter-hq.git
git push -u origin main
```

### Passo 3 — Deploy na Vercel
1. No [vercel.com](https://vercel.com), clique em **"Add New Project"**
2. Selecione o repositório `commuter-hq`
3. Deixe tudo como está e clique em **"Deploy"**
4. Aguarde ~1 minuto — pronto! Você receberá uma URL tipo `commuter-hq.vercel.app`

### Passo 4 — Instalar no celular como app
**Android (Chrome):**
1. Abra a URL no Chrome
2. Toque nos 3 pontinhos → "Adicionar à tela inicial"
3. Confirme — vira um ícone na tela!

**iPhone (Safari):**
1. Abra a URL no Safari
2. Toque no ícone de compartilhar (quadrado com seta)
3. "Adicionar à Tela de Início"

---

## 🔔 Notificações
- Vá em ⚙️ Config no app
- Ative o lembrete diário e escolha o horário
- Permita as notificações quando o navegador perguntar
- Clique "Testar notificação" para confirmar que está funcionando

---

## 📁 Estrutura do projeto
```
commuter-pwa/
├── index.html          # Entrada HTML
├── package.json        # Dependências
├── vite.config.js      # Configuração do bundler
├── public/
│   ├── manifest.json   # Config do PWA
│   └── sw.js           # Service Worker (offline + notificações)
└── src/
    ├── main.jsx        # Entry point React
    └── App.jsx         # App completo
```

## 🛠️ Rodar localmente
```bash
npm install
npm run dev
```
Abra http://localhost:5173

## 🏗️ Gerar build de produção
```bash
npm run build
```
