# ScriptSignals
1. # instalar
    -usá ```pip install ScriptSignals``` para instalar ScriptSignals
2. # importar
    -usa ````import ScriptSignals```` para importar ScriptSignals
3. # usar
    1. # send:
       - funcion: enviar informacion a otro script
       
       - argumentos: servidor, mensaje, datos, nombre, funcion
       1. servidor, es el servidor a enviar
       2. mensaje, es el mensaje a enviar
       3. datos, son datos extra en formato personalizado
       4. nombre, es el nombre del cliente
       5. funcion, es una funcion que se ejecutara si un servidor responde al mensaje
          
          -argumentos:
          1. info, es una lista con 3 elementos, el mensaje, datos extra sobre el y el servidor que lo envio
      2. # respond
         - funcion, es una funcion exclusiva del servidor para responder a mensajes
         - argumentos
         1. cliente
         2. mensaje
         3. datos
         4. nombre
         - cliente es el cliente a responder
         - mensaje es el mensaje a enviar
         - datos son datos extras a enviar
         - nombre es el nombre del servidor
      2. # create_server
         - funcion, es para convertir tu script en un servidor en un hilo aparte de manera que no bloquea el flugo principal del programa
         - argumentos
         1. funcion
         2. nombre
         - funcion es una funcion con los argumentos info que debe ser una lista de 3 elementos, un elemento es el mensaje recibido, el otro la informacion extra del mensaje, y el otro es el nombre del cliente que lo envio
         - nombre, es el nombre del servidor, los clientes deberan referenciarlo para que llegue el mensaje
