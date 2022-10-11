# Instansisasi Anonymous Class (lanj.)

<div class="grid grid-cols-1 gap-4">

<div v-click="1" class="">

Instansiasi pada saat pemberian argumen sebuah method.  
<div class="grid grid-cols-2 gap-4">
<div>

```java
class SomeClass {
    public void printSomething() {
        System.out.println("something");
    }
}
```

</div>
<div>

```java
public class Main {
    static void execute(SomeClass obj) {
        obj.printSomething();
    }

    public static void main(String[] args) {
        execute(new SomeClass() {
            @Override
            public void printSomething() {
                System.out.println("Overriden print!");
            }
        });
    }
}
```

</div>
</div>

</div>
</div>
