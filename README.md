
# 😎💵 Economizaí | Sistema de Gestão de Finanças Pessoais 

**Autores:**
- [Gustavo Liros](https://github.com/GustavoLiros)
- [Matheus Delfino]()
- [Nathan Rosa](https://github.com/nathanferr)
- [Ryan Silva](https://github.com/ryan-aquino)


## 📚 Descrição
Este repositório contém os arquivos relacionados ao sistema do Trabalho de Graduação (TG) intitulado **"ECONOMIZAÍ - SISTEMA DE GESTÃO DE FINANÇAS PESSOAIS: PERSPECTIVAS E REFLEXÕES SOBRE CONTROLE DE ORÇAMENTOS"**. O TG foi desenvolvido como parte do curso de **[Análise e Desenvolvimento de Sistemas](http://www.fateccarapicuiba.edu.br/analise-e-desenvolvimento-de-sistemas/)** na **[FATEC - Carapicuíba](http://www.fateccarapicuiba.edu.br)**.

## 💻 Informações para o uso e modificações
Usado para produzir e funcionar:
* O servidor do banco de dados -> [MySql](https://dev.mysql.com/downloads/mysql/).
* Ferramenta visual MySql -> [MySQL Workbench](https://www.mysql.com/products/workbench/), mas funciona com outras (verificar compatibilidade).
* Node 18.17 -> https://nodejs.org/en.
* Vscode -> https://code.visualstudio.com.

---
Passos para o sistema funcionar (levando em consideração que possui os itens listados acima):

**1.** Abrir o Vscode, na pasta em que pretende guardar os arquivos.

**2.** Abrir o terminal do Vscode. Por padrão o atalho é **CTRL+`**.

**3.**  No terminal, utilizar o comando: `git clone [URL]`. Por exemplo, usando HTTPS:
   * `git clone https://github.com/nathanferr/economizai.git`
   * Para funcionar o git clone, é necessário ter instalado o [git](https://git-scm.com/downloads) no computador. A versão utilizada nesse projeto foi a 2.42.0 Windows, mas vai depender do tipo de sistema operacional da sua máquina.
   * Após clonar o repositório, é importante estar no diretório ***sistema***, para isso basta no terminal dar o comando: `cd economizai/sistema`

**4.** Ja no diretório correto, utilizar o comando `npm install`, para instalar os pacotes necessários do node, será criado uma pasta com o nome *node_modules*. É um pouco pesado, e dependendo da maquina e internet pode demorar um pouco, mas basta esperar.

**5.** Com tudo isso instalado, basta abrir o seu banco de dados, no caso desse projeto foi utilizado como principal o *MySQLWorkbench*.
   * Com ele aberto e configurado (usuario, senha e porta), é necessário que o arquivo ***config.example*** seja atualizado com as suas informações (ele se encontra dentro do diretório ***economizai/sistema***). Após isso, não se esqueça de renomeá-lo para ***config.js***.
   * Basta apenas atualizar os seguintes dados:
      * host: 'localhost' -> esse aqui geralmente não muda, mas caso o seu estiver diferente, é importante atualizar.
      * user: 'root' -> importante manter entre aspas simples e colocar o usuário que foi definido no seu banco de dados.
      * password: 'root' -> importante manter entre aspas simples e colocar a senha que foi definida no seu banco de dados.
      * port: 3306 -> Colocar a porta do seu banco de dados, geralmente é 3306 ou 3310, mas vai depender da sua configuração.
   * Com tudo configurado, basta abrir dentro do seu banco de dados o arquivo com nome de ***iniciar.sql*** (ele se encontra no diretório ***economizai/banco***). Ao abrir, rode o script no banco.

**6.** Com o banco de dados aberto, funcionando e com o banco ***economizaiDB*** cadastrado (depois de rodar o script), volte ao terminal, no VsCode, e rode o comando `npm run dev`. Lembre-se, que o terminal, deve estar no diretório ***economizai/sistema***.

**7.** Por fim, após rodar o comando no terminar, aparecerá uma mensagem monstrando um "link", onde estará rodando o sistema, basta abrir o navegador (chrome, opera, edge, o de sua preferência) e colococar na barra de pesquisa acima o link. Normalmente ele é -> ***localhost:3000***.

***Qualquer dúvida, sugestão ou problema relacionado ao projeto, fique a vontade para entrar em contato conosco 🙂.***
