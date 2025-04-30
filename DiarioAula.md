# AulaAPS-AnaliseDesenvolvimentodeProjeto
Diario de Aula de APS

11/03/2025
**Aula Inaugural** 

O professor passou a estrutura disciplinar referente ao curso e as responsabilidades a serem cumpridas pelos alunos.
logo em seguida, o professor iniciou a explicação de como sera realizado a avaliação do seu conteudo e tambem, passou algumas questões para nós refletirmos.
o metodo escolhido pelo professor, foi o de avaliar os alunos de maneira continua, com atividades semanais, para ajudar no desenvolvimento de cada aluno, e tambem para uma melhor absosrção de conteudo. 

****
25/03/2025
**Aula 03**
Preço: Dev
O professor iniciou a aula orientando sobre o sabádo letivo, e fazendo uma retomada no assunto da 2ºaula 
"SDLC, modelos cascata, incremental, espiral, complementar, metodologias/processos auxiliares"
"Metodologias ageis - 4 valores, cliente, equipe, processo, software"
"motivos para estudar os antigos modelos de SDLC"
"Qual era a % de acerto no desenvolvimento de software"
e a reflexão sobre a frase "Baixar o preço resolve?"

Na sequancia começamos a falar do lavantamento de requisitos e sua importancia! "conhecer certo, analiasr certo e descrever certo" padrões e tecnicas.
Stakeholders.
tecnicas de lavantamentos de dados para entender o mercado,"Dor do cliente, requisitos exixtentes e inexixtentes nos concorrentes.", analise documental, prototipagem, questionarios.
permissões, cuidados com a comunicação, visão inviesada.
*Engenharia de Requisitos:  conceitos, termologia, fundamentos e importancia.
processos de extração, analise, validação e gerenciamento.

e finalizou informando a pesquisa para o desenvolvimento de um sistema de emprestimos, com a entrevista com o o "cliente".


****

22/04/2025

**Aula 06**

o professor, esta ensinando a fazer o diagrama de caso de uso.

@startuml
'https://plantuml.com/sequence-diagram'

left to right direction

actor cli as "cliente"
actor adm as "administrador"
actor lim as "limpeza"
actor man as "manutencao"

rectangle "Sistema reserva de quadra"{
  usecase "consultar calendario" as cu01
  usecase "buscar reserva" as cu02
  usecase "realizar reserva" as cu03
  usecase "verificar disponibilidade" as cu04
  usecase "cancelar reserva" as cu05
  usecase "gerenciar todas as reservas" as cu06
  usecase "cadastrar quadra" as cu07
  usecase "status reserva" as cu08 
  usecase "Gerenciar limpeza" as cu09
  usecase "status limpeza" as cu10


  cu03 .> cu04 : <<include>>
  cu05 <. cu02 : <<extends>>
}

cli --> cu01
cli --> cu02
cli --> cu03
cli --> cu04
cli --> cu05

adm --|> cli
adm --|> lim
adm --|> man
adm --> cu06
adm --> cu07

lim --> cu01
lim --> cu09
lim --> cu10

man --> cu01
man --> cu04
@enduml

****
Aula 29/04/2025

Nesta Aula nos demos sequancia no projeto e colocamos em pratica o conceito para levantamento e documentação dos requisitos para que 
quando nós programadores colocarmos em produção, possamos executar de forma direta e completa. 

