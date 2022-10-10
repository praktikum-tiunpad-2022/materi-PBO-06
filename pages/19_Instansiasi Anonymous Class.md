# Instansisasi Anonymous Class

<div class="grid grid-cols-2 gap-4">

<div v-click="1" class="">

Extend sebuah class yang ada(concrete/abstract).  

```java
class Base {
    public void printSomething() {
        System.out.println("halo! saya base class");
    }
}

public class Main {
    public static void main(String[] args) {
        Base obj = new Base() {
            @Override
            public void printSomething() {
                System.out.println("halo! saya anon");
            }
        };

        obj.printSomething();
    }
}
```

</div>

<div v-click="2" class="">

Implementasi interface.  

```java
interface Animal {
    public void speak();
}

public class Main {
    public static void main(String[] args) {
        Animal semut = new Animal() {
            @Override
            public void speak() {
                System.out.println("sup bro");
            }
        };

        semut.speak();
    }
}
```

</div>
</div>
