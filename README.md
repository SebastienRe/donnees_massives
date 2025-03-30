# Données massives avec Hadoop

[https://github.com/big-data-europe/docker-hadoop/tree/master](https://github.com/big-data-europe/docker-hadoop/tree/master) customisé pour le cours de données massives.

## Utilisation

Connecter vous en SSH sur votre conteneur Namenode, via visual studio code ou autre, au ossier ```/opt/hadoop-3.2.1/```

Au démarrage, en ligne de commande, exécuter la commande suivante :

```bash
$HADOOP_HOME/sbin/start-yarn.sh
```

cela permet de démarrer le service YARN ce qui permet de lancer des jobs MapReduce.
Developper le code MapReduce dans dossier ```codes```

executez :

```bash
$HADOOP_HOME/bin/hdfs dfs -mkdir -p /user/root
```

pour créer le répertoire de l'utilisateur root sur HDFS.
pour ajouter des fichiers d'entrées, exécutez la commande suivante :

```bash
$HADOOP_HOME/bin/hdfs dfs -put input /user/root/input
```
