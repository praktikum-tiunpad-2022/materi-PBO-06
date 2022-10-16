# Inner Class Access Modifier

<div class="grid grid-cols-2 gap-4">

<div v-click="1" class="">

Seperti member lainnya, inner class dapat memiliki access modifier seperti private dan protected.  

```java
class OuterClass { // outer class
    int x = 5; // member outer class
    private class InnerClass { // private class
        int y = 10; //member inner class
    }
}

public class Main {
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();

        // jika private maka inner class
        // tidak bisa dipanggil
        OuterClass.InnerClass inner = outer.new InnerClass();
        System.out.println(outer.x + inner.y);
    }
}
```

</div>

<div v-click="2" class="">

Inner class (jika tidak static) dapat mengakses member milik outer class-nya.  

```java
class OuterClass { // outer class
    int x = 5; // member outer class
    private class InnerClass { // inner class
        public int getOuterX() {
            return x; // mengambil x dari outer
        }
    }
}

public class Main {
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();

        // instansiasi inner class
        OuterClass.InnerClass inner = outer.new InnerClass();
        System.out.println(inner.getOuterX()); // 5
    }
}
```

</div>
</div>
