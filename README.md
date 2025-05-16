# 📈 YouTube Trending Video Dashboard

Este projeto foi desenvolvido na ferramenta **Tableau** com o objetivo de automatizar a análise semanal de vídeos em alta no YouTube. Ele atende à equipe de planejamento de anúncios da agência **Sterling & Draper**, oferecendo insights visuais sobre **categorias de vídeos em alta, distribuição por país e tendências específicas por região**.

---

## 🎯 Objetivo do Negócio

Automatizar relatórios de tendências no YouTube para responder rapidamente a perguntas frequentes como:

- Quais categorias de vídeo foram tendências na semana passada?
- Como essas categorias se distribuíram entre os países?
- Quais categorias foram mais populares nos Estados Unidos?

---

## 📊 O Dashboard

O painel foi desenvolvido com foco em **usabilidade diária** e atende diretamente os gerentes de mídia e analistas da empresa.

📌 **Principais elementos do dashboard:**

- Gráfico de áreas empilhadas: Histórico de tendências (valores absolutos e percentuais por categoria)
- Gráfico de pizza: Distribuição de vídeos em alta por país
- Tabela interativa: Categorias por país com destaque (realce) proporcional
- Filtros dinâmicos: por data e país

📷 Layout do dashboard:

![Layout do Dashboard](images/dashboard-layout.png)

---

## 🧱 Fonte de Dados

Os dados são fornecidos por uma tabela agregada no banco de dados `youtube`, atualizada diariamente:

**Tabela: `trending_by_time`**

| Coluna         | Descrição                                        |
|----------------|--------------------------------------------------|
| `record_id`    | Identificador único                              |
| `region`       | País/região geográfica                           |
| `trending_date`| Data de tendência (atualização diária)           |
| `category_title`| Categoria do vídeo                              |
| `videos_count` | Número de vídeos na seção de tendências naquele dia |

---

## 📁 Apresentação

A apresentação final com conclusões e recomendações está disponível no link abaixo:

📎 [Clique aqui para acessar o PDF](presentation/YT_trend_dashboard_presentation.pdf)

---

## 📝 Conclusões

- **Entretenimento e Música** dominam globalmente as tendências.
- **EUA, França e Rússia** são os países com maior volume de vídeos em alta.
- Cada região tem **preferências específicas** (ex: Rússia prefere "People & Blogs", Índia foca em "News & Politics").
- A análise de tendências permite **personalizar campanhas publicitárias** com mais precisão.

---

## 🔧 Ferramentas Utilizadas

![Tableau](https://img.shields.io/badge/-Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Google Slides](https://img.shields.io/badge/-Google%20Slides-FBBB00?style=for-the-badge&logo=google-slides&logoColor=white)

---

## 📌 Observações

- O dashboard é atualizado automaticamente todos os dias à meia-noite (UTC).
- Todos os gráficos possuem a mesma importância visual e analítica.
