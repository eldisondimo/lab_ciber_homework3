# Labiratorio ciberfisico: homework 3

## Composizione gruppo
_ Dimo Eldison (VR421018)<br>
_ Vicario Rudy (VR424611)<br>

## Descrizione progetto
L'obiettivo di questo homework consiste nel visualizzare e clusterizzare una pointcloud generata da una rosbag registrata con un drone volante, utilizzando le librerie PCL e OpenCV.<br>
L'homework è composto da 4 parti:<br>
1) Installazione di ORB_SLAM2<br>
2) Esecuzione di ORB_SLAM2 sulla rosbag <i>V1_01_easy.bag</i><br>
3) Creazione e salvataggio di una pointcloud in un file .pcd<br>
4) Fare il clustering dei punti contenuti nella pointcloud generata al punto 3 e visualizzarli<br>

## Istruzioni per l'esecuzione dell'acquisizione dei punti dalla bag
1. Nella cartella dell'homework, eseguire lo script "build.sh"<br>
```console
$ chmod +x build.sh
$ ./build.sh
```
2. Spostare la bag su cui si vuole eseguire l'acquisizione nella cartella dell'homework<br>
3. Modificare il percorso della export nello script "run.sh" in modo da identificare il path della cartella <i>ORB_SLAM2/Examples/ROS</i><br>
4. Eseguire lo script "run.sh"<br>
```console
$ ./run.sh
```
Verranno aperti 3 terminali contenenti rispettivamente:<br>
_ Roscore<br>
_ ORB_SLAM2<br>
_ la bag: inizialmente in pausa, premere <i>spazio</i> per avviarla<br>

Una volta terminata l'acquisizione dei punti premere <i>CTRL-C</i> sul terminale dell'ORB_SLAM2 per poter salvare i dati appena acquisiti nel file <b>pointcloud.pcl</b>.

Per poter visualizzare questi punti usare il comando <i>pcl_viewer</i><br>
```console
$ pcl_viewer pointcloud.pcl
```

## Istruzioni per il clustering
1. Spostare il file <b>pointcloud.pcl</b> nella cartella <i>bin</i> contenuta in <i>Cluster</i><br>
2. Spostarsi nella cartella <i>bin</i> contenuta in <i>Cluster</i> ed eseguire "Cluster"<br>
```console
$ cd Cluster/bin
$ ./Cluster pointcloud.pcl
```

### Immagini della pointcloud
![foto1](images/foto1.jpeg "foto1")
![foto2](images/foto2.jpeg "foto2")
