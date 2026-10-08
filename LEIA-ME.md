# Site MARONFIT — guia rápido de edição

## Ver o site no computador
Na pasta `maronfit-site`, rode:

```
python -m http.server 8000
```

Depois abra http://localhost:8000 no navegador.

## O que editar e onde

| O quê | Onde |
|---|---|
| **Vídeos das seções** | `assets/video/*.mp4` + imagem de capa `*.webp` com o mesmo nome. Para trocar, substitua mantendo o nome do arquivo |
| **Foto do Hugo (redes/Google)** | `assets/img/hugo.jpg` e `assets/img/og-maronfit.jpg` |
| **Número do CRN** | `js/config.js` → `crn: "CRN-9 12345"` |
| **Mensagem automática do WhatsApp** | `js/config.js` → `mensagemWhatsapp` |
| **Depoimentos** (somente reais e autorizados) | `js/config.js` → lista `depoimentos` |
| **Programas/produtos para venda** | `js/config.js` → lista `programas` (a seção aparece sozinha) |
| **Textos das seções** | `index.html` (cada seção está marcada com um comentário `====`) |
| **Resposta "Como funcionam os atendimentos"** | `index.html`, no FAQ (procure por `EDITAR`) |
| **Cores e fontes** | `css/style.css`, no bloco `:root` no topo |
| **Domínio do site (SEO)** | `index.html` → `<link rel="canonical">` |
| **Política de Privacidade / Termos** | `politica-de-privacidade.html` e `termos-de-uso.html` (modelos para revisão jurídica) |

Procure por `EDITAR` nos arquivos para encontrar todos os pontos pendentes.

## Publicação
É um site estático (HTML/CSS/JS): basta enviar a pasta inteira para qualquer hospedagem,
como Netlify, Vercel, GitHub Pages ou Hostinger.
