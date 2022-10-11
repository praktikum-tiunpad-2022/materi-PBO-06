---
layout: center
---

# Static Inner Class

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex-row'>
<div class='text-base text-justify mt-4'>

Inner class juga dapat didefinisikan secara static. Ini memungkinkan inner class dapat diakses dan diinstansiasi tanpa harus menginstansiasi outer class nya terlebih dahulu.  

Sama halnya dengan member static lain. Sebuah static inner class tidak dapat mengakses member non-static dari luar definisinya.  

</div>
</div>

<div class='flex-row'>
<div class='text-base text-justify mt-4' v-click="1">

```java
class OuterClass { // outer class
    int x = 5; // member outer class
    static class InnerClass { // inner class
        private int y = 10; // member inner class

        public int getY() { // getter y
            return this.y;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        OuterClass.InnerClass inner = new OuterClass.InnerClass();

        System.out.println(inner.getY()); // 10
    }
}
```

</div>
</div>

</div>
