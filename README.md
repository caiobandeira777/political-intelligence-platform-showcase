# Mandato365 — Political Intelligence Platform

> **Plataforma SaaS de inteligência política em produção, construída do zero por um desenvolvedor solo.**
> Transforma dados públicos (eleitorais, parlamentares, demográficos e digitais) em decisões estratégicas — com IA, em minutos.

🌐 **Live, teste real com deputado real:** https://www.mandato365.com.br](https://youtu.be/IVAE4H_5Yfo
🏛️ **Status:** Em produção, com gabinete parlamentar e partido político usando ativamente.

> ⚠️ **Sobre este repositório:** este é um **showcase público**. O código-fonte é **proprietário e privado**, por se tratar de um produto comercial em operação, com clientes reais e pipelines de dados próprios. Aqui você encontra a visão geral do produto, as funcionalidades, a arquitetura e a stack — tudo que importa pra entender o que foi construído, sem expor a implementação. Para uma demonstração técnica ao vivo ou conversa sobre o código, entre em contato.

---

## 🎯 O problema

Gabinetes parlamentares e campanhas se afogam em dados espalhados por dezenas de fontes — TSE, Câmara dos Deputados, Portal da Transparência, IBGE, redes sociais — e não têm tempo nem ferramenta para transformar isso em decisão. O Mandato365 faz essa ponte: **do dado bruto à estratégia, automaticamente.**

---

## ⚙️ Funcionalidades

### 📰 Clipping de notícias com IA
Monitora automaticamente tudo que sai na mídia sobre o parlamentar e o partido. Cada notícia é classificada por **sentimento (positivo / negativo / neutro)** e recebe um **resumo gerado por IA**.
**Por que importa:** o que exigia horas de leitura manual por dia agora chega pronto, com o termômetro da imagem pública em tempo real.
<img width="1488" height="1057" alt="8d2d6db3-e22f-4098-958b-4182313999a9" src="https://github.com/user-attachments/assets/183f51fc-810c-4f73-a3ea-2cd564abb053" />

### 📊 Analytics de redes sociais (Instagram, TikTok e Twitter/X)
Acompanha a performance dos posts, monitora adversários e identifica conteúdo viral em múltiplas plataformas.
**Por que importa:** a eleição também se ganha no digital — e o que se mede, se melhora.
<img width="1448" height="1086" alt="2640adab-3c13-4be2-82aa-8f6ac6f42c70" src="https://github.com/user-attachments/assets/acd154bf-e4d0-460e-a2fc-197d134ab210" />
<img width="1448" height="1086" alt="50ee5b15-f53b-4d53-a673-403e0d528926" src="https://github.com/user-attachments/assets/afe757bd-af4e-4020-b3cc-2c05ac00d77f" />
<img width="1448" height="1086" alt="73de4f6e-ce22-46c0-a7c4-eb4c905088c4" src="https://github.com/user-attachments/assets/bb36a87e-7ea5-4572-9d1a-1044113f5f7f" />
<img width="1448" height="1086" alt="f11a586e-c09f-407a-a480-7872b2ed458c" src="https://github.com/user-attachments/a<img width="1448" height="1086" alt="4fb4cd81-aa93-4db9-ab3f-a54743aa79bb" src="https://github.com/user-attachments/assets/9675944a-b978-42db-bc1a-cc1f565efb03" />
ssets/d0bf703a-0fb7-41bd-b593-33861a1f4343" />
![Uploading 4fb4cd81-aa93-4db9-ab3f-a54743aa79bb.png…]()

### 🧠 Análise de sentimento de posts
IA que lê o engajamento e revela como o público está reagindo ao conteúdo publicado.
**Por que importa:** separa o conteúdo que viralizou bem do que viralizou mal.
<img width="1448" height="1086" alt="e3b5765a-c6a2-4842-b0f5-d22a811c323d" src="https://github.com/user-attachments/assets/45cf20fc-e425-46e5-b5c9-d121e7818876" />

### 🗺️ Mapas eleitorais inteligentes
Cruzamento territorial de **votos, verbas, demografia, ROI eleitoral e ideologia** por município.
**Por que importa:** responde a pergunta de ouro de toda campanha — *"onde está meu voto, onde a verba virou voto, e onde vale a pena investir?"*
<img width="2690" height="584" alt="56710d2a-bf5e-49ab-8e6a-dca969fdc29b" src="https://github.com/user-attachments/assets/9e7acf9b-2c77-47c6-970b-7e31cc160870" />
<img width="1672" height="941" alt="57839e05-ad7c-4334-adb0-2d35d79f7dfa" src="https://github.com/user-attachments/assets/fb0f0fe8-0e9d-49ac-bf3f-2cff426ea30f" />
<img width="1448" height="1086" alt="de2f54fd-e03f-4f9a-894b-405695a89a47" src="https://github.com/user-attachments/assets/1f485643-8e73-426a-b6ff-11cc5f76a891" />


### 💰 Dashboard financeiro do gabinete
Acompanha emendas e verbas parlamentares, cruzando com retorno eleitoral.
**Por que importa:** mostra onde o recurso público está virando resultado e onde está sendo desperdiçado.
<img width="1452" height="1083" alt="8691fd10-0fab-41ad-aad9-bb56c55ffe65" src="https://github.com/user-attachments/assets/9c3c3c1d-5eb8-4b4a-8a4d-235da50b7a14" />

### ✍️ Criador de discursos parlamentares
Gera discursos com IA fundamentados em **dados reais do IBGE**.
**Por que importa:** discurso embasado em dado concreto da região, pronto em minutos.
<img width="1672" height="941" alt="b6106095-2bd9-4b9c-8c9b-4adeda2aa46e" src="https://github.com/user-attachments/assets/6f995d30-2f1f-4cd9-ba82-e170536278a0" />


### 💬 Assistente WhatsApp
Alertas estratégicos, score de reeleição e dados do mandato em tempo real, direto no celular.
**Por que importa:** a informação chega onde o político realmente está.

---

## 🏗️ Arquitetura (visão geral)

```
┌─────────────────────────────────────────────────────────────┐
│                     FONTES DE DADOS                          │
│   TSE  ·  Câmara dos Deputados  ·  Portal da Transparência   │
│   IBGE  ·  Google News  ·  Instagram / TikTok / Twitter      │
└─────────────────────────────┬───────────────────────────────┘
                              │  (pipelines de ingestão)
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              CAMADA DE PROCESSAMENTO + IA                     │
│   Normalização · Cruzamento de dados · Análise de IA (LLM)   │
│   Sentimento · Sumarização · Geração de conteúdo             │
└─────────────────────────────┬───────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    APLICAÇÃO (Next.js)                       │
│   Dashboards · Mapas · Relatórios · API · Assistente WhatsApp│
└─────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Stack técnica

| Camada | Tecnologias |
|---|---|
| **Frontend** | Next.js 14, TypeScript, Tailwind CSS, Recharts |
| **Backend** | Next.js API Routes, Node.js |
| **Banco de dados** | PostgreSQL |
| **IA / LLM** | Anthropic Claude (análise de sentimento, sumarização, geração de conteúdo) |
| **Dados** | TSE, Câmara dos Deputados, Portal da Transparência (CEAP), IBGE, redes sociais |
| **Infra / Deploy** | Vercel (produção) |

---

## 👤 Sobre o desenvolvimento

Projeto **construído do zero por um único desenvolvedor**, de ponta a ponta:
- Arquitetura e modelagem de dados
- Desenvolvimento full-stack
- Integração de IA para análise automatizada e geração de conteúdo
- Pipelines de ingestão e cruzamento de dados públicos
- Deploy e operação em produção

Não é um protótipo de portfólio — é um produto **rodando, com clientes reais.**

---

## 📬 Contato

Interessado em uma demonstração ao vivo, parceria ou oportunidade?

- 🌐 [mandato365.com.br](https://www.mandato365.com.br)
- 💼 [LinkedIn](https://www.linkedin.com/in/SEU-PERFIL)  <!-- troque pelo seu link -->
- 📧 seu@email.com  <!-- troque pelo seu email -->

---

<sub>© 2026 Mandato365 · Inteligência política baseada em dados · Código proprietário.</sub>
