# com.cglab.gamelibs
## use in unity package

```json
{
  "dependencies": {
    "com.cglab.gamelibs": "https://github.com/jfcarocota/com.cglab.gamelibs.git"
}
```

## InputSystem

### Cabecera de namespace

(Game controller)
```csharp
using GameLibs.GameControlInputs;
```
or

(Manage memory saves)
```csharp
using GameLibs.MemorySystem;
```

### Axis
<p style="text-aling="center";">
 Retuns a Vector2 with the X and Y axis from control:
</p>

  (Example on player controller)
  
  ```csharp
  void LateUpdate()
  {
      anim.SetFloat("axisX", Mathf.Abs(GameControlInputs.Axis.x));
      anim.SetBool("grounding", GameControlInputs.IsGrounding(ref rb2D, ref groundFilter));
      anim.SetFloat("velY", rb2D.velocity.y);
  }
  ```
