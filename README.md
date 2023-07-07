
## Documentação do Jogo Baseado em Texto

Esta documentação fornece uma visão geral, instruções de instalação e informações sobre as classes e estrutura do jogo baseado em texto implementado no código fornecido.

#### Visão Geral do Jogo

O jogo baseado em texto é um RPG simples onde o jogador controla um personagem e enfrenta combates com vários inimigos. O jogo inclui múltiplas opções de heróis para escolher, encontros aleatórios com inimigos, um sistema de combate baseado em turnos e ações como atacar, curar e fugir. A condição de vitória é derrotar todos os inimigos.

#### Instalação
Para executar o jogo baseado em texto, é necessário instalar as dependências necessárias e configurar o ambiente. Siga as etapas abaixo para começar:

#### Pré-requisitos
- O Node.js (versão 14 ou superior) deve estar instalado em seu sistema. Você pode baixá-lo no site oficial do Node.js: https://nodejs.org

- **Etapa 1:** Clonar o Repositório
Clone o repositório para o seu computador local usando o Git:

````bash
git clone <URL_do_repositório>
````
- **Etapa 2:** Instalar as Dependências
Navegue até o diretório do repositório clonado e instale as dependências necessárias usando o npm, o gerenciador de pacotes do Node.js:

#### Instalação npm
````bash
cd jogo-rpg
npm install
````
#### Instalação ts-node
```bash
npm install -g ts-node
```
#### Instalação prompt-sync
```bash
npm install -g prompt-sync
```
Isso irá baixar e instalar os pacotes necessários, incluindo ts-node e prompt-sync.

- **Etapa 3:** Iniciar o Jogo
  
Depois que as dependências forem instaladas, você pode iniciar o jogo executando o seguinte comando:
```bash
ts-node Main.ts
```
Isso executará o código TypeScript usando o ts-node e iniciará o jogo baseado em texto.

#### Instruções

Siga as instruções na tela para jogar o jogo. Você será solicitado a escolher um herói entre as opções disponíveis e, em seguida, poderá selecionar ações como lutar, curar ou fugir durante os encontros com os inimigos.

Use as teclas numéricas para fazer seleções e pressione Enter para confirmar sua escolha.

#### Classes e Estrutura do Jogo
O código do jogo inclui várias classes que representam os diferentes personagens e inimigos. Aqui está uma breve descrição de cada uma delas:

**Personagem:** A classe base para os personagens do jogo. Ela possui atributos como nome, pontos de vida, dano, defesa e métodos para atacar e receber ataques.

**Npc:** A classe base para os personagens não jogáveis (inimigos). Ela estende a classe Personagem e adiciona métodos específicos para os inimigos.

**Draconato:** Uma classe que representa um tipo específico de herói, o Draconato. Ela estende a classe Personagem e define os valores específicos para o Draconato, como nome, pontos de vida, dano, defesa, etc.

**Mago:** Uma classe que representa outro tipo de herói, o Mago. Ela também estende a classe Personagem e define os valores específicos para o Mago.

**Aranha, EsqueletoDeFogo, Lobo e Zumbi:** Classes que representam diferentes tipos de inimigos. Elas estendem a classe Npc e definem os atributos e comportamentos específicos de cada inimigo.


#### Notas Adicionais

O jogo utiliza a biblioteca prompt-sync para lidar com a entrada do usuário. Ela fornece uma maneira síncrona de obter entrada do usuário no console.
O jogo é implementado em TypeScript e transpilado para JavaScript usando o ts-node para execução.


















