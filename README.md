# Raciocínio 

Para o dependency manager eu escolhi o yarn, pois acredito que a instalação de pacotes com ele é mais ágil.
Também escolhi utilizar o vite como ferramenta de compilação, pelo fato dele ser mais rápido e flexível.
E o framework escolhido foi o React, pois possuo mais experiência com ele.

Para a aplicação, eu escolhi resolver o problema que é a falta de uma ferramenta de gerenciamento de vagas de emprego, para uma melhor organização de quais vagas
a pessoa se candidatou, em qual ela está participando de um processo seletivo e tudo mais.

Resolvi utilizar o React Router Dom para facilitar o desenvolvimento das rotas, já que decici fazer uma home page além da dashboard.
Escolhi usar o styled-components também, pois possuo mais familiaridade do que o SASS e outros pré-processadores.
Também optei por utilizar o react-icons, para uma melhor vizualização das funções dos botões.
Para integração do projeto com a API escolhi utilizar o axios.
Para validação de formulário utilizei a biblioteca React Hook Form.
Utilizei também o react-toastify para uma melhor visualização das requisições da API.
 
Comecei a aplicação desenvolvendo a estrutura de rotas e definindo os estilos globais da aplicação. Logo após, comecei a desenvolver os componentes da aplicação, 
primeiramente pelo header e depois o form. O header foi bem simples, contendo apenas a logo da plataforma e um botão para voltar à homepage. Já o form foi um pouco
mais complexo, contendo todas as labels, os inputs, os selects e o botão de enviar.

Depois de terminar a estrutura e estilização do componente form. Comecei a desenvolver o context, para gerenciar os dados e evitar o prop drilling.
Com o state listVacancies no gerenciamento de estados globais, comecei a desenvolver o card e a lista de vagas.
No card utilizei a tag Link do react-router-dom para redirecionar o usuário para a página da vaga, criei o componente "DivCard" pois a estrutura se repetiria muitas vezes,
utilizei o operador ternário para mudar a cor do background da situação da vaga, e assim diferenciar as opções.
O próximo passo foi fazer a integração da API. Comecei criando o state loading, para que quando o usuário fizer a requisição, mostre a palavra "Carregando..." em quanto ele espera,
depois fiz a chamada o metodo POST passando os dados que o usuário inserir. E caso a requisição seja bem sucedida chama o toast de sucesso, caso contrário chama o toast de error.
Depois o criei um useEffect para que observasse um state, e cada fez que houvesse uma alteração nesse state chamasse o metodo GET, para atualizar a lista de vagas.
Por último criei o metodo DELETE, para que usuário possa deletar as vagas criadas.
Depois disso comecei a trabalhar no modal de edição do card e no metodo PUT. Porém deram muitos conflitos na aplicação, e acabei perdendo um tempo enorme na
tentativa de corrigir os bugs, e resolvi não implementar esse método pois ia atrasar muito a entrega desse teste.
No context eu deixei todos os states, as funções do formulário, as funções dos toasts e as requisições da API.

Por fim fiz a página Home bem básica e finalizei o teste.

## Como rodar a aplicação

1. Clone o repositório
2. Rode o comando "cd burh-desafio-frontend".
3. Rode o comando "cd my-vacancies".
4. Rode o comando "yarn" para instalar as dependências do projeto (utilize yarn pois foi dependency manager utilizado no desenvolvimento do projeto".
5. Utilize o comando "code ." para visualizar o código.
6. E rode o comando "yarn run dev" para abrir a aplicação em seu navegador.

## Dependências e tecnologias utilizadas
<ul>
  <li>React</li>
  <li>Styled-Components</li>
  <li>React-hook-form</li>
  <li>Axios</li>
  <li>React Router DOM</li>
  <li>React Toastify</li>
  <li>React-Icons</li>
  <li>Yarn</li>
  <li>Vite</li>
</ul>

# Contato
Guilherme K Hirata - <a href="https://www.linkedin.com/in/guilhermekhirata/" target="_blank">Linkedin</a> <br>
Email - guilhermekhirata@hotmail.com

