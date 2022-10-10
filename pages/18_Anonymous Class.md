---
layout: center
---

# Anonymous Class

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex-row'>
<div class='text-base text-justify mt-4'>

Anonymous Class seperti namanya adalah suatu inner class yang tidak memiliki nama.  

*Apa maksudnya?*  

Jadi bayangkan ada sebuah class yang ingin diinstansiasi, tapi kita ingin mengubah  implementasi dalam suatu methodnya untuk instansiasi ini.  

Disini kita tidak usah mendeklarasikan suatu subclass baru dan meng-override method tersebut. Tapi kita bisa menggunakan anonymous class yang meng-extend class tersebut saat instansiasi.  

</div>
</div>

<div class='flex-row'>
<div class='text-base text-justify mt-4' v-click="1">

```java
class Dog {
    public void speak() {
        System.out.println("guk guk!");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog regularDog = new Dog();

        Dog superDog = new Dog() {
            @Override
            public void speak(){
                System.out.println("rill kh bg?");
            }
        };

        regularDog.speak();
        superDog.speak();
    }
}
```

</div>
</div>

</div>
