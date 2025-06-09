# Unity_VideoOnWebGL
Unity al exportar a WebGL es incapaz de encontrar los vídeos. Este es un bug que lleva años y ocurre en todas las versiónes (Comprobado hasta 2022)
Este proyecto es solo un ejemplo de como resolverlo usando la carpeta "Streaming Assets", la cual es por diferencia la soluciíon más eficiente y fácil.


Pasos:
* Replica el siguiente tutorial:
  https://www.youtube.com/watch?v=p7iXEZGx2Mc

* Crea una carpeta para guardar todos los videos (ej: videos).

* Crea otra carpeta con el nombre de “StreamingAssets” y almacena por segunda vez todos los vídeos.
  StreamingAssets: Es una carpeta reservada de Unity que al exportar se mantiene intacta.

* Descargan estos script y se lo asignan a los objetos: 
1. https://www.notion.so/Trigger-Cambio-de-Escena-33e2e75e38374efdacf56bec6bfb6d10
2. https://www.notion.so/GameMaster-AnanaHides-4e10bcc058ad42568734dceb7a66f201
3. https://lavish-grouse-704.notion.site/PlayVideoInWebGL-3e76a5a32d1d460a9e9a523ec1e0d23a

* En el script “PlayVideoInWebGL”, cambia los nombres de los vídeos por los suyos
* Arrastra los videos de la carpeta “videos” al arreglo “cinematicas” en el inspesctor de VideoPlayer, respetando el orden que defines en “GetVideoDuration()” dentro de “PlayerVideoInWebGL”.

Muy probablemente necesiten modificar más cosas, pero esto es la base.
  
