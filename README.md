Aplikacja Dydaktyczna wyświetlająca imię i wiadomość w różnych formatach dla zajęć o Continuous Integration, Continuous Delivery i Continuous Deployment.

W projekcie wykorzystamy virtual environment, dla utworzenia hermetycznego środowisko dla aplikacji:

# tworzymy hermetyczne środowisko dla bibliotek aplikacji:
python3 -m venv .venv

# aktywowanie hermetycznego środowiska
source .venv/bin/activate
pip install -r requirements.txt
pip install -r test_requirements.txt

# zobacz
pip list
Sprawdź: tutorial venv oraz biblioteki flask.

Uruchamianie applikacji:

# jako zwykły program
python main.py

# albo mozemy uruchomic w taki sposob:
PYTHONPATH=. FLASK_APP=hello_world flask run
# w przegladarce lub za pomoca curl
curl 127.0.0.1:5000/
Uruchamianie testów (see: http://doc.pytest.org/en/latest/capture.html):

PYTHONPATH=. py.test
PYTHONPATH=. py.test --verbose -s
Przydatne komendy:

Deaktywacja srodowiska wirtualego

 # deaktywacja
 deactivate
Aktywacja, jeśli wracamy do projektu gdzie jest już środowisko wirtalne

# spradzenie czy widzimy katalog (.venv)
# gdzie jest wirtualne srodowisko
ls -a

# aktywacja 
source .venv/bin/activate
Miejsce na twoje notatki:

# miejsce na twoje notatki
