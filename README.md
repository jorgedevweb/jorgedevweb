### Oi! Eu sou o Jorge Luiz 👋


- 🔭 Hoje trabalho com programação de máquinas
- 🌱 Estudadndo: Angular, Sistemas para Internet e PHP
- 📫 Contate-me no e-mail: jorgeluiz.devweb@gmail.com
<div style ="display: inline_block"><br>
<img width="40px" 
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" vspace="50px" />
  <img width="40px"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" vspace="50px" />
<img width="40px"
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" vspace="50px"/>
<img width="40px"
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" vspace="50px"/>
<img width="40px"
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" vspace="50px"/>
<img width="40px"
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg" vspace="50px"/>
<img width="40px"
src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original-wordmark.svg" />
</div>

 ![Snake animation](https://github.com/jorgedevweb/jorgedevweb/edit/main/README.md)

 name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          
                  
          
          
          
          

