# phishqr
Ferramenta de conscientização de Phishing através da utilização de QR code

## Descrição
O Phish QR é uma ferramenta que demonstra o uso do QR Code no cenário de Phishing, permitindo o acesso a contas apenas escaneando o QR Code malicioso. Este projeto foi desenvolvido originalmente por Kuba Gretzky (https://github.com/kgretzky/evilqr). A versão presente neste repositório foi baseada na original e possui modificações, como templates em português, título e ícone dinâmico da página conforme o template, entre outras melhorias.

Este projeto consiste em duas partes.

A primeira parte é uma extensão de navegador usada pelo atacante para coletar o QR code de login de aplicativo e enviar uma requisição para o nosso servidor (parte 2) contendo o QR Code.

Na segunda parte, temos o nosso servidor HTTP, onde o QR Code coletado pelo atacante será exibido nas páginas de phishing.

## Instalação
- Clone este repositório:
git clone https://github.com/whoamigod/phish-qr-client.git

- Carregue a extensão no navegador Chrome:
1. Abra a página de extensões: `chrome://extensions/`
2. Ative o modo de desenvolvedor.
3. Clique em "Carregar sem compactação" e selecione o diretório do repositório.

## Uso
- Inicie o servidor executando o './servidor/build_run.bat'
![image](https://github.com/whoamigod/phishqr/assets/124740533/d1ef3d8b-abe1-40c0-bc3d-4f6561d52691)

- Abra um dos sites suportados em seu navegador (com a extensão já instalada)
  ![image](https://github.com/whoamigod/phishqr/assets/124740533/3d5cc7ef-9207-4cd0-9a6b-9b5bab8941c3)

- Após a página carregar completamente, clique na extensão para ativar ela.
Abra o URL da página de phishing do servidor: http://127.0.0.1:35000(padrão) 
