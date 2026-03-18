# Job 3 - Build et run de l'image Apache/PHP

Image du resultat:

![Apercu Apache PHP](images/php.png)

Se placer dans le dossier job3 avant d'executer les commandes:

```bash
cd job3
```

Creer l'image Docker:

```bash
docker build -t mon-apache-php .
```

Creer le conteneur (sans le demarrer):

```bash
docker create --name mon-apache -p 8080:80 mon-apache-php
```

Demarrer le conteneur:

```bash
docker start mon-apache
```

Resultat visible sur:

```text
http://localhost:8080/
```

Arreter le conteneur:

```bash
docker stop mon-apache
```
