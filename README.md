# django-tutorial
  Esta aplicação segue o projeto de enquetes fornecido na documentação do django, 
contendo uma página pública que consistirá em:
* Ver enquetes e votar nelas.
* Parte administrativa que permite adicionar, alterar e deletar enquetes.

Obs: os comandos fornecidos são para ambientes windows.

Para executar o projeto:
1. Clone o repositorion com o comando `git clone https://github.com/ruben-sa-brito/django-tutorial.git` ou então baixe o projeto como zip.
   
2. Crie um ambiente virtual com `python -m venv venv`, e ative ele rodando ` venv\scripts\activate.bat`.
   
3. Com o ambiente virtual ativo instale o django com `pip install django`.
   
4. Para que a aplicação funcione precisamos criar as tabelas necessárias no banco de dados, o django pode realizar as migrações,
para isso digite no terminal: `python manage.py migrate` esse comando realizará as operações de banco de dados contidas nos arquivos de migração,
com isso nossa aplicação ja deve estar funcionando, rode no terminar o comando `python manage.py runserver`, no navegador acesse a url: <http://127.0.0.1:8000/polls/>
voce deverá ver "No polls are available." porque ainda nao cadastramos nenhuma enquete.

5. Poderemos cadastrar novas enquetes na area administrativa do django, para acessá-la vamos criar um superuser, para isso rode `python manage.py createsuperuser`, e entao acesse <http://127.0.0.1:8000/admin/>, forneça as credenciais criadas anteriormente e terá acesso a área administrativa e poderá criar novas enquetes.
   
6. Na área administrativa acesse questions em polls, preencha os campos "Question text", "Date information", e o campo "Choice text" com pelo menos duas opçoes de votos, com isso ja podemos acessar novamente <http://127.0.0.1:8000/polls/> com a enquete para votação disponível.
