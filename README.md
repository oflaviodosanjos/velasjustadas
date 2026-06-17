# Método Velas Ajustadas™ — Landing Page

Landing page de vendas do programa de mentoria estratégica individual **Método Velas Ajustadas™**.

---

## 🚀 Deploy no GitHub Pages

### Passo a passo

1. **Crie um repositório** no GitHub (ex: `velas-ajustadas` ou `seu-usuario.github.io`)
2. **Faça upload** do arquivo `index.html` para a raiz do repositório
3. Vá em **Settings → Pages**
4. Em **Source**, selecione `Deploy from a branch`
5. Escolha a branch `main` e a pasta `/ (root)`
6. Clique em **Save**
7. Em alguns minutos seu site estará disponível em:
   `https://seu-usuario.github.io/velas-ajustadas/`

---

## ✏️ Personalização obrigatória antes de publicar

Abra o `index.html` e substitua os seguintes itens:

| O que alterar | Onde encontrar no arquivo | Exemplo |
|---|---|---|
| Link do checkout | `href="#"` nos botões de CTA | `href="https://pay.hotmart.com/..."` |
| Número de WhatsApp | `wa.me/55XXXXXXXXXX` | `wa.me/5511999999999` |
| Público-alvo | `EMPREENDEDORES` no eyebrow do hero | `FISIOTERAPEUTAS` |
| Vídeo de depoimento | Seção `#depoimentos` | Substituir placeholder por `<iframe>` do YouTube/Vimeo |
| Timer de deadline | Chave `va_dl4` no JS | O timer já persiste em `localStorage` automaticamente |

---

## 📁 Estrutura do projeto

```
index.html      ← Landing page completa (autocontida, sem dependências locais)
README.md       ← Este arquivo
.gitignore      ← Arquivos a ignorar
```

O arquivo `index.html` é **100% autocontido**:
- Fontes carregadas via Google Fonts (CDN)
- Sem dependências de bibliotecas externas
- Sem arquivos CSS ou JS separados
- Funciona offline após o primeiro carregamento

---

## 🎨 Design

| Elemento | Valor |
|---|---|
| Tipografia — Títulos | Playfair Display (700/800/900) |
| Tipografia — Interface | Space Grotesk (400/500/600/700) |
| Tipografia — Corpo | Plus Jakarta Sans (400/500/600) |
| Cor primária | `#1E1410` (Brown deep) |
| Cor de acento | `#A8822A` / `#C9A042` (Gold) |
| Fundo principal | `#EDE7DA` (Cream) |
| Fundo sections | `#FAF8F3` (White) / `#E4DDD0` (Cream2) |
| Fundo dark sections | `#1E1410` (Brown) |

---

## 🗂️ Seções da página

| ID | Seção |
|---|---|
| `#inicio` | Hero — headline, card bússola, bottom strip com timer |
| `#problema` | "Isso te soa familiar?" — ilustração SVG + texto |
| `#solucao` | O Método — 3 pilares |
| `#como-funciona` | 6 fases do programa |
| `#depoimentos` | Placeholder de vídeo de depoimento |
| `#oferta` | Tabela de entregáveis + card de preço com timer |
| `#faq` | 7 perguntas frequentes |
| `#cta-final` | CTA de fechamento |

---

## ⏱️ Timer de urgência

O countdown é de **24 horas** a partir do primeiro acesso do visitante.  
Ele persiste no `localStorage` com a chave `va_dl4` — ou seja, cada visitante tem seu próprio timer independente.

Para **resetar o timer** (ex: novo webinar), altere a chave no JS:
```js
var KEY = 'va_dl5'; // mude o número a cada campanha
```

---

## 📞 Suporte

Dúvidas sobre o projeto? Entre em contato via WhatsApp no rodapé da página.

---

*Método Velas Ajustadas™ · Todos os direitos reservados.*
