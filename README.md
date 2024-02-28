# 11-mermaid-mhuber

```mermaid
    MonoBehaviour <|-- PlayerController
    MonoBehaviour <|-- EnemyController
    MonoBehaviour <|-- GameController
 
    class GameController {
        - player: GameObject
        - enemy: GameObject 
        + void Start()
    }
    class PlayerController {
        - speed: float 
        + void Update()
    }
 
    class EnemyController {
        - chaseSpeed: float 
        - target: Transform 
        + void Update()
    }
```
