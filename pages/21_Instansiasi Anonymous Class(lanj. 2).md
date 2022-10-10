# Instansisasi Anonymous Class (lanj. 2)

<div class="grid grid-cols-1 gap-4">

<div v-click="1" class="">

Anonymous class juga bisa mengakses variabel yang ada dalam block yang sama.  

**DENGAN SYARAT** variabel tersebut harus final atau “effectively” final.

<div class="grid grid-cols-2 gap-4">
<div>

```java
class Base {
    public void printInt(int a) {
        System.out.println("Integer bernilai: " + a);
    }
}
```

</div>
<div>

```java
public class Main {
    public static void main(String[] args) {
        int num = 10;   // "effectively" final
        Base obj = new Base() {
            @Override
            public void printInt(int a) {
                // akses num dalam anon class
                System.out.println(a + num);
            }
        };
        // jika line di bawah diuncomment
        // maka akan error
        // num = 8;
        obj.printInt(5); // 15
    }
}
```

</div>
</div>

</div>
</div>
