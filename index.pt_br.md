---

titulo: Documentação do KOOMPI OS

descrição: Descubra como usar o KOOMPI OS e todas as suas ferramentas e configurações.

---

# KOOMPI OS

Sinta a experiência GNOME Vanilla no Ubuntu com um pouco de tempero.

**Esta página é a documentação oficial dos componentes do KOOMPI OS.**\

Confira o  [**Manual**](https://handbook.koompios.org) para guias e tutoriais escritos pelo usuário.

## FAQ

Respostas às perguntas mais frequentes sobre o KOOMPI OS.

- **Por que uma nova Distribuição?**\

  O KOOMPI OS surgiu da necessidade de uma distribuição Linux baseada no Ubuntu que

  forneceria o GNOME vanilla sem nenhuma alteração para a experiência do usuário. Mais tarde, seu escopo foi estendido para experimentar algumas ferramentas e tecnologias, como ABRoot e pix (o subsistema baseado em Distrobox).

  

- **Ele usa OSTree?**\

  Não. O KOOMPI OS alcança a imutabilidade por meio de [`ABRoot`](https://github.com/koompi-os/ABRoot) [anteriormente alcançado através do utilitário `almost`]. O uso de OSTree pode ser considerado no futuro.

 

  Escrevemos o utilitário "almost" para imutabilidade sob demanda com base no

   atributo de imutabilidade dos arquivos. Essa abordagem funcionou em qualquer partição

   esquema/sistema de arquivos.

  

  Introduzimos um novo utilitário [ABRoot](https://github.com/koompi-os/ABRoot) substituindo o `almost` utilitário para fornecer total imutabilidade e atomicidade, transacionando entre 2 partições raiz (A⟺B). Ele também permite transações sob demanda por meio de um shell transacional.

  

- **Lançamento contínuo/Rolling Release?**\

  Não. O KOOMPI OS é de lançamento pontual e segue o ciclo de lançamento do Ubuntu.

## Guia do usuário

- **[Instalação](https://handbook.koompios.org/2022/11/05/installation.html)**

- **[Primeira configuração](https://handbook.koompios.org/2022/11/18/first-setup.html)**

- **[Atualizações](https://handbook.koompios.org/2022/12/10/updates.html)**

- **[Mais guias](https://handbook.koompios.org/)**

## Documentação dos componentes principais

- **[Pix](/docs/pix)**\

  é um gerenciador de pacotes baseado em contêiner que permite a instalação de pacotes de outras distribuições em um ambiente de sandbox.

- **[ABRoot](/docs/ABRoot)**\

  é um utilitário que permite transações totalmente atômicas entre 2 partições raiz (A⟺B).

- **[VSO](/docs/kso)**\

  é um utilitário que permite executar tarefas de manutenção na instalação do KOOMPI OS.

- ~~**[Almost](/docs/almost)**~~\

  ~~permite que você torne seu sistema imutável simplesmente alternando o atributo i dos arquivos.~~

## Contribuindo

- **[Packaging](/docs/packaging)**\

  programas para o KOOMPI OS requerem algumas considerações e diretrizes a serem seguidas.
