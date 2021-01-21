# examen

1/ On appelle interopérabilité, la capacité d'un produit ou un système, ayant des interfaces intégralement connues, à fonctionner avec d’autres produits ou systèmes déjà existants ou futurs et cela sans restriction d’accès ou de mise en œuvre

2/ Le web est le réseau des réseaux. Cette phrase, es soit, montre à quel point le web est un bon exemple d'interopérabilité. Mille et un réseaux communiquent entre eux pour former le web.

3/ 
1. HTML - format de données
2. URI - adressage et nommage
3. HTTP - protocole de requêtes

Elles font un socle pratique pour l'open data car si elles sont bien définies dans un site web, tout le monde pourra accéder au ressources, partout dans le monde.

4/
Client web: un logiciel en capacité d'envoyer  à un serveur web, des requêtes HTTP et d'afficher les résultats. Les clients web les plus répandus sont les navigateurs web.
Serveur web: un logiciel en capacité de répondre à des requêtes HTTP. EN d'autres termes, il est capable de renvoyer des données (par exemple une page HTML ou du json), en réponse à des demandes écrites en HTTP (par exemple une requête GET ou POST).


exercice2:
Requete fetch testé sur navigateur:
fetch('https://otakuotake.herokuapp.com/get2randomcharacters', { method: 'GET',
                            headers: {},
                            mode: 'cors',
                            cache: 'default'}).then(
                        function(response){
                            response.json().then(
                                function(data){ 
                                    if (data.length>0){//si on a accès à des ventes de la commune dans l'url
                                    console.log(data)
                                    }
                                    
                                }
                            )
                        }
                    );


