# Preguntes

Us faig aquest document amb preguntes i dubtes que tinc cap el profe.

Primer de tot, cal que feu funcionar el projecte, la qual cosa podeu fer instalant les llibreries (si aneu als settings intellij us hauria d'avisar que les instaleu)


## Endpoints news
#### news/?page=2
- **GET :** Retorna totes les instàncies que hi hagi de news (paginades de 30 en 30)
- **POST :** Crea una nova instància de news i la retorna. En cas que no es pugui crear, es retorna `error 400`
  [Enllaç](http://127.0.0.1:8000/news/)
#### news/news_id
- **GET :** Retorna la instància de news que conté la news_id. En cas que no existeixi es retorna `error 400`.
- **PUT :** Actualitza la instància amb la id passada i la retorna. En cas que no existeixi es retorna `error 400`. 
- **DELETE :** Elimina la instància amb la id passada i la retorna. En cas que no existeixi es retorna `error 400`.
  [Enllaç](http://127.0.0.1:8000/news/1)
#### news/ask
-**GET :** Retorna totes les instàncies que hi hagi de news de tipus pregunta (paginades de 30 en 30)
[Enllaç](http://127.0.0.1:8000/news/ask)
#### news/newest
-**GET :** Retorna totes les instàncies que hi hagi de news de tipus pregunta (paginades de 30 en 30)
[Enllaç](http://127.0.0.1:8000/news/newest)


També està feta la comprovació de si es poden utilitzar o no sense estar loguejat. Proveu a loguejar-vos i desloguejar-vos i podreu veure que desapareixen opcions

## Preguntes
> Els endpoints de filtres estan bé? (es a dir, els endpoints de ask i newest)

> Els altres endpoints estan bé?

> La comprovació de si les dades son correctes, estan ben formatejades, etc; l'hauriem de fer aqui al backend o despres al frontend? Exemple: Si ens poden passar que un comentari es de submission i reply_comentari a la vegada (restriccio que no hauria de passar mai)

> Per al sistema de api/key, cal que aquesta sigui assignada a un usuari del sistema? Es a dir, en cas que no estigui loguejat, redirigir-lo al login, fer-li registre el primer cop, i llavors, quan està loguejat se li dona un token
 
> El esquema OpenApi el podem generar amb el mateix backend (hi ha una llibreria que ho fa) o cal que ho fem amb swagger o a ma?