# Deploy · Scavaseg

Protótipo encriptado (StaticCrypt AES-256, roda 100% no navegador). Senha: `scavaseg-seguros-2026`

## Passos (Gustavo)
1. Criar repo em github.com/new. Como o índice é encriptado, pode ser **público** (necessário para GitHub Pages no plano Free).
2. Subir os arquivos desta pasta (index.html, CNAME, .nojekyll) para a raiz do repo (branch main).
3. Ativar GitHub Pages (Settings → Pages → branch main / root) e aguardar o certificado HTTPS provisionar.
4. DNS no **Wix**: Domínios → guilds.com.br → Registros DNS → CNAME host `scavaseg-seguros` valor `SEU_USUARIO.github.io`.
5. Só mandar o link ao cliente DEPOIS do HTTPS pronto (StaticCrypt só funciona em https://).

O método de push + Pages + HTTPS via token está no runbook da skill (references/runbook.md).

## Mensagem para o cliente (WhatsApp)
> Oi Scavaseg! Preparei uma prévia navegável do sistema. Acesse https://scavaseg-seguros.guilds.com.br e use a senha `scavaseg-seguros-2026`. Dá uma olhada com calma e me conta o que achou 🤝

## Segurança
- O conteúdo do protótipo NÃO fica em texto claro no HTML (está encriptado). Repo público é seguro.
- Para trocar a senha, rode o encrypt-deploy.sh de novo com a nova senha.
