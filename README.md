# 🎨 GAG Visual — Gestão

**Uma PWA (Progressive Web App) para gerir contactos, orçamentos, facturas e recibos.**

![GAG Visual](https://img.shields.io/badge/GAG%20Visual-Gestão-C9A24B?style=flat-square)
![PWA](https://img.shields.io/badge/PWA-Progressive%20Web%20App-5A5A5A?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## 📱 Funcionalidades

✅ **Contactos** — Guarda nomes, negócios e números de WhatsApp  
✅ **Orçamentos** — Cria orçamentos com cálculo automático de preços  
✅ **Facturas & Recibos** — Gera documentos profissionais em texto  
✅ **Mensagens Prontas** — 6 templates de mensagens para WhatsApp  
✅ **Armazenamento Local** — Dados guardados no telemóvel (sem cloud)  
✅ **Offline** — Funciona sem internet (cache automático)  
✅ **Instalável** — Adiciona ao ecrã inicial como app nativa  

---

## 🚀 Começar

### Opção 1: Usar Online (GitHub Pages)

1. Vai a: https://kaz232.github.io/gag-visual-app/
2. Clica em **"Instalar app no telemóvel"** ou usa o menu do navegador
3. Pronto! Tens a app no teu telemóvel

### Opção 2: Usar Localmente

```bash
git clone https://github.com/Kaz232/gag-visual-app.git
cd gag-visual-app
```

Depois, abre o arquivo `index.html` no navegador ou usa um servidor local:

```bash
python -m http.server 8000
# Depois acede a: http://localhost:8000
```

---

## 📋 Como Usar

### 1️⃣ Adicionar Contactos

- Vai a **"Contactos"**
- Clica em **"+"**
- Preenche: Nome, Negócio, Contacto (WhatsApp), Estado (Lead/Cliente)
- Guardar

### 2️⃣ Criar Orçamento

- Vai a **"Orçamento"**
- Escolhe: Cliente, Serviço, Quantidade, Prazo, Complexidade
- O preço calcula automaticamente
- Confirma e guarda

### 3️⃣ Gerar Factura/Recibo

- Vai a **"Histórico"**
- Clica no orçamento
- Escolhe entre **"Factura"** ou **"Recibo"**
- Copia o texto ou envia direto no WhatsApp

### 4️⃣ Enviar Mensagens

- Vai a **"Mensagens"**
- Escolhe a mensagem pronta
- Copia ou abre no WhatsApp
- A app substitui automaticamente `[Nome]` pelo nome do contacto

---

## 🎨 Design

- **Cores**: Paleta terra (Ochre #C9A24B, Terra escura #2B2118, Areia #EDE3D0)
- **Tipografia**: Fraunces (títulos) + Work Sans (corpo)
- **Responsive**: Optimizado para mobile (portrait)
- **Acessibilidade**: Contraste adequado, navegação clara

---

## 🛠 Estrutura do Projeto

```
gag-visual-app/
├── index.html              # App principal (HTML + CSS + JS inline)
├── service-worker.js       # Cache offline
├── manifest.json           # PWA metadata
├── icons/
│   ├── icon-192.png       # Ícone 192x192 (app launcher)
│   └── icon-512.png       # Ícone 512x512 (splash screen)
└── README.md              # Este arquivo
```

---

## 💾 Dados

- ✅ Todos os dados são guardados **localmente** no telemóvel (localStorage)
- ✅ Nenhum dado é enviado para servidores externos
- ✅ Para backup: copia manualmente os dados do navegador
- ⚠️ Se limpares o cache do navegador, os dados apagam

---

## 📊 Tabela de Preços

| Serviço | Preço Base |
|---------|------------|
| Flyer Comercial | Kz 2.500 |
| Logótipo Profissional | Kz 5.000 |
| Convite Digital | Kz 2.000 |
| CV Profissional | Kz 2.000 |
| Vídeo Curto Institucional | Kz 3.000 |
| Gestão Redes Sociais (mês) | Kz 15.000 |

**Multiplicadores:**
- Prazo: Flexível (0.9x) | Normal (1.0x) | Urgente (1.5x)
- Complexidade: Simples (1.0x) | Média (1.3x) | Complexa (1.6x)

---

## 🐛 Resolução de Problemas

### "A app não funciona offline"
- Certifica-te que registou o service worker (abre a app uma vez online)
- Limpa o cache: Abrir DevTools → Application → Clear site data

### "Os dados desapareceram"
- LocalStorage foi apagado (limpar cache do navegador)
- Sem backup automático — guarda as informações importantes noutro local

### "Não consigo instalar a app"
- Tenta usar HTTPS (GitHub Pages usa HTTPS automaticamente)
- Se usar localmente, cria um certificado SSL ou usa o servidor de teste

---

## 📱 Compatibilidade

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome/Edge | ✅ | ✅ |
| Firefox | ✅ | ✅ |
| Safari | ✅ | ⚠️ (instalação limitada) |
| Samsung Internet | — | ✅ |

---

## 📜 Licença

MIT — Usa livremente para fins comerciais e pessoais.

---

## 🤝 Contribuições

Sugestões ou melhorias? Abre uma issue ou um pull request!

---

## 📧 Contacto

**GAG Visual**  
Email: josemargourgel01@gmail.com  
WhatsApp: [Inserir número]

---

**Desenvolvido com ❤️ em Luanda, Angola**