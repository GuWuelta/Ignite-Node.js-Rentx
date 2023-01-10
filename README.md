# Requisitos do Projeto

## Cadastro de carros

**RF**

> - Deve ser possível cadastrar um novo carro;

**RN**

> - Não deve ser possível cadastrar um carro com uma placa já existente;
> - O carro deve ser cadastrado com disponibilidade por padrão;
> - Para cadastrar um carro o usuário deve ser um administrador.

## Listagem de carros

**RF**

> - Deve ser possível listar todos os carros disponíveis;
> - Deve ser possível listar todos os carros disponíveis pelo nome da categoria;
> - Deve ser possível listar todos os carros disponíveis pelo nome da marca;
> - Deve ser possível listar todos os carros disponíveis pelo nome do carro.

**RN**

> - Não é necessário que o usuário esteja logado para a listagem de carros.

## Alteração de carros

> - Não deve ser possível alterar a placa de um carro já cadastrado;

## Cadastro de especificação no carro

**RF**

> - Deve ser possível cadastrar uma especificação para um carro;

**RN**

> - Não deve ser possível cadastrar uma especificação para um carro não cadastrado;
> - O usuário responsável pelo cadastro deve ser um usuário administrador.
> - Não deve ser possível cadastrar uma mesma especificação já existente para o mesmo carro;

## Cadastro de imagens do carro

**RF**

> - Deve ser possível cadastrar a imagem do carro;

**RNF**

> - Utilizar o multer para upload dos arquivos;

**RN**

> - O usuário deve poder cadastrar mais de uma imagem para o mesmo carro;
> - O usuário responsável pelo cadastro deve ser um usuário administrador.

## Aluguel de carros

**RF**

> - Deve ser possível cadastrar um aluguel

**RN**

> - O usuário deve estar logado;
> - O aluguel deve ter duração mínima de 24 horas;
> - Não deve ser possível cadastrar um novo aluguel para um mesmo usuário;
> - Não deve ser possível cadastrar um novo aluguel para um carro que já está alugado;
> - Ao realizar um aluguel o status do carro deverá ser alterado para indisponível.

## Devolução de carros

**RF**

> - Deve ser possível realizar a devolução de um carro

**RN**

> - O usuário deve estar logado;
> - Se o carro for devolvido em menos de 24 horas, deverá ser cobrado a diária completa;
> - Ao realizar a devolução, o carro deverá ser liberado para outro aluguel;
> - Ao realizar a devolução, deverá ser calculado o total do aluguel;
> - Se o carro for devolvido após o horário previsto de entrega, deverá ser cobrado multa proporcional ao período de atraso;
> - Caso haja multa, deverá ser somada ao total do aluguel.

## Listagem de Alugueis para usuário

**RF**

> - Deve ser possível realizar a busca de todos os aluguéis para o usuário.

**RN**

> - O usuário deve estar logado na aplicação.

## Recuperação de Senha

**RF**

> - Deve ser possível para o usuário recuperar a senha informando o e-mail;
> - O usuário deve receber um e-mail com o passo a passo para a recuperação de senha;
> - O usuário deve conseguir inserir uma nova senha.

**RN**

> - O usuário deve informar uma nova senha.
> - O link enviado para a recuperação de senha deve expirar em 3 horas.