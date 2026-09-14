# Distribuição do Grill Me via QR Code

## Fluxo

```text
QR Code
  ↓
https://[SEU-DOMINIO]/grill-me
  ↓
Página simples
  ↓
Botão "Baixar Grill Me"
  ↓
grill-me.md
```

O funcionário **não** precisa abrir GitHub.

## O que já está pronto neste projeto

| Caminho | Função |
|---------|--------|
| `site/grill-me/index.html` | Página amigável de download |
| `site/grill-me/grill-me.md` | Arquivo que o botão baixa |
| `site/index.html` | Redireciona `/` → `/grill-me/` |
| `grill-me.md` (raiz) | Cópia de trabalho / espelho do arquivo |
| `manual-demanda-ia-grill-me.md` | Versão de edição do conteúdo |

## URL deste projeto

Repositório: https://github.com/tiCalpar/jornada-ia

Depois de ativar o GitHub Pages (pasta `/site`), a URL pública esperada é:

```text
https://ticalpar.github.io/jornada-ia/grill-me/
```

O QR Code deve apontar para essa URL (ou para um domínio próprio que redirecione para ela).

O botão **Baixar Grill Me** já aponta para `./grill-me.md` na mesma pasta da página — não precisa apontar para o GitHub.

## Como publicar (opção simples: GitHub Pages)

1. Suba este repositório no GitHub.
2. Em **Settings → Pages**:
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/site` (ou `/docs` se preferir mover a pasta)
3. Se a pasta publicada for `site`, a URL fica:
   - `https://SEU-USUARIO.github.io/NOME-DO-REPO/grill-me/`
4. (Opcional) Configure um **domínio próprio** apontando para o GitHub Pages.
5. QR Code aponta para o domínio próprio `/grill-me`.

> Se o Pages só publicar a raiz do repo, mova o conteúdo de `site/` para a raiz ou para `/docs` e ajuste a configuração.

## Atualizar o arquivo sem mudar o QR

1. Edite `manual-demanda-ia-grill-me.md` (conteúdo).
2. Copie para:
   - `grill-me.md`
   - `site/grill-me/grill-me.md`
3. Publique/atualize o site.
4. O mesmo QR continua válido.

## Gerar o QR Code

Quando a URL final existir, gere o QR apontando **somente** para ela.

Ferramentas comuns:

- Canva (QR Code nativo)
- https://qr.io / https://goqr.me
- Extensão/gerador interno da empresa

Texto do QR (exemplo):

```text
https://[SEU-DOMINIO]/grill-me
```

Coloque esse QR no vídeo da Clara (cena final / CTA).

## O que NÃO fazer

- Não apontar o QR direto para `raw.githubusercontent.com/...`
- Não apontar para a página do repositório no GitHub
- Não escrever “Markdown”, “GitHub” ou “repositório” na página do funcionário
