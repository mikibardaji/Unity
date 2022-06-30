# Unity
Descripció programa fet pas a pas

Partim del programa que ja li hem creat una figura, que al apretar el espai ens salta.
També hem fet que sol es pugui fer un salt, i fins que no caigui no serveixi de res apretar el espai.
[AssetStore](https://assetstore.unity.com/ "AssetStore"), vam agafar endless runner, i alli tenim art i audios.

#####PlayerController.cs
RayOrigin es un raig, que serveix per saber, si col·lisiona, amb alguna forma, si la distancia amb lo que ha colisionat es menor que 1, llavors estas al terra. 
Es un gameobject buit
![RayCast](ray.png "RayCast")


##### Platformcontroller.cs
PlatformCreator, vaig a buscar la definció. En cada frame, si la plataforma que s'esta movent esta en una X negativa, crea una plataforma.
**Quaternion.identity** es per ficar la rotació, que en aquest cas ho fiques amb la rotació de la prefab.
També destruim la plataforma quant es troba a menys 15.
**Debug** quant puges a producció, els prefabs tenen que anar obligatoriament, a la carpeta resources. Els assedatasets. sol existeixen quant treballem amb producció.

![Debug](debug.png "Debug")
