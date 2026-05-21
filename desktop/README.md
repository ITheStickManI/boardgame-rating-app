# PWA - Notas de Jogos de Tabuleiro

Este pacote contém os arquivos para publicar um app PWA simples de avaliação de jogos de tabuleiro.

## Arquivos

- `index.html`: aplicativo principal.
- `manifest.json`: configurações de instalação do PWA.
- `service-worker.js`: cache offline básico.
- `icons/icon-192.png` e `icons/icon-512.png`: ícones do app.

## Como testar localmente

O PWA precisa rodar em um servidor local ou em HTTPS. Não basta abrir o arquivo diretamente pelo Windows.

Opção simples com Python:

```bash
python -m http.server 8000
```

Depois acesse:

```text
http://localhost:8000
```

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub.
2. Envie todos os arquivos deste pacote para o repositório.
3. Vá em `Settings > Pages`.
4. Em `Source`, selecione a branch principal e a pasta `/root`.
5. Aguarde o GitHub gerar o link.
6. Abra o link no celular ou desktop e use a opção “Instalar app”.

## Observação

O botão “Salvar no aparelho” salva a última avaliação no `localStorage` do navegador.
