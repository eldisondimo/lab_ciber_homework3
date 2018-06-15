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
3. Eseguire lo script "run.sh"<br>
```console
$ ./run.sh
```
