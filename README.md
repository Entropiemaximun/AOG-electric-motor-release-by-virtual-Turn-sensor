Dedicated Video [https://youtu.be/RfxuXKgiek0](https://youtu.be/6qb0Y6SKDuY)
--------------------------
Code dedicated to the electric motor and its disengagement in the event of setpoint error accumulation.

Define a new virtual steering wheel rotation sensor that can be adjusted in the AgOpenGPS parameters.

During autosteering, the WAS evaluates the WAS (wheel angle sensor) error: If the error is maintained or reduced, this can be considered normal. But if the error is increasing, it's an abnormal situation, such as manual steering or a problem with the steering sensor.

This code checks the evolution of the error and accumulates an index according to the abnormal situation.
As a result, it stops the autosteer if the steering wheel rotation sensor value exceeds the index.

Depending on the quality of the AgopenGPS response and the hardware, we can set the turn sensor value between 30 and 60.

------------------------------------------------------
Code dédié au moteur électrique et a son débrayage  en cas d'accumulation  d'erreur  sur la consigne.

Définir un nouveau capteur de rotation de volant virtuel que l'on peut ajuster dans les paramètres d'AgOpenGPS

Pendant l'autoguidage, le WAS évalue l'erreur du WAS ( capteur d'angle de la roue) : Si l'erreur se maintient ou se réduit, on peut considérer que c'est normal. Mais si l'erreur augmente de plus en plus, il s'agit d'une situation anormale : Comme une reprise du volant manuellement ou le capteur de direction avait un problème.

Ce code vérifie l’évolution de  l'erreur et cumule un  indice en fonction de la situation anormale.
Le résultat est qu'il arrête l'autoguidage si la valeur du capteur de rotation de volant est supérieure à l'indice.

En fonction de la qualité de la réponse de l'AgopenGPS et du matériel, nous pouvons régler la valeur du capteur de virage entre 30 et 60.
-----------------------------------------------------------------------------------------------
Bonus ;  it include the  switch mode to stop autosteer ( code from Matthew Elias)
Bonus : inclus  le switch mode  et  l'arret de l'autosteer ( code de Matthew Elias)
https://github.com/m-elias/AgOpenGPS_Boards/tree/master/TeensyModules/V4.1/Firmware

