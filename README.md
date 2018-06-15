# Labiratorio ciberfisico: homework 3

## Composizione gruppo
_ Dimo Eldison (VR421018)<br>
_ Vicario Rudy (VR424611)<br>

## Descrizione progetto
L'obiettivo di questo homework consiste nel visualizzare e clusterizzare una pointcloud generata da una rosbag registrata con un drone volante, utilizzando le librerie PCL e OpenCV.<br>
L'homework è composto da 4 parti:<br>
1) Installazione di ORB_SLAM2<br>
2) Esecuzione di ORB_SLAM2 sulla rosbag V1_01_easy.bag<br>
3) Creazione e salvataggio di una pointcloud in un file .pcd<br>
4) Clusterizzare i punti contenuti nella pointcloud generata al punto 3 e visualizzarli<br>

### Immagini della pointcloud
![foto1](images/foto1.jpeg "foto1")
![foto2](images/foto2.jpeg "foto2")
![foto3](images/foto3.jpeg "foto3")
![foto4](images/foto4.jpeg "foto4")

## Istruzioni per l'esecuzione
1. Nella cartella dell'homework, eseguire lo script "build.sh"<br>
```console
$ chmod +x build.sh
$ ./build.sh
```
2. Spostare la bag su cui si vuole eseguire l'homework nella cartella dell'homework<br>
3. Modificare il percorso della export nello script "run.sh" in modo da identificare il path della cartella ORB_SLAM2/Examples/ROS<br>
4. Eseguire lo script "run.sh"<br>
```console
$ ./run.sh
```
Verranno aperti 3 terminali contenenti rispettivamente:
_ Roscore
_ ORB_SLAM2
_ la bag: inizialmente in pausa, premere <i>spazio</i> per avviarla

Una volta terminata l'acquisizione dei punti premere <i>CTRL-C</i> sul terminale dell'ORB_SLAM2 per poter salvare i dati appena acquisiti nel file <b>pointcloud.pcl</b>.
