Link do aplikacji na aws: http://rogalskiawsapp.eu-central-1.elasticbeanstalk.com/ <br/>
Na konsole latwiej wejsc tedy: https://eu-central-1.console.aws.amazon.com/elasticbeanstalk/home?region=eu-central-1#/welcome

Użyto następujących serwisów
=============================
- AWS 
- travis.ci
- github (github actions)
- dockerhub

Deployment (5-8minutes):
=============================
 travis.ci -> travis.yml <br/>
 github actions -> .github/workflows/rogalski.yml
 
Step by step
=============================

Zrob folder .github/workflows <br/>
Zaloz konto na https://www.travis-ci.com/ <br/>
Zaloz konto no aws, studencki trial <br/>
Zaloz elastic beanstalk na aws <br/>
Zrob usera przez IAM na aws, tworzac go zapisz tokeny <br/>
Dodaj secrety na konkrentym repozytorium w travisie <br/>
Dodaj secrety na konkretnym repozytorium w githubie <br/>
Zrob plik .travis.yml, skonfiguruj go jak tutaj (wazne nazwy z awsa, i zmiana brancha master na main) <br/>
Dodaj tam plik .yml, skonfiguruj go jak tutaj (wazne nazwy z awsa, i zmiana brancha master na main) <br/>

commit, push i samo powinno sie w obu odpalic, ale jedno sie wywroci, bo nie moga isc dwa deploymenty na raz, wiec trzeba bedzie recznie rerun travisa albo github action <br/>




Results
==============
<img width="1097" alt="image" src="https://user-images.githubusercontent.com/41301282/170297299-0782e906-1261-4d6a-a3c4-8686ef72bd17.png">

![image](https://user-images.githubusercontent.com/41301282/170295677-1ee4490d-78d2-41f1-bbd7-80ce60668c48.png)

<img width="1409" alt="image" src="https://user-images.githubusercontent.com/41301282/170297553-a377025a-519c-4bdd-9dc7-4632b4960818.png">

<img width="1349" alt="image" src="https://user-images.githubusercontent.com/41301282/170308827-c936b86f-57a4-445f-ae0d-f40421409d55.png">

![image](https://user-images.githubusercontent.com/41301282/170308643-b4a21271-3ffc-4766-9a3c-fb0aef880f36.png)

CZĘŚĆ DODATKOWA
===============

GitHub Ations ma zbudować obraz aplikacji i przesłać go na repozytorium DockerHub.
===================
Dodano standardowe, znane juz linie w pliku yaml oraz skonfigurowano secret keys w settingach <br/>
![image](https://user-images.githubusercontent.com/41301282/170437827-b0a92641-8190-4cfd-bda7-0fc8c5316051.png)

![image](https://user-images.githubusercontent.com/41301282/170442247-521f64ea-a6d0-4f58-a53b-03e0839d4b4c.png)
