How To:

1) attivare il Virtual Environment con il seguente comando:
	$ source venv/bin/activate		(dove 'venv' è il nome del VE che ho creato)

2) registrare la Environmental Variable di Flask con il seguente comando:
	$ export FLASK_APP=microblog.py

3) $ flask run

4) attivare il Debugger:
	$ export FLASK_DEBUG=1

5) settare un server SMTP su localhost per debuggare la ricezione di mail:
	https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-vii-error-handling





Remember:

- installare l'estensione "flask-wtf" con il seguente comando:
	$ pip install flask-wtf
  come spiegato qui: https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-iii-web-forms

- installare l'estensione "flask-sqlalchemy" con il seguente comando:
	$ pip install flask-sqlalchemy

- installare l'estensione "flask-migrate" con il seguente comando:
	$ pip install flask-migrate

- DB.1 - creare la "migration repository" per poter migrare facilmente il db nel momento in cui qualche modifica viene effettuata (e.g. aggiunta campo), con il seguente comando:
	$ flask db init

- DB.2 - creare gli script per la migrazione, con il seguente comando:
	$ flask db migrate -m "users table"	(la parte '-m ..' è un commento opzionale)

- DB.2 - migrare a tutti gli effetti, con il seguente comando:
	$ flask db upgrade (o downgrade in caso si voglia tornare ad una versione precedente)

- installare l'estensione "flask-login" con il seguente comando:
	$ pip install flask-login

- installare l'estensione "flask-mail" con il seguente comando:
	$ pip install flask-mail

- installare l'estensione "pyjwt" con il seguente comando:
	$ pip install pyjwt