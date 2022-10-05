# Preparando o ambiente

 Para este projeto rodar, precisaremos instalar três ferramentas: __Cypress__ , __NodeJS__ necessário para executar código __JavaScript__ e o __Visual Studio Code ou VSC__, editor que usamos para escrever código.
<br>

#### NodeJS

- **1.** Abra uma janela do terminal em seu computador. Isso pode ser feito da seguinte forma:
<br>

-  __Windows:__ Você pode acessar a busca no menu inicial e procurar por Prompt de Comando, ou acessar via Menu Iniciar > Sistema do Windows > Prompt de Comando.

- __MacOs:__ O Terminal está disponível no menu de Aplicações, dentro da pasta de Utilitários.

- __Linux__ (Ubuntu): O Terminal está disponível no menu de Programas/Aplicações. Caso não localize, pode estar dentro da pasta Utilitários.
<br>

- **2.** No terminal, digite node **--version** ou **node -v**  caso retorne um número de versão, como por exemplo, **v16.13.1**, o NodeJS já está instalado.
<br>

- Caso precise instalar, siga as instruções para cada sistema operacional que estão na <a href="https://nodejs.org/pt-br/">página inicial do NodeJS.</a></p>
<br> 
- O site do NodeJS oferece duas opções para download, a LTS e a "current" (atual), conforme imagem abaixo. Você pode escolher a versão LTS (Long Term Support, ou Suporte a Longo Prazo) e clicar no botão correspondente para baixar e instalar normalmente como qualquer outro programa.
<img src="https://user-images.githubusercontent.com/98066667/193942963-a61b7b8e-1734-40b1-ad6c-d89ecc2e3c34.png">
<br>
## Instalação do Cypress

O Cypress é um framework para automação de testes end-to-end, que utiliza o __JavaScript__ como linguagem de programação. Caso queira o  projeto com exatamente a mesma versão que estou usando, para não ter diferenças em nomenclatura de arquivos, faça a sua instalação fixando a versão na mesma que eu estou utilizando, através do comando:<
br>
````npm install cypress@10.3.1 --save -include=dev ````

Dessa forma, não haverá diferenças de telas ou implementações.

**Documentação do cypress para instalação:**
- [cypress](https://www.cypress.io/)

### Instalação Visual Studio Code

O Visual Studio Code é o editor que escolhemos utilizar para escrever nossos códigos durante este curso. Os links para baixar e instalar de acordo com o seu sistema operacional estão na página inicial do VSC.

- [Visual studio code](https://code.visualstudio.com/)

Após concluí as instalações. Abra o terminal e  digita o comando npx cypress open ou npm run test, caso tenha incluído o comando anterior no script test do arquivo package.json conforme eu oriento abaixo:



### Execuções:
colocando esse comando dentro de **package.json** para abrir o cypress via terminal.
```
{
    "scripts": {
    "cy:run": "npx cypress open "
    }
} 
```
- segue lo link de mais comandos de execução na [documentação](https://docs.cypress.io/guides/guides/command-line#How-to-run-commands) 

### variáveis de ambientes

Você precisa criar seu próprio cypress.env.json arquivo que o Cypress verificará automaticamente. A seguir deve adicionar **cypress.env.json** ao seu **.gitignore** arquivo, os valores aqui pode ser diferente para cada máquina local.

```
{
  "user_name": "seu e-mail",
  "password": "sua senha"
}
```
 

- [Documentação das variáveis de ambientes](https://docs.cypress.io/guides/references/configuration#Configuration-File)

## Rodando os testes

Na primeira abertura do Cypress, quando você digita o comando npx cypress open ou npm run test, caso tenha incluído o comando anterior no script test do arquivo package.json, vai aparecer a seguinte tela nova:

<img src="https://cdn1.gnarususercontent.com.br/1/40407/642de4e3-8e2c-4707-b480-d5692263c27e.png" style="width:900px;height:300px" >

Nessa tela você irá escolher **E2E Testing**, em sequência, uma nova tela que mostra todos os navegadores instalados, para que você escolha qual irá utilizar inicialmente.

<img src="https://cdn1.gnarususercontent.com.br/1/40407/ed906de9-810e-4e0c-8eda-5ee91b4a806f.png" style="width:900px;height:300px" >

Depois de selecionado, você vai marcar a opção **Start E2E Testing in navegador** escolhido.


























