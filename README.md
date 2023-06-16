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
[Link do dataset](https://www.kaggle.com/datasets/hwassner/TwitterFriends)  
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

## O Projeto  
### Exibição dos nós 
![Image 071](https://github.com/GuilhermeBzz/ECM978-ProjetoP2/assets/79452551/b39ab71b-4d25-4344-9317-713bdbe5ee22)

### Exibição de recomendação a partir de um usuário (Utilizando segundo caso)
![Image 072](https://github.com/GuilhermeBzz/ECM978-ProjetoP2/assets/79452551/5837ef81-cd54-47ec-91f5-cdd058a31e41)

### Exibição da recomendação e da força do relacionamento (Utilizando primeiro caso)
![Image 073](https://github.com/GuilhermeBzz/ECM978-ProjetoP2/assets/79452551/96058a9d-d510-4ca9-8891-ce9f63fa45fa)

### Exibição da lista de recomendações (Utilizando o segundo caso)
![Image 074](https://github.com/GuilhermeBzz/ECM978-ProjetoP2/assets/79452551/6d147959-6740-489d-a92f-8f9548b58dc1)

### Exibição os nós (Utilizando um número maior de dados)
![Image 075](https://github.com/GuilhermeBzz/ECM978-ProjetoP2/assets/79452551/e31749b7-3905-4c47-b3ef-e3f4b2a69822)
No geral, não utilizamos esse número de dados pois causava muita lentidão para executar qualquer comando.


