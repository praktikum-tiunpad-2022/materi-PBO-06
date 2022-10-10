---
layout: center
---

# Enum Class

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex-row'>
<div class='text-base text-justify mt-4 font-light'>

**Enum** adalah sebuah konsep yang tidak eksklusif di Java saja. Hampir seluruh bahasa pemrograman mempunyai konsep enum.  

Pada dasarnya, enum adalah sebuah *kumpulan variabel-variabel yang bersifat konstan atau tidak akan berubah*.  

Dalam Java, enum class adalah sebuah class yang “spesial”. Semua konstanta dalam enum class bersifat **public**, **static** dan **final** (tidak bisa di override).   

Enum class bisa saja memiliki method, tapi tidak disarankan. Dan juga enum class **tidak bisa diinstansiasi dan meng-extend class lain**.  

</div>
</div>

<div class='flex-row'>
<div class='text-base text-justify mt-4' v-click="1">

```java
enum Hari {
    SENIN, SELASA, RABU, KAMIS, JUMAT, SABTU, MINGGU
}

public class Main {
    public static void main(String[] args) {
        Hari prakA = Hari.SELASA;
        Hari prakB = Hari.RABU;
    }
}
```

</div>
</div>

</div>
