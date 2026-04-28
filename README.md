# TKMaster — Site Institucional

> Presença digital da **TKMaster Consultoria e Sistemas** — conectando empresas a profissionais de TI qualificados, com gestão ativa e acompanhamento real.

---

## 📄 Páginas

| Arquivo | Descrição |
|---|---|
| `index.html` | Homepage — serviços, como funciona, diferenciais e CTA |
| `tkmaster_talentos.html` | Banco de talentos — cadastro para profissionais PJ |
| `tkmaster_contato.html` | Formulário de contato para empresas e profissionais |
| `tkmaster_vmv.html` | Visão, Missão e Valores |
| `tkmaster_privacidade.html` | Política de Privacidade (LGPD) |
| `tkmaster_404.html` | Página de erro personalizada |

---

## 🗂 Arquivos de suporte

| Arquivo | Descrição |
|---|---|
| `sitemap.xml` | Mapa do site para indexação pelo Google |
| `robots.txt` | Instruções para robôs de busca |
| `og-image.jpg` | Imagem de prévia para WhatsApp, LinkedIn e Facebook (1200×630px) |
| `cookie-banner.html` | Snippet do banner de cookies — já embutido nas páginas |

---

## 🛠 Tecnologias

- **HTML5** — estrutura semântica
- **CSS3** — design system próprio com variáveis, animações e responsividade
- **JavaScript** — interações leves (menu mobile, cookie banner, dropdown)
- **Google Fonts** — Barlow + Barlow Condensed
- Sem frameworks, sem dependências externas

---

## 🎨 Design System

| Token | Valor |
|---|---|
| Navy (primária) | `#0B1D3A` |
| Red (destaque) | `#C0151A` |
| Gray | `#9A9A94` |
| Font display | `Barlow Condensed` |
| Font body | `Barlow` |

---

## ⚙️ Configuração no servidor

**Página 404 personalizada**

Apache (`.htaccess`):
```apache
ErrorDocument 404 /tkmaster_404.html
```

Nginx:
```nginx
error_page 404 /tkmaster_404.html;
```

**Sitemap no Google Search Console**

Após publicar, cadastre o sitemap em:
`https://search.console.google.com` → Sitemaps → `https://www.tkmasters.com.br/sitemap.xml`

---

## 📁 Estrutura de arquivos

```
/
├── index.html
├── tkmaster_talentos.html
├── tkmaster_contato.html
├── tkmaster_vmv.html
├── tkmaster_privacidade.html
├── tkmaster_404.html
├── sitemap.xml
├── robots.txt
├── og-image.jpg
└── favicons/
    └── favicon-16x16.png
```

---

## 📋 Status

| Item | Status |
|---|---|
| Páginas principais | ✅ Concluído |
| Design responsivo | ✅ Concluído |
| Meta tags + OG tags | ✅ Concluído |
| Cookie banner (LGPD) | ✅ Concluído |
| Política de Privacidade | ✅ Concluído |
| Página 404 personalizada | ✅ Concluído |
| SEO (sitemap + robots.txt) | ✅ Concluído |
| Domínio e hospedagem | 🔲 Pendente |
| Google Search Console | 🔲 Pendente |

---

## 🏢 Sobre a TKMaster

**TKMaster Consultoria e Sistemas** — Rio de Janeiro, RJ, Brasil  
Outsourcing de TI com Gerente de Contas dedicado e gestão ativa durante todo o projeto.

🌐 [www.tkmasters.com.br](https://www.tkmasters.com.br)  
💼 [LinkedIn](https://www.linkedin.com/company/tkmasterconsultorias/)  
📺 [YouTube](https://www.youtube.com/@TKMasterConsultorias)  
📸 [Instagram](https://www.instagram.com/tkmaster.consultoria)
