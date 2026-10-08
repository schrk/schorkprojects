# Schork Projects

Site institucional da Schork Projects — consultoria de desenvolvimento com IA, fundada em abril de 2026.

É um site estático de um único arquivo (`index.html`), sem build. Basta abrir no navegador.

## Publicar no seu domínio (GitHub Pages)

1. Faça o merge deste branch no `main`.
2. No GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: `main` / pasta `/ (root)` → **Save**
3. Ainda em **Settings → Pages**, em **Custom domain**, digite seu domínio (ex.: `schorkprojects.com`) e salve.
   O GitHub cria o arquivo `CNAME` no repositório automaticamente.
4. No painel do seu registrador de domínio (Registro.br, GoDaddy, Hostinger, Cloudflare etc.), crie os registros DNS:

   | Tipo  | Nome  | Valor                  |
   |-------|-------|------------------------|
   | A     | @     | 185.199.108.153        |
   | A     | @     | 185.199.109.153        |
   | A     | @     | 185.199.110.153        |
   | A     | @     | 185.199.111.153        |
   | CNAME | www   | `schrk.github.io`      |

5. Aguarde a propagação do DNS (de minutos até algumas horas) e marque **Enforce HTTPS** em Settings → Pages.

> O GitHub Pages em repositório **privado** exige plano pago (GitHub Pro/Team). Com o plano gratuito, o repositório precisa ser público.

## Personalizar

- E-mail de contato: procure `contato@schorkprojects.com` no `index.html` e troque pelo seu.
- Cores: variáveis CSS em `:root` no topo do `index.html` (`--accent` é a cor de destaque).
