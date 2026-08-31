# Método Paccola 4D — landing page

Página de vendas independente, arquivo único (`index.html`), sem build step. Pronta pra subir direto no GitHub + Vercel.

## Subir no GitHub

```bash
cd deploy
git init
git add index.html
git commit -m "Landing page Método Paccola 4D"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
git push -u origin main
```

## Publicar no Vercel

Não precisa de `vercel.json` nem de build command — é HTML estático puro.

**Opção 1 — pelo site:**
1. Entre em [vercel.com/new](https://vercel.com/new) e importe o repositório do GitHub.
2. Em "Framework Preset", deixe **Other**.
3. Build Command e Output Directory podem ficar em branco (o Vercel serve o `index.html` da raiz automaticamente).
4. Deploy.

**Opção 2 — pela CLI:**
```bash
npm i -g vercel
cd deploy
vercel --prod
```

## Antes de publicar de verdade

Alguns pontos que ainda estão como placeholder ou pendentes de confirmação (marcados em `.fine` no rodapé de cada seção):

- Números de mercado (fontes citadas, mas confirme os mais recentes antes de publicar).
- Nome completo, cidade e autorização de uso das avaliações/depoimentos reais (Google + print de WhatsApp).
- Todos os botões de candidatura já apontam para `https://paccolaacademy.com.br/captura`.

## Domínio próprio

Se quiser um domínio diferente do `*.vercel.app`, adicione em Project Settings → Domains no painel do Vercel depois do primeiro deploy.
