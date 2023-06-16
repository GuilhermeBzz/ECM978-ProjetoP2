# Projeto de ECM978-Banco de Dados não Convencionais - Relacionamento entre Usuários do Twitter

### Integrantes
<pre>
Nome                               RA
André Monteiro Sanches Garcia    - 19.01230-6
Arthur Castanheda Sarnadas       - 19.00756-6
Giovanni Brandini Blanco Benuthe - 19.00043-0
Guilherme Bernardelli Zeigler    - 19.02453-3
</pre>

## Nosso Dataset
([Link do dataset](https://www.kaggle.com/datasets/hwassner/TwitterFriends))
No nosso dataset, dentre os dados de cada nó, temos um campo que contém a lista de contas que um usuário segue.  
Pensamos em 2 casos para analisar:  

### Primeiro caso:  
Considerando essa lista como a conexão de primeiro grau  (amigos). Sendo assim, o segundo grau seria outro usuário que compartilhasse contas seguidas com com o primeiro (amigo do amigo).  
<pre>
Usuario1 ---1o grau---> ContaA <---2o grau--- Usuario2>   
</pre>
  
### No segundo caso:
Consideramos esse campo de lista como ligação entre dois usuários, sendo assim, dois usuários que compartilhasse contas seguidas seriam amigos. E o amigo do amigo, seria um terceiro usuário que   compartilhasse contas seguidas com o segundo usuário.  
<pre>
Usuario 1 -----> ContaA <----- Usuario 2 -----> ContaB <----- Usuario 3  
   |-------------1o grau----------|-------------2o grau-----------|
</pre>
