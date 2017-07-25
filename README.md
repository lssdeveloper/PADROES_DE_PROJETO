# PADROES_DE_PROJETO
Estudo sobre padrões de projetos

Semana 1 - Padrão Observer 

Definição:

O padrão observer define a dependência um-para-muito entre os objetos para que quando um objeto mude de estado todos os seus dependentes sejam avisados e atualizados automaticamente

editora + assinantes = padrão observer
carro de polícia + carro roubado = padrão observer

Quando os dados no Subject mudam os observadores são avisados.
Os observadores assinaram (registraram-se) no Subject para receber atualizações quando os dados de Subject são alterados.

Novos valores de dados são comunicados para os observadores de alguma forma quando são alterados.

Objeto Subject = Objeto que contém o estado  (O sujeito)
Objetos Observadores = Objetos dependentes (dependendo do tipo de notificação, o observador também pode ser atualizado com os novos valores.

Qdo o estado de um objeto é alterado, todos os seus dependentes são notificados.

Para implementarmos o design de classe incluimos interfaces Subject e Observer

Principios de projeto:
Busque designs levemente ligados entre objetos que interagem.

O Padrão Observer fornece um design de objeto onde os sujeitos e os observadores são levemente ligados.

Por que?
-O que o sujeito sabe sobre um observador é que ele implementa uma certa interface.
-podemos adicionar novos observadores a qualquer momento
-não precisamos modificar o sujeito para adicionar novos tipos de observadores
-podemos reutilizar sujeitos ou observadores independentes uns dos outros
-alterações no sujeito ou num observador não irá afetar o outro.

A vantagem é o descoplamento ou seja a depêndencia de um objeto com o outro.

Pontos importante:
Princípio OO
    -Encapsule o que varia
    -Dê prioridade à composição em relação à herançaa
    -Programe par Interface, não para implementação
    -Busque projetos levemente lilgados entre objetos que interagem.
    -Projetos levemente acoplados são muito mais flexíveis e fáceis de modificar
    -OS Subjects (Sujeitos), ou como são conhecidos, Observables, atualizam os observadores usando uma interface comum.
    -Os Observers são levemente ligados, já que o sujeito não sabe nada entre eles a não ser que implementam a Interface Observadores.
    -É possível empurrar ou puxar dados de Observablr ao utilizar o padrão("puxar é considerado mais "correto")
    -Não dependa de uma ordem ou notificação específica para seus Observers.


   


