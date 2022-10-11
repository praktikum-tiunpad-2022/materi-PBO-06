---
layout: center
---

# Inner Class

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex-row'>
<div class='text-base text-justify mt-4'>

Dalam Java, sebuah class dapat memiliki class lagi didalamnya. Class yang berada di dalam class lain disebut inner class atau nested class.  

*Kenapa menggunakan inner class?*  

Jika penggunaannya tepat, nested/inner classes membuat kode menjadi lebih mudah untuk dibaca dan dipahami.  

</div>
</div>

<div class='flex-row'>
<div class='text-base text-justify mt-4' v-click="1">

```java
class OuterClass { // outer class
    int x = 5; // member outer class
    class InnerClass { // inner class
        int y = 10; //member inner class
    }
}

public class Main {
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();

        // instansiasi inner class
        // walaupun outer class punya inner class
        // tidak memiliki objek inner
        OuterClass.InnerClass inner = outer.new InnerClass();
        System.out.println(outer.x + inner.y);
    }
}
```

</div>
</div>

</div>
