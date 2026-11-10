# Berinscape

Jogo de fantasia medieval para navegador.

**[Jogar Berinscape](https://vitorjow-ui.github.io/berinscape/)**

Controles: WASD/setas ou clique para andar; Shift para correr; roda do mouse para zoom; Esc para pausar. O progresso fica salvo no navegador.

## Código e recursos

O envio inicial foi feito pelo navegador: o código está em `berinscape-source.zip` e os recursos nas partes `assets-pack.partNNN`. Backups, protótipos antigos e modelos de produção não fazem parte do repositório.

Para desenvolver, baixe o repositório completo e extraia `berinscape-source.zip` na raiz. Execute:

```sh
python Berinscape/tools/build_site.py
python Berinscape/tools/serve.py
```

O primeiro comando verifica e extrai os recursos, depois prepara `dist/`. O servidor local está em http://127.0.0.1:8765; consulte as instruções dentro do ZIP para detalhes.

## Publicação

O workflow `.github/workflows/pages.yml` reconstrói e publica o jogo no GitHub Pages quando há alterações na branch `main`. Para mudar o código nesta forma de distribuição, atualize o ZIP preservando a pasta `Berinscape/`.

Requer internet para carregar Three.js. A versão atual foi preparada para teclado e mouse. Os créditos completos acompanham o jogo e estão nas configurações e em `Berinscape/docs/licenses/` dentro do pacote de código.
