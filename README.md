
<div>
 ![logo da exact](img/logo-exactsales.png)
</div>



# Cadência de e-mail
## Índice
1. [Aba Campanha](#aba_campanha)
    - [Criar Campanha](#criar_campanha)
    - [Buscar Campanha](#buscar_campanha)
    - [Editar Campanha](#editar_campanha)
    - [Finalizar Campanha](#finalizar_campanha)
    - [Excluir Campanha](#excluir_campanha)

2. [Aba Listas](#aba_lista)
    - [Detalhe da lista](#editar_campanha)

>## Aba Campanhas
![Aba campanha de e-mail](img/AbaCampanha.png)
>- Caso não exista nenhuma campanha o sistema vai abrir uma tela com uma imagem e a mensagem `Você ainda não possui nenhuma campanha` , logo abaixo da mensagem  um link que abrirá a Tela [Criar Campanha](#criar_campanha), onde será criada as campanhas.
>- Caso exista campanha cadastrada o sistema ira trazer todas as caompanhas registradas
>- Será permitido apenas duas campanhas configuradas caso o usuario tente confirgurar a terceira o sistema deve emitir a seguinte mensagem `Ja existe duas campanhas configuradas, ao menos uma deve estar finalizada`.
> - Caso o usuário necessite cadastrar uma terceira campanha, ao menos uma campanha das criadas anteriormente deverá se encontrar como `Finalizada`.


 ## Criar Campanha
> - Botão só irá aparecer habilitado caso não tenham 2 campanhas com os status `“Agendado”, “Rascunho” ou “Ativo”`, se houver 2 campanhas com esses status o botão vai aparecer desabilitado e com um tooltip com a mensagem `“Já existem duas campanhas configuradas”`.
>    - Botão salvar/ criar
>        - Vai salvar a campanha de acordo com as configurações feitas pelo usuário e redirecionar para a aba campanha.
>        - Se ao salvar a campanha e não tiver preenchido o campo “Nome da campanha”, vai apresentar feedback com a mensagem `”Precisamos de uma nome para salvar essa campanha”, colocando o foco no campo.`
>        - Se ao salvar a campanha não tiver uma “Lista de envio” configurada, vai apresentar feedback com a mensagem ”Precisamos de uma lista de envio para salvar essa campanha”, colocando o foco no campo.
>        - Se ao salvar a campanha não tiver configurado `“Conta de e-mail do remetente” ou “Limite de envio diário”` ou em alguma Etapa não tiver `“Data de início” ou “Template de e-mail” `definidos, vai apresentar um modal com a mensagem `“Nem todas as configurações foram definidas, a campanha será salva como rascunho. Deseja Salvar?”`, se ele concordar em salvar redirecionar para a Campanhas e apresentar feedback com mensagem “Campanha salva”.
>        - Se ao salvar todas as configurações estiverem corretas, vai redirecionar para aba Campanhas e apresentar feedback com mensagem “Campanha salva”.

## Buscar Campanha
> - Após digitar 3 caracteres vai procurar campanha(s) dentro da listagem que o nome contenham os caracteres digitados

## Editar Campanha
> - Se a campanha estiver “Agendada” ou  “Rascunho”, será permitido a edição.
> - Se a campanha estiver “Ativa” ou  “Finalizada”  será apresentada ícone desabilitado e um tooltip com a mensagem `”Campanhas em xxxx não poderão ser editadas”`, informando que não será possível editar a campanha.


## Finalizar Campanha
> - Só vai aparecer como habilitado caso a campanha estiver ativa. 
> - Se a campanha estiver `“Agendada”, “Rascunho” ou “Finalizada”` será apresentada ícone desabilitado e um tooltip com a mensagem ”Campanhas em xxxx não pode ser finalizadas”, informando que não será possível finalizar a campanha.	

## Excluir Campanha
> - Se a campanha estiver “Agendada”, “Rascunho” ou “Finalizada” será permitida a sua exclusão.
> - Se a campanha estiver “Ativa” vai apresentar ícone desabilitado e um tooltip com a mensagem `“Campanha Ativa não pode ser excluída”` , informando que não será possível excluir. 
> - Se houver falha ao excluir, informar o usuário com mensagem padrão.
> - A exclusão da campanha vai ser feita de forma logica


[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/SAWFvFhowW4/0.jpg)](https://www.youtube.com/watch?v=SAWFvFhowW4)
