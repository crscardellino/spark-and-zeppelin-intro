# Introducción a Apache Spark y Apache Zeppelin - WTPC 2019 @ FCQ-UNC

Slides de la presentación disponibles en [Google Slides](https://docs.google.com/presentation/d/1lsDqZe5voPZ4o3-9pux2DCSedFatiqiJ_MWI39d2uF8/edit?usp=sharing).

## Instrucciones para ejecutar el notebook

- Descargar y levantar [Apache Zeppelin](http://zeppelin.apache.org/) (ver más abajo).
- Importar el notebook `zeppelin-notebook.json`.

## Descarga e instalación de Apache Spark

    ~/ $ curl -LO http://apache.dattatec.com/spark/spark-2.4.3/spark-2.4.3-bin-hadoop2.7.tgz
    ~/ $ tar xvf spark-2.4.3-bin-hadoop2.7.tgz
    ~/ $ cd spark-2.4.3-bin-hadoop2.7
    ~/ $ ./bin/pyspark --master local[*]  # o ./bin/spark-shell para Scala
    >>> textfile = spark.read.text(“README.md”)

## Descarga e instalación de Apache Zeppelin

    ~/ $ curl -LO http://apache.dattatec.com/zeppelin/zeppelin-0.8.1/zeppelin-0.8.1-bin-all.tgz
    ~/ $ tar xvf zeppelin-0.8.1-bin-all.tgz
    ~/ $ cd zeppelin-0.8.1-bin-all
    ~/ $ ./bin/zeppelin-daemon.sh start  # o ./bin/zeppelin-daemon.sh stop

Cuándo haya iniciado, dirigirse a `http://localhost:8080/`