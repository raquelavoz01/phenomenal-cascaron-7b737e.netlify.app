# Estúdio de Histórias IA 📚

Bem-vindo ao Estúdio de Histórias IA, sua assistente criativa para dar vida a mundos, personagens e narrativas épicas. Este aplicativo web utiliza o poder da IA generativa da Google (Gemini) para ajudar escritores a criar livros completos, desde o conceito inicial até os capítulos detalhados e a narração em áudio.

## ✨ Funcionalidades

- **Biblioteca Pessoal:** Crie e gerencie múltiplos livros em sua própria biblioteca digital.
- **Importação e Exportação:** Salve e carregue toda a sua biblioteca com um único arquivo JSON.
- **Conceituação Detalhada:** Defina o título, o cenário e crie personagens únicos com descrições e vozes de narração distintas.
- **Geração por IA:**
    - **Capas de Livro:** Gere capas de livro fotorrealistas e impressionantes com base no conceito da sua história.
    - **Sinopse e Tags:** Crie uma sinopse envolvente e tags relevantes para o seu livro com um clique.
    - **Esboço da História:** Desenvolva um esboço detalhado com dezenas de capítulos, cada um com um plano de eventos e desenvolvimento de personagens.
    - **Escrita de Capítulos:** Expanda cada item do esboço em um capítulo completo e detalhado, com mais de 4.000 palavras.
- **Editor Integrado:** Edite e refine o conteúdo gerado pela IA diretamente no aplicativo.
- **Leitor com Narração:** Ouça sua história ganhar vida com uma narração em áudio multi-falante, onde cada personagem (e o narrador) tem sua própria voz.

## 🛠️ Tecnologias Utilizadas

- **Frontend:** React, TypeScript, Vite
- **API de IA:** Google Gemini API (modelos Flash, Flash Image e TTS)
- **Backend:** Netlify Functions (Serverless)
- **Estilização:** CSS puro com variáveis

## 🚀 Configuração e Deploy

Para rodar este projeto, você precisará de uma chave de API do Google Gemini e uma conta na Netlify.

### 1. Obtenha sua Chave de API

1.  Acesse o [Google AI Studio](https://makersuite.google.com/app/apikey).
2.  Clique em "Create API key in new project" para gerar sua chave.
3.  Copie a chave. Você precisará dela no próximo passo.

### 2. Configuração na Netlify

Este projeto é configurado para ser implantado facilmente na Netlify.

1.  **Faça o Fork ou Clone do Repositório:** Coloque o código em sua conta do GitHub.
2.  **Crie um Novo Site na Netlify:**
    - Na Netlify, clique em "Add new site" -> "Import an existing project".
    - Conecte ao seu provedor Git (GitHub) e selecione o repositório do projeto.
3.  **Configure a Variável de Ambiente:**
    - Nas configurações do seu site na Netlify, vá para **Site configuration** → **Build & deploy** → **Environment**.
    - Clique em **New variable**.
    - Insira **exatamente** o seguinte:
        - **Key:** `API_KEY`
        - **Value:** Cole a chave de API que você copiou do Google AI Studio.
4.  **Acione o Deploy:**
    - Vá para a aba **Deploys** e clique em **"Trigger deploy" → "Deploy site"**.
    - **Este passo é crucial!** A Netlify só aplicará a nova variável de ambiente após um novo deploy.

O arquivo `netlify.toml` na raiz do projeto já contém todas as configurações de build necessárias, então a Netlify deve construir e implantar o site e a função serverless automaticamente.

## ✍️ Como Usar

1.  **Crie um Novo Livro:** Na tela da biblioteca, clique em "+ Criar Novo Livro".
2.  **Defina o Conceito:** Dê um título ao seu livro, adicione personagens (com nomes, descrições e vozes) e descreva o cenário.
3.  **Gere a Capa e Sinopse:** Use os botões na seção 2 para que a IA crie uma capa e uma sinopse para sua história.
4.  **Gere o Esboço:** Clique em "Gerar Esboço com IA". A IA criará uma lista de capítulos com um plano para cada um.
5.  **Escreva os Capítulos:** Para cada item no esboço, clique em "Escrever" para que a IA gere um capítulo completo.
6.  **Edite e Refine:** Após a geração, você pode expandir, editar e refinar cada capítulo conforme desejar.
7.  **Leia e Ouça:** Quando tiver capítulos escritos, vá para a tela de leitura para ler sua história ou ouvi-la sendo narrada pela IA.
