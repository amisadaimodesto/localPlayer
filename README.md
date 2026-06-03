[![CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

# localPlayer

Um reprodutor de áudio moderno, construído com tecnologias web nativas (HTML, CSS e JavaScript), projetado para rodar **100% offline** diretamente no seu navegador. 

## ✨ Funcionalidades

* **Leitura de Metadados (ID3 Tags):** Extração automática do título da faixa, álbum, artista e da **capa (Album Art)** embutida no arquivo usando a biblioteca [jsmediatags](https://github.com/aadsm/jsmediatags).
* **Espectrograma Dinâmico:** Visualização das ondas sonoras em tempo real utilizando a *Web Audio API* e a *Canvas API*.
* **Playlist Inteligente:** Lista elegante que quebra nomes longos corretamente, calcula a duração de cada faixa e exibe a música atualmente em reprodução.
* **Controles de Reprodução:**
    * Tocar / Pausar
    * Próxima / Anterior
    * Aleatório (Shuffle)
    * Repetir Todos (Repeat)
    * Repetir Um (Repeat One)
* **Customização Local:** Possibilidade de alterar a imagem de fundo do player, com salvamento da preferência no cache do navegador (`localStorage`).
* **Privacidade Total:** Como o projeto processa os arquivos de áudio via `URL.createObjectURL()`, nenhuma música é enviada para servidores. Tudo roda diretamente na sua máquina.

## 🚀 Como usar

1. Clone ou baixe este repositório.
2. Abra o arquivo `index.html` em qualquer navegador moderno.
3. Clique em **Selecionar músicas** e escolha um ou mais arquivos `.mp3` do seu computador.
4. (Opcional) Escolha uma imagem em **Plano de fundo** para personalizar seu player.

## 🛠️ Tecnologias Utilizadas

* **HTML5**
* **CSS3** (Flexbox, Backdrop-filter para efeito Glassmorphism)
* **JavaScript (Vanilla)**
    * File API
    * Web Audio API
    * Canvas API
    * Local Storage
* [**jsmediatags**](https://github.com/aadsm/jsmediatags) (Leitura de ID3 tags)

## 📁 Estrutura do Projeto

\`\`\`text
meu-player-mp3/
├── index.html           # Estrutura principal
├── README.md            # Documentação
├── css/
│   └── style.css        # Estilos e design
└── js/
    ├── jsmediatags.min.js # Biblioteca para leitura de tags ID3
    └── script.js        # Lógica do player e visualizador
\`\`\`
