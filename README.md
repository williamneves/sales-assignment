# SALES ASSIGNMENT

Esse é um teste para a vaga de Júnior Full Stack divulgada no Twitter de @drwilliamneves.

## Descrição

O projeto consiste em um sistema onde o vendedor vai lançar sua venda e no final conferir todas suas vendas efetuadas. Ele vai poder excluir uma venda e também poder editar uma venda. (TOTAL CRUD OPERATION)

Em uma outra página ele vai poder conferir as suas comissões por venda, de acordo com uma regra percentual.

### Objetivo Bônus

Seu manager, vai poder aprovar ou reprovar uma venda, e a comissão só será visível após a aprovação. O vendedor não pode ver a página de aprovação de venda do manager, e o manager não pode lançar vendas.

## Recomendação
Faça o clone desse projeto e inicie o repositorio em seu computador. Esse repositório só vem com o Next.js pré instalado.

```
yarn install
```
## REGRAS
**Páginas:**
- Login
- Cadastro de vendas
- Listagem de vendas
- Editar ou Excluir uma venda
- Visualização de comissão de cada venda (a forma de visualização é de acordo com o desenvolvedor).

**Tecnologias Obrigatorias:**
- Framework: Next.js (JavaScript)
- Database: Sanity.io
- Autenticação: Firebase

**CSS Framework:**

(O desenvolvedor pode escolher qual framework CSS ele deseja utilizar)
- Material UI é preferencial, porém, se não souber, não perca tempo aprendendo, use o framework CSS ou CSS Vailla que você for mais confortável.

### Schema desejado
Venda:
- id (objectId)
- nome do cliente (string)
- vendedor (referenceId)
- produto (string)
- valor (number)
- data (date)
- status (string) **(aprovado ou reprovado)** [opcional]
- comissão (number) [opcional]

User: (Opcional, se quiser usar apenas o auth user é possivel, porém se for para o objetivo bonus, é necessário criar um schema para o user)
- id (objectId)
- authUserId (ID do usuário do Firebase)
- role (string) admin ou vendedor

**Regra da comissão:**
- Vendas de até 400 reais: comissão de 1%
- Vendas de 400 a 800 reais: comissão de 2%
- Vendas de 800 a 1200 reais: comissão de 3% com bonus de 50 reais para a primeira do mês.
- Vendas de 1200 a 1600 reais: comissão de 4% com bonus de 100 reais para a primeira do mês.

Se as vendas totais do mês passarem de 10.000 reais, cada venda após bater esse valor terá um bonus de 1%.

### Deployment
- Ao final do projeto, o desenvolvedor deve fazer o deploy do projeto em https://vercel.com/.

### Requerir avaliação
Se você terminou o projeto, preencha o formulário abaixo:
- https://forms.gle/pH9iRZhSWMSvNyw66

### Dicas:
Leia as documentações:
- https://nextjs.org/docs/getting-started
- https://www.sanity.io/docs/overview-introduction
- https://firebase.google.com/docs/auth
