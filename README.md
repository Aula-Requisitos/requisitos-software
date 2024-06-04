
# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 
Link do site: https://klitagenda.klitcode.com/

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
<br/>*<Link para a pasta com os protótipos de baixa fidelidade.>* https://ninjamock.com/Designer/Workplace/195325781



### 3. Requisitos

***3.1. Requisitos Funcionais (RF)***

| RF   | Descrição                                                                                      | Prioridade |
| ---- | ---------------------------------------------------------------------------------------------- | ----- |
| RF01 | O sistema deve controlar o acesso de usuários não administradores às funcionalidades de adicionar usuário e veículo.| Médio |
| RF02 | O sistema deve permitir ao usuário cadastrar reservas, incluindo informações como usuário, data, hora, veículo e observações. | Alto |
| RF03 | O sistema deve permitir ao usuário visualizar todas as reservas disponíveis com filtro de usuário e data. | Alto |
| RF04 | O sistema deve possuir um sistema de calendário para facilitar a inclusão das datas. | Baixo |
| RF05 | O sistema deve possuir um sistema de login com possibilidade de recuperação de senha. | Médio |
| RF06 | O sistema deve realizar uma verificação a cada 5 minutos para verificar se possui alguma reserva vencida. | Baixo |
| RF07 | O sistema deve possuir uma verificação para impedir a criação de reservas com a mesma data e mesmo veículo. | Alto |
| RF08 | O sistema deve verificar se o horário de término não é menor que o horário de início para criar uma nova reserva. | Alto |
| RF09 | O sistema deve exibir apenas as reservas da empresa do usuário. | Alto |
| RF10 | O sistema deve verificar se não existe uma reserva vencida a cada troca de menu. | Baixo |

***3.2. Requisitos Não Funcionais (RN)***

| RN   | Descrição                                                                                      |  Prioridade |
| ---- | ---------------------------------------------------------------------------------------------- | ----- |
| RN01 | O sistema possui um sistema de notificação ao WhatsApp do cliente ao criar uma reserva. | Baixo |
| RN02 | O sistema possui um sistema de notificação via e-mail do cliente ao criar uma reserva. | Baixo |
| RN03 | O sistema deve responder em 2 segundos. | Médio |
| RN04 | O sistema possui certificado de criptografia SSL. | Médio |
| RN05 | O sistema possui uma interface clean com coloração roxa. | Baixo |
| RN06 | O sistema é responsivo. | Alto |
| RN07 | O sistema possui acessibilidade. | Alto |
| RN08 | O sistema é em Single Page Application. | Alto |
| RN09 | O sistema é em linguagem JavaScript com React. | Baixo |
| RN10 | O backend é implementado com o Firebase. | Baixo |	

### 4. História do usuário (RF)

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

## Entrevista

1.  **Como é feito o agendamento de visitas atualmente?**
	R: Atualmente nós realizamos por meio de um grupo de whatsapp.
	
2. **Quais os tipos de usuários?**
	R: Seria dois tipos, administrador e corretor.

3. **Qual a média de usuários vocês precisam usar?**
	R: No nosso caso, precisariamos de uma média de 7 usuários, seriam 5 corretores e 2 administradores.
	
4. **Quais os principais problemas que vocês enfrentam hoje?**
	R: Hoje enfrentamos duplicidade no agendamento, falta de organização e falta de comunicação

5. **Vocês acreditam que um aplicativo irá te ajudar? Se sim, quais as principais funcionalidades necessárias?**
	R: Sim, pois no aplicativo deverá ter um sistema de notificação para o corretor responsável, melhor 		   										organização com uma tabela de agendamentos marcados, sistema de verficação de duplicidade e sistema para adicionar veículos e usuários.

6. **Em quais plataformas vocês desejam utilizar o sistema?**
	R: Gostaria de utilizar no celular e para o computador.

7. **Como vocês lidam com cancelamentos e remarcações de agendamentos atualmente?**
	R: Hoje em dia, só enviamos as informações no grupo de whatsapp.

8. **Como vocês lidam com situações de esquecimento dos agendamentos?**
	R: Normalmente é uma dor de cabeça, pois o cliente fica irritado, o que consequentemente resulta na perca da locação.

9. **Qual a média de visitas diárias?**
	R: Geralmente são 20 visitas.
 
10. **Em qual grau (baixo, médio ou alto) a falta de um sistema de agendamento afeta a empresa atualmente?**
	R: Médio, porque não impossibilita o agendamento da visita, mas tem vários problemas de organização, com a duplicidade e os esquecimentos.



## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*
    
[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.





