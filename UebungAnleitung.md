# Übung Jenkins 
Nachdem der Level 10 Developer Marc sich über Continuous Integration / Delivery und Deployment informiert hat, will er nun verschiedene SCM-Tools ausprobieren. Nach einer mehrtägigen Recherche im Internet hat er sich folgende Tools ausgesucht:

- Jenkins
- GitLab
- Buddy
- Heroku

Leider verpflichtet Herr Endboss (Chef von Marc) Mark dazu, weitere Tickets im Projekt abzuarbeiten, weshalb er nicht die Zeit hat, sich die verschiedenen SCM-Tools anzuschauen. Allerdings kennt Mark eine Gruppe von Studenten, welche sich liebendgern neue SCM-Tools anschauen. 
Die Studenten haben sich bereit erklärt alle SCM-Tools zu testen. Dafür bilden die Studenten Zweiergruppen, welche wiederrum drei große Gruppen bilden. Einmal Gruppe Jenkins Gruppe Gitlab und Gruppe Heroku&Buddy.

## Aufgabe Gruppe Jenkins (CI)
Die Studenten sollen in Zweiergruppen eine Pipeline in Jenkins erstellen, welche folgende Schritte besitzt:
1. Build: Baut das Projekt 
2. Test: Führt die Tests aus
3. Deploy: führt ein Echo aus, da wir im Container sind 

Dafür sollen die Studenten folgende Schritte unternehmen:
1. Das GitHub-Repository "IWS-DEMO" forken (https://github.com/pdomscheid/IWS-Demo)
2. Jenkins mithilfe von Docker installieren (https://hub.docker.com/r/jenkins/jenkins/)
3. Das Setup fertigstellen
4. Eine Pipeline für das geforkte Repo erstellen, mit den oben genannten Schritten (Declarative Pipeline: https://jenkins.io/doc/book/pipeline/syntax/)
5. (Optional) Die Tests durch einen Test-Report in Jenkins visuell darstellen 
6. (Optional) Den Test-Report als Artifiact zusätzlich im Build hinterlegen


## Aufgabe Gruppe Heroku & Buddy (CI & CD)
Die Studenten sollen in Zweiergruppen eine Pipeline in Buddy erstellen und die Applikation mithilfe von Heroku deployen. Diese Aufgabe besteht wiederrum aus zwei Teilaufgaben

### Aufgaben Teilaufgabe 1
1. Das GitHub-Repository "ISW-DEMO" forken (https://github.com/pdomscheid/IWS-Demo)
2. Eine Pipeline für das geforkte Repo erstellen, welches aus drei Schritten besteht:
   1. Build: Baut das Projekt
   2. Test: Führt die Tests aus
   3. Deploy: Echo das die App deployed wurde
3. Optional (Archiviere das Test-Result)

### Aufgaben Teilaufgabe 2
1. Das GitHub-Repository "MSO-Backend" forken (https://github.com/pdomscheid/MSO-Backend)
2. Das Node-projekt mithilfe von Heroku deployen (https://heroku.com)
3. Eine Pipeline für das geforkte Repo mithilfe von Buddy erstellen, welche aus zwei Schritten besteht:
   1. Build: Baut das Projekt
   2. Deploy: Deployed die Applikation zu Heroku

Falls die Studenten dieser Gruppe zu früh fertig sind (was wahrscheinlich ist), sollen diese die Aufgaben der Gruppe Gitlab bearbeiten.

## Aufgaben Gruppe GitLab
Diese Aufgabe besteht aus zwei Teilaufgaben.

### Teilaufgabe 1
1. Das GitLab-Repository "IWS-Demo" forken (https://gitlab.com/pdomscheid/iws-demo)
2. Eine Pipeline erstellen, welche aus drei Schritten besteht: (https://docs.gitlab.com/ee/ci/pipelines.html)
   1. Build: Baut das Projekt
   2. Test: Führt die Tests aus
   3. Deploy: Echo das das Projekt deployed wurde

### Teilaufgabe 2
1. Das GitLab-Repository "MSO Backend" forken (https://gitlab.com/pdomscheid/MSO-Backend)
2. Eine Pipeline erstellen, welche aus zwei Schritten besteht: 
   1. Build: 
      1. Baut das Projekt
      2. Baut das Frontend im Root-Ordner dist
   2. Deploy: Deployed das Projekt auf Heroku (https://medium.com/swlh/how-do-i-deploy-my-code-to-heroku-using-gitlab-ci-cd-6a232b6be2e4)
   3. Speichere die Dist-Ausgabe als Artifakt im Build 

## Abschluss
Ein Spiderchart soll für die verschiedenen Tools angelegt werden. Dafür sollen folgende Punkte mit Werten von 0 (schlecht) - 5 (sehr gut) bewertet werden:
- Installation
- Konfiguration
- Erweiterbarkeit (Plugins)

Die Bewertung bitte an die "Tutoren" weiterleiten!


