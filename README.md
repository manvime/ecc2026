# Livro ECC 2026

Flipbook com as 41 páginas do PDF enviado, na ordem original. Exibe a capa original e as folhas com efeito de virar páginas, sem títulos ou capas adicionais. A senha de leitura foi entregue separadamente na conversa.

## Como publicar

1. Extraia o ZIP. Envie os arquivos extraídos, não o próprio ZIP.
2. No repositório **manvime/ecc2026**, abra **Add file → Upload files**.
3. Envie `index.html`, `livro-pdf.enc`, `README.md` e `LICENCA_StPageFlip.txt` diretamente para a raiz do repositório, substituindo os arquivos de mesmo nome. Para atualizar a edição do livro, envie `index.html` e `livro-pdf.enc` juntos. Para atualizar somente o leitor da edição oficial de 41 páginas, basta substituir `index.html`. Se aparecer, envie também `.nojekyll` (opcional neste site HTML pronto).
4. Salve com **Commit changes** na branch `main`.
5. Abra **Settings → Pages**. Escolha **Deploy from a branch**, branch **main** e pasta **/(root)**. Clique em **Save**.
6. Aguarde a publicação e abra o endereço indicado em **Visit site**. Esse é o endereço para compartilhar e usar em um QR code.

Se usar o plano GitHub Free, o repositório precisa ser público para publicar pelo Pages. O livro continua criptografado, e somente a tela de senha fica visível antes de desbloquear.

Cada arquivo deste pacote fica abaixo do limite de 25 MiB para envio pelo navegador. No celular, pode ser necessário ativar a versão para computador do site do GitHub para encontrar as opções.

## Uso

- Abra o site publicado por HTTPS e digite a senha informada na conversa.
- Vire as folhas pelas setas ou deslizando o dedo. No computador, também funcionam as setas do teclado.
- Afaste dois dedos sobre a folha para ampliar e aproxime para reduzir. Com a folha ampliada, arraste com um dedo para ler outras partes.
- O botão de download fornece o PDF original após desbloquear o livro. O PDF só é transferido quando solicitado.
- O cadeado fecha o livro. Recarregar a página pede a senha novamente.

## Conteúdo protegido

`index.html` contém o leitor e as imagens criptografadas; `livro-pdf.enc` contém o PDF original criptografado. Mantenha os dois arquivos na mesma pasta, com os mesmos nomes.

Não envie o PDF original, as imagens das páginas ou a senha ao repositório. Não escreva a senha neste README. Para trocar a senha, é necessário gerar novamente os arquivos criptografados. Quem recebe a senha pode ler, baixar e compartilhar o livro.

A proteção usa AES-256-GCM e PBKDF2-HMAC-SHA256 com 600.000 iterações. Não há rastreadores nem dependências de CDN. A senha não é armazenada no navegador nem incluída nos arquivos. As páginas são carregadas conforme a leitura para reduzir o uso de memória no celular.

## Referências

- https://docs.github.com/pt/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

Pacote pronto para envio. A hospedagem é ativada no seu GitHub.
