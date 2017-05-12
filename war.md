# Narzędzia programisty Python

Długość: 1 godzina. Głównie rozmowy i małej ilości demonstracji, bez slajdów. Celem jest wymiana doświadczeń i opinii nt. narzędzi, których używaja zawodowi _pythonowcy_.

## Wstęp. 

Przybiorę formę gry z rolami. Załóżmy, że pracujemy razem w normalnym zespole programistycznym gdzie główną technologią jest Python, ja jestem odpowiedzialny za produktywność, a Ty od nie dawna jesteś w zespole. Razem będziemy _dowozić_ nowe funkcje, sprinty, wgrywać kod na serwery produkcyjna, gasić pożary i naprawiać błędy w kodzie. Każdej stronie zależy, żeby nie marnować czasu, żeby było go jak najwięcej na piłkarzyki i myślenie, nie chcemy wykonywac dodatkowej pracy tylko dlatego, że nie znamy krótszej drogi. 

Nic co zaproponuję nie jest prawdą, a jedynie opinią. Moje rekomendacje można obalić, a proponowanej logice zaprzeczyć, ale zgódźmy się co nadrzędnej zasady. *Narzędzia się liczą.* _Tools Matter_. I co do drugiej pomocniczej, nie ma dobrego powodu, żeby znać narzędzie słabo, troszkę i mniej więcej. Spędzimy z nimi tysiące godzin i lata, warto już od samego początku dążyć do aktywnego poznawania ich i mistrzostwa. Tak, mistrzostwa. Wybierz dobre narzędzia i znaj każdą ich moc. Sprawdź to, stań się mistrzem swoich narzędzi, jak się nie opłąci, zwrócę Ci pieniądze. 

Przerywaj mi, sugeruj własne, kontruj, pytaj i męcz. Z chęcią się dowiem czegoś nowego.

## O wyborze narzędzi ogólnie. 

Wybierz narzędzie sam, ale spośród tego co znają ludzie, z którymi pracujesz, zawodowo czy hobbistycznie. Wymieniaj się wiedzą, pokazuj co odkryłeś sam i pytaj o triki innych. Nie bądź tym jednym emacsem na całym _openspejsie_ (chyba, że już jesteś jego mistrzem). 

Jeżeli cała Twoja drużyna korzysta z foo, a Ty od zawsze korzystasz z bar, ale jakoś specjalnie Ci nie zależy, to spróbuj się dostosować. Nie mocno, nie na siłę, nie ze stratą w produktywności ale rozważ. Ja uwielbiam narzędzia i nie raz byłem fanatykiem własnych, chciałem przekonywać do moich ścieżek i chyba traciłem na tym. Jak wszyscy wokół Ciebie korzystają z Ubuntu ale zostawiają Ci wolną rękę, to nie wybieraj Gentoo, a jak wszyscy wokół Ciebie korzystają z Gentoo to ucz się `portage`! Przyjdzie taki zły piątek, kiedy będziecie w sześć osób na Twoim dziwnym systemie naprawiali Twój błąd a Ty nie będziesz wiedzieć jak znaleźć paczkę która zawiera pliki `v4l-*-24xxx-01.fw` i Ci Jacek nie pomoże, a mógłby. 

Rób tak jak Twoja drużyna, no ale też bez przesady.   


## Wielkie tematy IDE/edytor tekstu

[IDE czy nie IDE?](https://youtu.be/VN3ak9HKvyM?t=29s). Czym jest IDE? Kiedy IDE? Kiedy nie IDE?

#### [PyCharm](https://www.jetbrains.com/pycharm/download/)
- nawigacja, do klasy, do pliku, do każdego _symbolu_, nawigacja po edycjach, nawigacja po nawigacji, po metodach
- refaktoring, wyciągnij/wciągnij kod, 
- znajdź użycia, także pod zmienioną postacią, znajdź implemetacje
- integracja z gitem, cofanie sekcji do stanu z repozytorium
- zmień nazwę symbolu
- czyszczenie kodu (code analysis)
- nadpisz metodę
- współpracuje z dockerem
- ukradli multikursor _sablajmowi_ i ulepszyli go
- szift+enter!
- repozytorium konfiguracji

minusy: 
- prędkość
- zeżre prawie wszystkie zasoby na średnim komputerze
- tak rozbudowany program my setki małych irytujących błędów, także w regresji
- poznanie całości zabierze miesiące, może lata, ale warto
- czasami kosztuje pieniądze
- debugger powolny, a konsola tragicznie zaimplementowana
- rozpieszcza tak, że niektórzy nigdy się gita nie nauczą
- _sablajmowcy_ będą przewracać oczami i pytać się kiedy się nawrócisz
- słabe, słabe, słabe pluginy

co na początek:
- Help -> Keymap reference
- Menu Navigate
- Menu Refactor

#### SublimeText/[Anaconda](https://github.com/DamnWidget/anaconda), 

- szybkość
- multikursor
- _Goto Anything_,
- konfiguracja w plikach, Customize Anything
- pluginy, szybkośc instalacji pluginów
- nie ma za dużo cudów, więc da się go nauczyć i zająć się pracą

minusy:
- [abandonware](https://en.wikipedia.org/wiki/Abandonware) [ostatnia wersja "23 September 2016", 4 wersje w 2016]
- przenoszenie konfiguracji to ból w życi, chyba, że coś się zmieniło

#### vim

na początek:
- :wq, dd, p, P, o, O, A, I, :%s, /cokolwiek, ciw, x, r, dw, d$
potem vimtutor, i może kolekcjonować pluginy od tych co się znają

#### [Visual Studio Code](http://donjayamanne.github.io/pythonVSCode/)

Rafał mówi, że bardzo dobre.

Wszystko inne... no jak kto woli, ale ja bym nie tracił czasu. 
Nie Atom, NIE gedit, NIE nano, 

Pogadajmy, co kto używa?

## Sysyem operacyjny

- Linux czy MacOS
- kiedy da się pracować pod Windowsem

## Hardware
- dlaczego i7

## System operacyjny jako narzędzie, terminal, bash/zsh

```
alias ag apt apt-get apt-file awk arp-scan
bash bg bzip2 bunzip2
cat cd chmod chown cp cron cal curl
date du df dd detox diff dmesg docker dpkg dos2unix
echo env exec export encfs egrep
find for free fg file
grep gzip git gpg gpg-agent groups
hash -r hg history htop hwinfo
ifconfig ifup ifdown if if info ipython
jobs
kill killall keepassx
less locate ll ls ln -s lowriter lsof lsusb
man make mv mc mbank-cli? meld mkdir mount
netstat
ping pip `ps aux` pass pwd py.test pyenv python3!
rsync reboot rm
scp sh sed sort source sleep ssh stat su sudo sync screen shutdown
touch tree type tar tmux top tr
uniq uname umount unzip `usermod -aG docker bartek`
vim vlc
which wget wc while whoami
xargs (wym zargs!)
```

## Debuggery, ipdb, pdb, pdbpp?, print('pupa'), śledzenie kodu, logging. 

## IPython, REPL na sterydach, Jupyter

- jest jeszcze [bpython](https://github.com/bpython/bpython)

## Virtualenv, pyenv, venv, docker, site-packages, virtualenvwrapper, instalacja pakietów

- najprosztszy setup.py, przejrzyj setup.py na githubie, 
- setuptools to piekło, [ma "osobnego" BDFLa-delegata](http://python-notes.curiousefficiency.org/en/latest/pep_ideas/core_packaging_api.html)

## dzwonki i gwizdki, może kiedyś użyjesz

line profiler, 
concurrency visualizer

## git, mercurial, svn

## github, gitlab, bitbucket

## ssh, tunele

## Alternatywne implementacje Pythona, 
- pypy, 
- anaconda, 
- [micropython](https://github.com/micropython/micropython)

cmentarz: ironpython, jython, [CL-Python](https://github.com/metawilm/cl-python), brython, srajton,

## Standardy kodu. 

pep8, pylint, pyflakes, flake8, mccabe

## testowanie 
- py.test, nosetests, std unittest, 
- [mock](https://docs.python.org/3/library/unittest.mock.html), 
- [freezegun](https://github.com/spulec/freezegun), BDD/cucumber/gherkin/?

---
na to nie starczy czasu:

## moje ulubione biblioteki
- pygments
- requests
- sqlalchemy
- django
- cookiecutter
- arrow/moment
- :| lxml, BeautifulSoup, xmltodict 

## Przykłady narzędzi *w Pythonie*. httpie, ansible, supervisor, mycli, pgcli, docker-compose, [sentry](http://sentry.io), [uWSGI](https://uwsgi-docs.readthedocs.io/)

## Grube koty
[NLTK](http://www.nltk.org/), [scipy](http://www.scipy.org/), [scikit-learn](http://scikit-learn.org/)

## Kradnięcie Internetu: Scrapy

## Linki: 
- https://github.com/vinta/awesome-python