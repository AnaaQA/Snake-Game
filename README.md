
### <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> Snake-Game

  
 <p align="center">
  <img src="https://github.com/Nathan-Andrade/snakeGame/blob/master/github-pictures/gifSnakeGame.gif?raw=true"  width="400">
</p>

 ## :airplane: Tecnologias e Bibliotecas
<details><summary>Tecnologias</summary>

Este projeto foi desenvolvido com as seguintes tecnologias:


-   [HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
-   [CSS3](https://developer.mozilla.org/en-US/docs/Archive/CSS3)
-   [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)


## :information_source: Como rodar a aplicação
<p>
	Abra seu VS Code, em seguida clique com o botão direito do mouse sobre o arquivo `index.html` e selecione `Open with Live Server` ou `Open in Default Browser`.
	E por fim o mais importante de todos, DIVIRTA-SE BASTANTE !!
</p>


</details>

<p align="center">
  <img src="https://github.com/anandanobre/snake-game/blob/main/snakegame.gif" width="400" />
</p>

<details><summary><b>⚡Snake Game Código👈  Stats</b></summary>

# Snake Game(Jogo da cobrinha)
Jogo da cobrinha desenvolvido com pygame

<p align="center">
  <img src="https://github.com/anandanobre/snake-game/blob/main/snakegame.gif" width="400" />
</p>
<br />
Caso seja necessário instalação da biblioteca execute o seguinte comando no prompt do anaconta ou no terminal da IDE:

```
pip install pygame
```

</details>

## Watch my contribution graph eaten by the snake🐍
  ![snake gif](https://github.com/AnaTODOS/AnaTODOS/blob/output/github-contribution-grid-snake.svg)

<details><summary><b>⚡Snake Game Código👈  Stats</b></summary>


```diff

# Nome da Actions:  
name: Snake Game

# Controlador do tempo que sera feito a atualização dos arquivos.
on:
  schedule:
      # Será atualizado a cada 5 horas.
    - cron: "0 */5 * * *"

# Permite executar na na lista de Actions (utilizado para testes de build).
  workflow_dispatch:

# Regras
jobs:
  build:
    runs-on: ubuntu-latest
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Repositorio que será utilizado para gerar os arquivos.
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: AnaaQA  #Seu usuario
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

      - run: git status

      # Para as atualizações.
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

´´´

</details>
