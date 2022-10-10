---
layout: center
---

# Exercise <kbd><span class='text-teal'>Test.java</span></kbd>

<div class="grid grid-cols-1 gap-2">

<div class="text-sm">

Perbaiki program di bawah ini agar bisa di compile dengan tidak mengubah kode pada main method!

</div>

<div>

```java
public class Problem {
    private final String s;

    class Inner {
        static void testMethod() {
            s = "set from inner";
            System.out.println(s);
        }
    }

    // Dont change the code below!
    // Code below must be executed without error!
    public static void main(String[] args) {
        Problem.Inner inner = new Problem.Inner();
        inner.testMethod();
    }
}
```

</div>

</div>
