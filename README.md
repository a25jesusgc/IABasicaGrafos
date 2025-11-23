# Descrición

Emprega este arquivo para describir os cambios do teu proxecto.

Utiliza o formato en markdown coas marcas básicas que aparcen no seguinte exemplo:

# Título principal
## Subtítulo

Texto normal con **negriña** e *cursiva*.

- Lista 1
- Lista 2

[Ligazón](https://exemplo.com)


```csharp
using UnityEngine;

public class OlaMundo : MonoBehaviour
{
    void Start()
    {
        Debug.Log("Ola, mundo desde C#!");
    }
}

```


# Exercicio IA Basica Grafos
## Edición da escena TanksWaypoints

Engadín una nova zona chamada **Palmeira** (Palm), representada por unha palmeira xigante to medio do mapa.
Esta zona ten un novo Waypoint, o Waypoint **WP009**, ao cal fíxenlle as seguintes conexións:
 - Link 11: WP009 co WP003 (Bidireccional)
 - Link 12: WP009 co WP006 (Bidireccional)
 - Link 13: WP009 co WP007 (Bidireccional)

Para esta nova zona, engadín o botón *Go to Palm* que fai que o tanque se mova ao waypoint[8], que é o WP009.

```csharp
using UnityEngine;

public class TanksWaypointsFollow : MonoBehaviour
{
    // Engadín o seguinte método
    // Ir á palmeira (waypoint 8)
    public void GotoPalm() {
        graph.AStar(currentNode, waypoints[8]);
        currentWP = 0;
    }
}


```