https://youtu.be/RfxuXKgiek0
--------------------------

Code dedicated to electric motor

Define a new  virtual Turn sensor  that we can adjust in AgOpenGPS setting 

  During autosteer   the WAS evaluate error 

   If the error  keep or  reduce   we can consider that is normal 
But  if the error  increase more and more   it look like an annormal situation :
 Like   manual steering  or was sensor  do trouble

 This code   check the error  and   add the quantity of error according anormal situation  
    with  a result  taht  he stop autosteer in case of  the value of turnsensor will be exceed the  error quantity


Based  on   quality  of  answer   from AgopenGPS setting  and  the hardware  we can set  Turn sensor arround  30 to 60  

------------------------------------------------------
Code dédié au moteur électrique

Définir un nouveau capteur de rotation de volant virtuel que l'on peut ajuster dans les paramètres d'AgOpenGPS 

  Pendant l'autoguidage, le WAS évalue l'erreur du WAS ( capteur d'angle de la roue) :
Si l'erreur se maintient ou se réduit, on peut considérer que c'est normal. 
Mais si l'erreur augmente de plus en plus, il s'agit d'une situation anormale :
 Comme si la direction etait manuelle ou le capteur de WAS avait  un probleme

 Ce code vérifie l'erreur et ajoute la quantité d'erreur en fonction de la situation anormale.  
    Le résultat est qu'il arrête l'autoguidage si la valeur du capteur de rotation de volant est supérieure à la valeur de quantité d'erreur.


En fonction de la qualité de la réponse de l'AgopenGPS et du matériel, nous pouvons régler la valeur du capteur de virage entre 30 et 60. 

-----------------------------------------------------------------------------------------------
Bonus ;  it include the  switch mode to stop autosteer ( code from Matthew Elias)
Bonus : inclus  le switch mode  et  l'arret de l'autosteer ( code de Matthew Elias)
https://github.com/m-elias/AgOpenGPS_Boards/tree/master/TeensyModules/V4.1/Firmware

