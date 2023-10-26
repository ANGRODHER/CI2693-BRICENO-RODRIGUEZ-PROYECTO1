Angel Rodriguez 15-11669
Kevin Briceño 15-11661

Proyecto I: Grafo


Objetivo: El objetivo de este proyecto es la implementacion de lista de adyacencias para grafo dirigidos

Descripción general: Implementar mendiate una interfaz Graph, un Grafo cualquiera que se le pueda ralizar operaciones de adicion, eliminacion de un nodo, encontrar un nodo, tamaño del grafo, etc.

Implementación: Se creó la clase AdyacencyListGraph.java, en ella utilizaremos una tabla de hash que almacenará cada nodo del grafo; además, tendremos un arreglo de la clase edge que almacenará las conexiones entre los nodos.

Contenido:

1. AdyacencyListGraph.java: como se explica anteriormente, esta clase tendrá la tarea de tener todas la funciones necesaria para manejar la interfaz de un grafo. No solo contiene la tabla de hash y el arreglo que almacenan vertices y sus arcos respectivamente, sino que, además, contiene los métodod de añadir un nodo, eliminar un nodo, buscar si un nodo está contenido, conectar y desconectar dos nodos, nodos adyacentes a un nodo dado, tamaño del grafo, generacion de un subgrafo a partir de un grafo, predecesores y sucesores
	
2. connect.java: esta clase está implementada con un metodo abstracto, contiene tambien el constructor que almacena los id de las conexiones así como los metodos de para busqueda y un toString

3. edge.java: esta es un clase hija de connect, esta clase por medio de un extend, el extremo de inicio con el extremo final de un par de vertice, creado así un arco entre ellos.

4. Graph.Java en la interfaz principal, a patir de alli se harán todas las llamadas correspondientes y se podrá hacer uso de los método mencionados en adjacencyListGraph

5. vertex.java: Es la clase que almacena los nodos con un respectivo id, en ella tenemos método de buscar un nodo.

6. ClienteCorreccionP1.Java: esta clase contiene el main, desde aqui se cargaran los grafos y se haran las llamadas a los métodos que estan en la intefar Graph.

Notese: que en las clases vertex, edge, connect encontrará algunos constructores adicionales que no se estáran usando en este proyecto, se implementaron con el fin de ser usados más adelante, ya que no solo no dan el id de nodo, sino que permiten asignarles un peso a ese nodo o arco. Lo que permitirá en un furuto implementar caminos ponderados en un grafo.


complejidad aproximada segun el método:

 Ya que se está usando tablas de hash, los metodo de añadir, contener, remover y tamaño tiene una complejidad O(1) constante. Mientras que los métodos relacionados a las conexiones contienen ciclos for para un arreglo con la cardinalidad de las conexiones, por tanto su complejidad sería O(n)

Complejidad aproximada total: O(n)
