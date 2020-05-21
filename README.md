# app-qae
## ce repository contiendra le poc d'une application des utilisateurs
Nous allons d'abord travailler sur l'entite permission<br>
Voici son contenu : <br>
Permission
  -  id
  -  label
  -  dateCreation
  -  dateUpdated
  -  dateDeleted
  -  isDeleted
<br/>  
1- Voici le format du json lors qui doit etre soumis lors d'un ajout : <br/>
<pre>
{
  label: "test"
}  
</pre>
Et le format retourne par le serveur :
<pre>
{
  id: 1
  label: "test",
  dateCreation: 2015-12-09,
  isDeleted : false,
  dateUpdated: null,
  dateDeleted: null
} 
</pre><br/>
2-Contenu pagination json :
<pre>
{
 data:[
  { 
    id: 1,
    label: "test",
    dateCreation: 2015-12-09,
    isDeleted : false,
    dateUpdated: null,
    dateDeleted: null
  },
  { 
    id: 2,
    label: "test2",
    dateCreation: 2015-11-14,
    isDeleted : false,
    dateUpdated: null,
    dateDeleted: null
  },
  { 
    id: 3,
    label: "test1",
    dateCreation: 2015-09-14,
    isDeleted : false,
    dateUpdated: null,
    dateDeleted: null
  }
 ],
 nbPerPage: 10,
 totalElements: 100,
 totalPages: 10,
 currentPage: 1,
}
</pre>

## Les technologies utilisees sont : Quarkus-Angular et Electron
## Chaque projet fait dans ces technologies se trouvera dans un dossier specifique
