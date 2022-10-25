Hva jeg har gjort:
La til testLogging slik det stod i Canvas
Laget lokalt repository og delt det til Github
La til continuous integration for java med gradle i Actions
Prøvde å pushe, fikk error fra Github
Kjørte disse kommandoene i terminalen (fra: https://stackoverflow.com/questions/58282791/why-when-i-use-github-actions-ci-for-a-gradle-project-i-face-gradlew-permiss)
  git update-index --chmod=+x gradlew
  git commit -m "Make gradlew executable"
La til kode i enden av yml-filen
  - name: Testing
    run: gradle test
Pushet igjen, nå virket det
Leste at testene var PASSED inne i Actions et sted
