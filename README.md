# TKMaster — Site Institucional

> Presença digital da **TKMaster Consultoria e Sistemas** — conectando empresas a profissionais de TI qualificados, com gestão ativa e acompanhamento real.

---

## 📄 Páginas — PT (raiz)

| Arquivo | Descrição |
|---|---|
| `index.html` | Homepage — serviços, como funciona, diferenciais e CTA |
| `talentos.html` | Banco de talentos — cadastro para profissionais PJ |
| `parceiros.html` | Página de parceria — Parceiro Comercial e Parceiro TA |
| `contato.html` | Contato para empresas e profissionais |
| `vmv.html` | Visão, Missão e Valores |
| `privacidade.html` | Política de Privacidade (LGPD) |
| `termos.html` | Termos de Uso do site |
| `404.html` | Página de erro personalizada |

## 📄 Páginas — EN (`/en/`)

| Arquivo | Descrição |
|---|---|
| `en/index.html` | Homepage — English version |
| `en/talents.html` | Talent pool — registration for PJ professionals |
| `en/partner.html` | Partner page — Commercial Partner and TA Partner |
| `en/contact.html` | Contact for companies and professionals |
| `en/vmv.html` | Vision, Mission & Values |
| `en/privacy.html` | Privacy Policy (LGPD) |
| `en/terms.html` | Terms of Use |
| `en/404.html` | Custom error page |

---

## 🗂 Arquivos de suporte

| Arquivo | Descrição |
|---|---|
| `sitemap.xml` | Mapa do site para indexação pelo Google |
| `robots.txt` | Instruções para robôs de busca |
| `og-image.jpg` | Imagem de prévia para WhatsApp, LinkedIn e Facebook (1200×630px) |
| `netlify.toml` | Configuração de deploy e redirecionamento 404 no Netlify |

> **Botão WhatsApp flutuante** — embutido diretamente nas páginas antes do `</body>`. Número configurado: `+55 21 98993-4272`. Para alterar, busque `wa.me/5521989934272` nos arquivos HTML e substitua pelo novo número.

> **Cookie banner** — embutido diretamente nas páginas antes do `</body>`. Nas páginas EN o texto já está em inglês e aponta para `en/privacy.html`.

---

## 🌐 Estrutura bilíngue PT/EN

O site é bilíngue com seletor `PT · EN` no nav de todas as páginas.

- Páginas **PT** ficam na raiz `/`
- Páginas **EN** ficam na pasta `/en/` com nomes em inglês
- O botão **PT** nas páginas EN aponta para `../nomepagina.html`
- O botão **EN** nas páginas PT aponta para `en/nomepagina.html`
- Links internos das páginas EN são relativos (sem prefixo `en/`)
- Links das páginas EN para PT usam `../` como prefixo

---

## 🛠 Tecnologias

- **HTML5** — estrutura semântica
- **CSS3** — design system próprio com variáveis, animações e responsividade
- **JavaScript** — interações leves (menu mobile, cookie banner, dropdown, lang switcher)
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

> **Regra de cor de seções:** a última seção antes do rodapé nunca pode ser navy (`#0B1D3A`), pois o rodapé também é navy. Usar vermelho (`#C0151A`) como fundo nas seções CTA finais.

> **Alternância de seções em `parceiros.html` / `partner.html`:** Comercial (branco) → TA (navy) → Como Funciona (branco) → Modelo (navy) → FAQ (branco) → CTA (vermelho).

---

## ⚙️ Configuração no servidor

**Página 404 personalizada**

O `netlify.toml` já configura o redirecionamento automaticamente:
```toml
[[redirects]]
  from   = "/*"
  to     = "/404.html"
  status = 404
```

Para Apache (`.htaccess`):
```apache
ErrorDocument 404 /404.html
```

Para Nginx:
```nginx
error_page 404 /404.html;
```

**Sitemap no Google Search Console**

Após publicar, cadastre o sitemap em:
`https://search.console.google.com` → Sitemaps → `https://www.tkmasters.com.br/sitemap.xml`

---

## 📁 Estrutura de arquivos

```
/
├── index.html
├── talentos.html
├── parceiros.html          ← novo
├── contato.html
├── vmv.html
├── privacidade.html
├── termos.html
├── 404.html
├── sitemap.xml
├── robots.txt
├── netlify.toml
├── og-image.jpg
├── favicons/
│   └── favicon-16x16.png
└── en/
    ├── index.html
    ├── talents.html
    ├── partner.html        ← novo
    ├── contact.html
    ├── vmv.html
    ├── privacy.html
    ├── terms.html
    └── 404.html
```

---

## 🔗 Âncoras de navegação

### PT — `index.html`
| ID | Seção |
|---|---|
| `#como-funciona` | Como funciona para empresas |
| `#servicos` | Serviços |
| `#alocacao` | Alocação de TI |
| `#gestao-contratos` | Gestão de Contratos |
| `#gerencia-contas` | Gerência de Contas |
| `#desenvolvimento` | Desenvolvimento de Sistemas |
| `#stacks` | Tecnologias |
| `#sobre` | Por que TKMaster |
| `#profissionais` | Para Profissionais |

### EN — `en/index.html`
| ID | Section |
|---|---|
| `#how-it-works` | How it works for companies |
| `#services` | Services |
| `#staffing` | IT Staffing |
| `#contracts` | Contract Management |
| `#account-management` | Account Management |
| `#development` | Systems Development |
| `#stacks` | Technologies |
| `#about` | Why TKMaster |
| `#professionals` | For Professionals |

### PT/EN — `vmv.html` / `en/vmv.html`
| PT ID | EN ID | Seção |
|---|---|---|
| `#pilares` | `#pillars` | Visão, Missão e Posicionamento |
| `#valores` | `#values` | Valores |
| `#proposito` | `#origin` | Origem / citação da fundadora |

### PT/EN — `talentos.html` / `en/talents.html`
| PT ID | EN ID | Seção |
|---|---|---|
| `#como-funciona` | `#how-it-works` | Processo de cadastro |
| `#garantias` | `#guarantees` | Garantias |
| `#stacks` | `#stacks` | Stacks com demanda ativa |
| `#cadastro` | `#register` | CTA de cadastro |

### PT/EN — `parceiros.html` / `en/partner.html`
| PT ID | EN ID | Seção |
|---|---|---|
| `#comercial` | `#commercial` | Parceiro Comercial |
| `#talent-acquisition` | `#talent-acquisition` | Parceiro TA |
| `#como-funciona` | `#how-it-works` | Como funciona |
| `#modelo` | `#model` | Modelo de parceria |
| `#faq` | `#faq` | Perguntas frequentes |
| `#inscrever` | `#sign-up` | CTA final |

---

## 🧩 Componentes globais

### Menu Institucional (dropdown)
Presente no nav de todas as páginas. Abre ao hover ou clique, fecha com delay de 200ms para permitir movimento do mouse. Itens: Por que TKMaster · Visão, Missão e Valores · Seja Parceiro · Fale Conosco.

### Rodapé — 5 colunas
Todas as páginas têm o rodapé com `grid-template-columns: 2fr 1fr 1fr 1fr 1fr`:

| Coluna | Conteúdo |
|---|---|
| 1 | Logo + descrição + redes sociais |
| 2 | Empresa |
| 3 | Para Empresas |
| 4 | Para Profissionais |
| 5 | Parceiros ← novo |

> Para adicionar a coluna Parceiros em páginas existentes: (1) alterar o CSS de `2fr 1fr 1fr 1fr` para `2fr 1fr 1fr 1fr 1fr`; (2) colar o bloco `<div>Parceiros...</div>` após o bloco "Para Profissionais" dentro de `.footer-grid`.

### WhatsApp FAB
Botão flutuante verde fixo no canto inferior direito. Embutido antes de `</body>` em todas as páginas. Sobe automaticamente quando o cookie banner está visível.

### Cookie banner
Banner LGPD fixo no rodapé com animação de slide-up. Armazena consentimento no `localStorage` por 365 dias. Texto em PT nas páginas PT, em inglês nas páginas EN.

---

## 📋 Status

| Item | Status |
|---|---|
| Páginas principais PT | ✅ Concluído |
| Páginas EN (`/en/`) | ✅ Concluído |
| Página de Parceiros PT (`parceiros.html`) | ✅ Concluído |
| Página de Parceiros EN (`en/partner.html`) | ✅ Concluído |
| Seletor PT · EN no nav | ✅ Concluído |
| Menu Institucional (dropdown) | ✅ Concluído |
| Rodapé 5 colunas com coluna Parceiros | ✅ Concluído |
| Design responsivo | ✅ Concluído |
| Meta tags + OG tags (PT e EN) | ✅ Concluído |
| Twitter Card + hreflang (PT e EN) | ✅ Concluído |
| Cookie banner (LGPD) PT e EN | ✅ Concluído |
| Botão WhatsApp flutuante | ✅ Concluído |
| Política de Privacidade | ✅ Concluído |
| Termos de Uso | ✅ Concluído |
| Página 404 personalizada PT e EN | ✅ Concluído |
| SEO (sitemap + robots.txt) | ✅ Concluído |
| Âncoras individuais por serviço | ✅ Concluído |
| Sitemap atualizado com URLs de parceiros | 🔲 Pendente |
| Coluna Parceiros no footer das demais páginas | 🔲 Pendente |
| Domínio e hospedagem | 🔲 Pendente |
| Google Search Console | 🔲 Pendente |

---

## 🏢 Sobre a TKMaster

**TKMaster Consultoria e Sistemas** — Rio de Janeiro, RJ, Brasil
Outsourcing de TI com Gerente de Contas dedicado e gestão ativa durante todo o projeto.

🌐 [tkmaster-web.netlify.app](https://tkmaster-web.netlify.app)
💼 [LinkedIn](https://www.linkedin.com/company/tkmasterconsultorias/)
📺 [YouTube](https://www.youtube.com/@TKMasterConsultorias)
📸 [Instagram](https://www.instagram.com/tkmaster.consultoria)