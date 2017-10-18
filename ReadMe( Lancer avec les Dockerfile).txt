*******************************************************************************************************
***************************** MISE EN PLACE DE L'APPLICATION "dbproject" ******************************
*******************************************************************************************************
                                                                                                      *
OS : Windows 10 Professionnel 64 bits                                                                 *
------------------------------------------------------------------------------------------------------*
Après installation de Docker                                                                          *
												      *
1 - Se mettre sur le dossier téléchargé	à partir du PowerShell					      *
												      *
2 - Exécuter la commande : "docker build -t appliprof2:1.0 ./db"				      *
												      *
3 - Exécuter la commande : "docker build -t appliprof1:1.0 ./MyTomcat"                                *
												      *
4 - Exécuter la commande : "docker run -d -v dbdata:/var/lib/postgresql/data --name db appliprof2:1.0"*
												      *
5 - Exécuter la commande : "docker run -d --name mytomcat --link db -p 9090:8080 appliprof1:1.0       *
												      *
6 - Accéder à l'application via l'adresse : "http://Votre adresse IP:9090/dbproject/accueil.jsp"      *
                                                                                                      *
**************************************  Enjoy !  ******************************************************
*******************************************************************************************************
