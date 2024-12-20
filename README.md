## Pomodoro Timer com Avisos de Voz

Este repositório contém um script para gerenciar sessões de Pomodoro (trabalho e descanso) no seu terminal, com avisos sonoros e mensagens no terminal. O script utiliza as ferramentas `timer` e `spd-say`, e oferece um toque divertido com `lolcat` para imprimir as mensagens.

Funcionalidade

O script define duas opções principais de Pomodoro:

- Sessão de Trabalho (45 minutos): Usada para períodos de trabalho focado.
- Pausa (10 minutos): Usada para descanso ou pausa breve entre as sessões de trabalho.

Ao final de cada sessão, o script emite um aviso com uma mensagem de voz usando o comando `spd-say` e exibe uma mensagem no terminal.

## Requisitos

Para que o script funcione corretamente, é necessário instalar algumas dependências:

- Go (necessário para instalar o `timer`)
- spd-say (para emitir os avisos de voz)
- lolcat (opcional, para adicionar um toque divertido às mensagens no terminal)

## Instalando Dependências

1. Instalar o Go:
   - Siga as instruções de instalação do Go (https://go.dev/doc/install) para o seu sistema operacional.

2. Instalar o `spd-say`:
   Para distribuições baseadas em Debian (como Ubuntu e Mint), use o comando abaixo:

`sudo apt install speech-dispatcher`

3. Instalar o `lolcat` (opcional):
   Se você deseja adicionar uma fala divertida no terminal, instale o `lolcat` com o comando:

   `sudo apt install lolcat`

4. Instalar o `timer`:
   Com o Go instalado, execute o seguinte comando para instalar o `timer`:

   ```go install github.com/caarlos0/timer@latest ```

Como Usar

1. Baixar o Script

Clone este repositório ou copie o script para o seu diretório de preferência:

``` git clone https://github.com/seu-usuario/pomodoro-timer.git ```

```cp pomodoro-timer/pomodoro.sh ~/pomodoro.sh```

2. Tornar o Script Executável

Dê permissão de execução para o script:

``` chmod +x ~/pomodoro.sh ```

3. Adicionar Aliases no seu Shell

Para tornar os aliases permanentes, adicione a linha abaixo ao seu arquivo de configuração do shell (~/.bashrc, ~/.zshrc, etc.):

source ~/pomodoro.sh

Depois disso, aplique as configurações:

``` source ~/.bashrc  # Ou ~/.zshrc, se estiver usando Zsh ``` 

4. Usar o Pomodoro

Agora você pode iniciar as sessões de Pomodoro diretamente no seu terminal usando os seguintes comandos:

- Iniciar uma sessão de trabalho de 45 minutos:

  wo

- Iniciar uma pausa de 10 minutos:

  br

Ao final de cada sessão, o sistema emitirá um aviso com o comando `spd-say` e imprimirá uma mensagem no terminal.

Contribuições

Sinta-se à vontade para contribuir com melhorias, abrir issues ou sugerir novos recursos para este projeto. Para isso, basta criar um *pull request* ou abrir uma *issue*.

Licença

Este projeto está licenciado sob a Licença MIT.
