# KitchenChaos

Course by [Code Monkey](https://www.youtube.com/watch?v=AmGSEH7QcDg)

哔哩哔哩搬运版： [Unity 游戏开发初中级教程2023版](https://www.bilibili.com/video/BV1UN4y117rz/)

## Naming Rules

* Spend time deciding on a proper name!
* Don't be afraid to rename things
* Don't use single letter names
* Don't use acronyms or abbreviations

## Code Style
```
public class MyCodeStyle : MonoBehaviour {
    // Constants: UpperCase SnakeCase
    public const int CONSTANT_FIELD = 56;

    // Properties: PacalCase
    public static MyCodeStyle Instance { get; private set; }

    // Events: PacalCase
    public event EventHandler OnSomethingHappened;

    // Fields: camelCase
    private float memberVariable;

    // Function Names: PacalCase
    private void Awake() {
        Instance = this;

        DoSomething(10f);
    }

    // Function Params: camelCase
    private void DoSomething(float time) {
        // Do something...
        memberVariable = time + Time.deltaTime;
        if (memberVariable > 0) {
            // Do something else...
        }
    }
}
```