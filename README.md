# asig
 select usuario.codusu, calendario.inipro, calendario.convoc, calendario.charinfo, calendario.aseso 
from usuario inner join calendario on usuario.codusu = calendario.codcal where extract( month from inipro) between 9 and 10; 

 select usuario.codusu,usuario.nomusu, usuario.apeusu, archiinv.titarchi, calendario.presenpro from archiinv inner join usuario on usuario.codusu = archiinv.codarchi inner join calendario on calendario.codcal = archiinv.codarchi WHERE calendario.presenpro <= CURRENT_DATE-100;
