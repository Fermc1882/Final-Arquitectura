# Final-Arquitectura

EXPLICACION DEL HARDWARE:
este codigo funciona con un tubo el cual cuenta con 4 agujeros , este tubo con la funcionalidad de que no se tenga en cuenta la luz externa la cual no provenga directamente de los leds instalados s, los huecos cuentas con dos pares de elementos , cada par contiene una fotorresistencia  y un led los cuales tienen la funcionalidad de detectar cuando un objeto para entre ellos , para  el sistema de cableado se uilizo un arduino UNO en el cual se le pusieron resistencias de 10k a las fotorresistencias y a los leds unas de 1k , todo fue realuzado en tubos de PVC y cable de timbre.

EXPLICACION SOFTWARE:
1.
https://github.com/Fermc1882/Final-Arquitectura/blob/main/Captura%20de%20pantalla%202023-11-14%20151121.png
en esta primera imagen se logra observar todo el setup del proyecto  e el cual de sefinen los dos leds y las dos fotorresistencias y sus conexiones con el arduino las cuales sosn vitales para enviarle la 
señal al codigo cuando se detecte un bajo umbral de luz en el fotorresistor y ded sdefine una distancia la cual es la distancia que tenemos entre una fotopuerta y la otra , en nuestro caso era de 30cm y se paso
a metros para hallar la velocidad y aceleracion en metros sobre segundo.
2.
https://github.com/Fermc1882/Final-Arquitectura/blob/main/Captura%20de%20pantalla%202023-11-14%20151501.png
en esta imagen se ve como se inicializan la velocidad y la aceleracion en 0 , ademas se definen los valores de umbral de luz , los tenemos enn 30 y en 150 ya que es la luz que da cada led en promedio ,
esto para detectar cuanto es la aluz minima que tiene que tener cada fotorresistencia por default .
3.
https://github.com/Fermc1882/Final-Arquitectura/blob/main/Captura%20de%20pantalla%202023-11-14%20151527.png
en esta imagen see pone toda la logica del codigo la cual es que se detecta un boolean de que si un objeto ya paso para que asi el codigo no se corra infinitamente , cuanndo setecta el umbral mas 
bajo de lo normal en la compuerta 1 se empieza un contador el cual se finaliza cuando la otra fotopuerta detecta su umbral mas bajo de lo normal y asi es como obtiene el tiempo que se demoro en pasar entre una y otra para asi proceder a hallar la velocidad y la aceleracion.
4.
https://github.com/Fermc1882/Final-Arquitectura/blob/main/Captura%20de%20pantalla%202023-11-14%20151633.png
y por ultimo se hallan la velocidad , aceleracion y tiempo transcurrido mediante formulas y se muewstra en el print .




