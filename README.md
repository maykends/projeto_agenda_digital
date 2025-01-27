## Projeto de Clinica que possui uma função de Agendamento interno

No que consite este projeto:
- Administrar medicos e especialidade e agendas
- Criar uma agenda para disponibilizar as consultas para usuários comuns
- Permitir o usuario escolher um consulta em dia e horario de acordo com agenda do medico.

## Configurando o ambiente para executar a aplicação web.
Faça o download deste repositorio:

```
$ git clone https://github.com/maykends/projeto_agenda_digital
```

Crie um maquina virtual e instale a bibliotecas disponiveis no 
arquivo requirementes.txt:

Entre na pasta criada e inicie um ambiente virtual:
```
$ cd projeto_agenda_digital
$ python -m venv venv
```
Depois voce deve ativa-lo com o seguinte comando:

```
$ .\venv\Scripts\Activate
```

Verificar e instalar setuptools:
```
pip install --upgrade setuptools
```

Apos ativado, instale as bibliotecas necessárias para executar o projeto:
```
 (venv)$ pip install -r requirements.txt
```
Para poder ter o primeiro acesso e pode configurar o aplicação vamos executar o comando 
'migrate' para gerar o banco de dados padrão do Django(SQLite). E depois criar o superusuario:
```
(venv)$ python manage.py migrate
(venv)$ python manage.py createsuperuser
Apelido/Usuário: admin
E-mail: admin@mail.com
Password: 
Password (again):
```

Para iniciar o servidor depois deste passo você deve:
```
(venv)$ python manage.py runserver
```


Para visualizar se tudo esta executando como esperado vamos acessar o seguinte endereço:
[http://localhost:8000/](http://localhost:8000/)

Ou você pode ter acesso a admin do Django:
[http://localhost:8000/admin](http://localhost:8000/admin)

