# Requisitos do SoloCalc

## 1. Objetivo do sistema

O SoloCalc é um sistema desenvolvido para auxiliar na organização e interpretação de dados de análise de solo, permitindo realizar recomendações de calagem e adubação de acordo com a metodologia definida para o projeto.

O sistema tem como objetivo facilitar o trabalho de organização dos dados e reduzir a necessidade de realizar cálculos manualmente.

---

## 2. Requisitos Funcionais

### RF01 — Cadastro de usuários

O sistema deverá permitir o cadastro de usuários autorizados a utilizar a aplicação.

### RF02 — Autenticação

O sistema deverá permitir que os usuários realizem login utilizando suas credenciais.

### RF03 — Controle de acesso

O sistema deverá controlar o acesso às funcionalidades de acordo com o perfil do usuário.

### RF04 — Cadastro de produtores

O sistema deverá permitir cadastrar, consultar, alterar e excluir produtores.

### RF05 — Cadastro de propriedades

O sistema deverá permitir cadastrar propriedades relacionadas aos produtores.

### RF06 — Cadastro de talhões

O sistema deverá permitir cadastrar talhões relacionados às propriedades.

### RF07 — Cadastro de culturas

O sistema deverá permitir cadastrar e consultar culturas agrícolas.

### RF08 — Cadastro de análise de solo

O sistema deverá permitir registrar os dados de uma análise de solo, incluindo informações como:

* pH;
* V% atual;
* CTC;
* cálcio (Ca);
* magnésio (Mg);
* potássio (K);
* fósforo (P);
* H+Al;
* argila;
* data da análise;
* observações.

### RF09 — Cálculo de calagem

O sistema deverá calcular a necessidade de corretivo de acidez do solo de acordo com a metodologia adotada no projeto e apresentar o resultado em toneladas por hectare.

### RF10 — Cálculo de adubação

O sistema deverá calcular a recomendação de adubação de acordo com os dados da análise de solo, da cultura e da metodologia adotada no projeto.

### RF11 — Cadastro de corretivos

O sistema deverá permitir cadastrar os corretivos utilizados nos cálculos, incluindo as informações necessárias para a recomendação.

### RF12 — Cadastro de fertilizantes

O sistema deverá permitir cadastrar fertilizantes e suas respectivas características.

### RF13 — Registro de recomendações

O sistema deverá armazenar as recomendações calculadas pelo sistema.

### RF14 — Histórico

O sistema deverá permitir consultar recomendações realizadas anteriormente.

### RF15 — Relatório

O sistema deverá permitir visualizar as informações da análise de solo e os resultados da recomendação.

### RF16 — API

O sistema deverá disponibilizar operações de consulta, criação, alteração e exclusão por meio de uma API utilizando os métodos HTTP adequados:

* GET;
* POST;
* PUT;
* DELETE.

### RF17 — Auditoria

O sistema deverá registrar ações relevantes realizadas pelos usuários, permitindo identificar quem realizou determinada ação e quando ela ocorreu.

---

# 3. Requisitos Não Funcionais

### RNF01 — Segurança

O sistema deverá utilizar mecanismos de segurança adequados aos riscos identificados no projeto.

### RNF02 — Senhas

As senhas dos usuários não deverão ser armazenadas em texto puro. Deverá ser utilizado um mecanismo seguro de hash de senhas.

### RNF03 — Configurações sensíveis

Informações sensíveis, como chaves secretas e credenciais do banco de dados, não deverão ser armazenadas diretamente no código-fonte.

### RNF04 — Validação

Os dados fornecidos pelos usuários deverão ser validados antes de serem processados ou armazenados.

### RNF05 — Banco de dados

O sistema deverá utilizar um banco de dados relacional adequado às necessidades do projeto.

### RNF06 — Controle de privilégios

O sistema deverá utilizar o princípio do menor privilégio, concedendo aos usuários somente as permissões necessárias para realizar suas funções.

### RNF07 — Responsividade

A interface deverá funcionar adequadamente em diferentes tamanhos de tela.

### RNF08 — Usabilidade

A interface deverá ser organizada, intuitiva e apresentar mensagens de feedback ao usuário.

### RNF09 — Disponibilidade e recuperação

O projeto deverá possuir mecanismos de backup e recuperação dos dados.

### RNF10 — Manutenibilidade

O código deverá ser organizado em componentes com responsabilidades bem definidas, facilitando sua manutenção e evolução.

### RNF11 — Auditoria

O sistema deverá manter registros das ações relevantes realizadas pelos usuários para auxiliar no monitoramento e na segurança da aplicação.

---

# 4. Observação sobre os cálculos

As fórmulas utilizadas para os cálculos de calagem e adubação deverão seguir a metodologia definida pelo projeto e/ou pelos materiais fornecidos pelos professores.

As fórmulas, variáveis utilizadas e exemplos de cálculo serão documentados posteriormente no arquivo `docs/calculos.md`.
