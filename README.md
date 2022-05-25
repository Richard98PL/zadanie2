Link do aplikacji na aws: http://rogalskiawsapp.eu-central-1.elasticbeanstalk.com/
Na konsole latwiej wejsc tedy: https://eu-central-1.console.aws.amazon.com/elasticbeanstalk/home?region=eu-central-1#/welcome

Użyto następujących serwisów
- AWS
- travis.ci
- github (github actions)

Deployment:
 travis.ci -> travis.yml
 github actions -> .github/workflows/rogalski.yml
 
Step by step

Zrob folder .github/workflows
Zaloz konto na https://www.travis-ci.com/
Zaloz konto no aws, studencki trial
Zaloz elastic beanstalk na aws
Zrob usera przez IAM na aws, tworzac go zapisz tokeny
Dodaj secrety na konkrentym repozytorium w travisie
Dodaj secrety na konkretnym repozytorium w githubie
Zrob plik .travis.yml, skonfiguruj go jak tutaj (wazne nazwy z awsa, i zmiana brancha master na main)
Dodaj tam plik .yml, skonfiguruj go jak tutaj (wazne nazwy z awsa, i zmiana brancha master na main)

commit, push i samo powinno sie w obu odpalic, ale jedno sie wywroci, bo nie moga isc dwa deploymenty na raz, wiec trzeba bedzie recznie rerun travisa albo github action




Results
<img width="1097" alt="image" src="https://user-images.githubusercontent.com/41301282/170297299-0782e906-1261-4d6a-a3c4-8686ef72bd17.png">

![image](https://user-images.githubusercontent.com/41301282/170295677-1ee4490d-78d2-41f1-bbd7-80ce60668c48.png)

<img width="1409" alt="image" src="https://user-images.githubusercontent.com/41301282/170297553-a377025a-519c-4bdd-9dc7-4632b4960818.png">

