
# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 

## 1. Introdução

***1.1.  klitCode***

 Vinicius Enrique Pinheiro Itakura https://github.com/ViniciusItakura
 <br/>Gustavo Eugênio Tertuliano Ferreira https://github.com/gusteugenio
 <br/>Leonardo David dos Santos https://github.com/LeonardoDavidSantos
 <br/>Bruno Oliveira de Campos https://github.com/0l1mpus
 <br/>Victor Hugo dos Santos Messias https://github.com/victorhsmessias

***1.2.  klitAgenda***

***1.3.  Propósito do Sistema***

Nosso sistema oferece uma plataforma completa para o gerenciamento eficiente de reservas em uma empresa. Com uma inteface intuitiva e funcionalidades poderosas, o klitAgenda simplifica o processo de agendamento, permitindo que você utilize o uso de recursos e aumente a produtividade da equipe.

***1.2.  Público Alvo***

Este documento se destina a empresas e clientes que buscam facilitar e simplificar o processo de agendamento, permitindo que você utilize os recursos e aumente sua produtividade.
<br/><br/>
***1.3. Descrição dos usuários***
<br/><br/>
O software foi projetado para empresas, onde há necessidade de controle de saída e entrada de veículos empresariais. Os Perfis dos nossos usuários são funcionários de empresas responsáveis pelo agendamento ou realização de visitas ao cliente. Entre os usuários que fazem a condução do veículo para realizar a visita, 90% deles são homens e somente 10% são mulheres, sendo eles maiores de 18 anos. Já entre os que fazem o agendamento, mais de 90% dos usuários são mulheres, com a mesma faixa etária. A frequência do software pelos usuários é de 5 dias por semana. Com relação aos cargos de cada um, os usuários que agendam a visita são pessoas em cargos administrativos e os que fazem a condução são aqueles em cargos nos quais é necessário visitar os clientes para determinadas demandas.


Planilha dos perfis de usuários:</br>
![planilha-klitcode](https://github.com/Aula-Requisitos/requisitos-software/assets/137667932/aad3c057-559e-4ad6-8521-7206f113b387)
<br/>
Personas: 
![image](https://github.com/Aula-Requisitos/requisitos-software/assets/136620727/1d1a3926-91b9-4b0b-b905-1082f5a9d67a)
<br/>
![image](https://github.com/Aula-Requisitos/requisitos-software/assets/136620727/f18854aa-a14c-4ba3-bad4-c9bac70f9d21)
<br/>
![image](https://github.com/Aula-Requisitos/requisitos-software/assets/136620727/7355b47d-4624-4853-9a80-3ceaea217e1d)
<br/>



Cenário atual:
  Vinicius Eugênio é corretor de imobiliária e atualmente sua equipe realiza os cadastros de agendamento manualmente no whatsapp o que possibilita erros humanos como criar reservas no mesmo período de outra reserva, fazendo com que ocorra desorganização pela quantidade de reservas.
Frequentemente seus funcionários agendam visitas para um funcionário em horários que o carro já está sendo utilizado, o que resulta em faltas na visita aos clientes e gera insatisfação.
  

Cenário depois da implantação:
  A klitCode percebe o problema e desenvolve um sistema que gerenciará todas as reservas, administrando as regras de negócio, evitando duplicidade de agendamentos e enviando notificação ao funcionário para o mesmo ser avisado ao criar a visita. Isso resulta na dimunuição de faltas a visitas a clientes e melhor satisfação dos clientes da imobiliária.

## 2. Documentos gerais no repositório

***2.1. Requisitos de usuário***

[*<Link para a pasta com os requisitos de usuário.>*](https://padlet.com/viniciusitakura/kanban-ujjcsnad60lsswef)

***2.2. Requisitos de sistema***

[*<Link para a pasta de requisitos de sistema .>*](https://padlet.com/viniciusitakura/kanban-ujjcsnad60lsswef)

***2.3. Protótipos***

[*<Link para a pasta com os protótipos.>*](https://www.figma.com/file/wYNr0KqXAKncGABYOl7htl/Untitled?type=design&mode=design&t=2EY4E2F8Cz4LL0in-0)

### Requisitos Funcionais (RF)

| RF   | Descrição                                                                                      |
| ---- | ---------------------------------------------------------------------------------------------- |
| RF01 | O sistema deve controlar o acesso de usuários não administradores às funcionalidades de adicionar usuário e veículo. |
| RF02 | O sistema deve permitir ao usuário cadastrar reservas, incluindo informações como usuário, data, hora, veículo e observações. |
| RF03 | O sistema deve permitir ao usuário visualizar todas as reservas disponíveis com filtro de usuário e data. |
| RF04 | O sistema deve possuir um sistema de calendário para facilitar a inclusão das datas. |
| RF05 | O sistema deve possuir um sistema de login com possibilidade de recuperação de senha. |
| RF06 | O sistema deve realizar uma verificação a cada 5 minutos para verificar se possui alguma reserva vencida. |
| RF07 | O sistema deve possuir uma verificação para impedir a criação de reservas com a mesma data e mesmo veículo. |
| RF08 | O sistema deve verificar se o horário de término não é menor que o horário de início para criar uma nova reserva. |
| RF09 | O sistema deve exibir apenas as reservas da empresa do usuário. |
| RF10 | O sistema deve verificar se não existe uma reserva vencida a cada troca de menu. |

### História do usuário RF

| RF   | Descrição                                                                                      |
| ---- | ---------------------------------------------------------------------------------------------- |
| RF01 | Como dono de imobiliária quero um sistema que controle o acesso de usuários, para poder possuir administradores e usuários comuns. |
| RF02 | Como dono de imobiliária quero um sistema que permita ao usuário cadastrar reservas, incluindo informações como usuário, data, hora, veículo e observações, para poder ter um melhor controle. |
| RF03 | Como dono de imobiliária quero um sistema que permita ao usuário visualizar todas as reservas disponíveis com filtro de usuário e data, para ser de fácil acesso à meus colaboradores. |
| RF04 | Como dono de imobiliária quero um sistema que possua um sistema de calendário para facilitar a inclusão das datas, para agilizar mais ainda os cadastros. |
| RF05 | Como dono de imobiliária quero um sistema que possua login com possibilidade de recuperação de senha, para facilitar a identificação de quem editou a agenda. |
| RF06 | Como dono de imobiliária quero um sistema que realiza uma verificação a cada 5 minutos para verificar se possui alguma reserva vencida, para evitar poluição visual na tela. |
| RF07 | Como dono de imobiliária quero um sistema que possua uma verificação para impedir a criação de reservas com a mesma data e mesmo veículo, para evitar duplicidade. |
| RF08 | O sistema deve verificar se o horário de término não é menor que o horário de início para criar uma nova reserva. |
| RF09 | O sistema deve exibir apenas as reservas da empresa do usuário. |
| RF10 | O sistema deve verificar se não existe uma reserva vencida a cada troca de menu. |

### Restrições Não Funcionais (RN)

| RN   | Descrição                                                                                      |
| ---- | ---------------------------------------------------------------------------------------------- |
| RN01 | O sistema possui um sistema de notificação ao WhatsApp do cliente ao criar uma reserva. |
| RN02 | O sistema possui um sistema de notificação via e-mail do cliente ao criar uma reserva. |
| RN03 | O sistema é rápido. |
| RN04 | O sistema possui certificado de criptografia SSL. |
| RN05 | O sistema possui uma interface clean com coloração roxa. |
| RN06 | O sistema é responsivo. |
| RN07 | O sistema possui acessibilidade. |
| RN08 | O sistema é em Single Page Application. |
| RN09 | O sistema é em linguagem JavaScript com React. |
| RN10 | O backend é implementado com o Firebase. |

## Entrevista



## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*
    
[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.





