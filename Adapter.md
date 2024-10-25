The adapter converts an original interface of a component into another interface through an intermediate object. Used to resolve incompatible interfaces/provide more stable interface to components of differing interfaces.
Decouples client from interface implementation and encapsulates within adapter.
#### Examples
![[Pasted image 20241024220506.png]]
![[Pasted image 20241024215632.png]]
![[Pasted image 20241024215659.png]]
![[Pasted image 20241024215730.png]]
```java
public interface IDisneyAdapter {  
	public void move();
}
// Without adapter
public class SlothAdapter implements IDisneyAdapter {
	private Sloth theSloth;
	public SlothAdapter(String name) {
	theSloth = new Sloth(name);
	}
	public void move() {
		theSloth.wake();
		theSloth.pushToClimb();
	}
}

public class DisneyMadess {
	public static void main(String[] args) {
		//With adapter
		IDisneyAdapter slothAdt = new SlothAdapter("Flash");
		slothAdt.move();
		
		IDisneyAdapter ironManAdt = new IronManAdapter("Tony");
		ironManAdt.move();
		
		IDisneyAdapter trooperAdt = new TrooperAdapter("Storm");
		trooperAdt.move();
	}  
}
```