# Autoboxing dan Unboxing

<div class="grid grid-cols-2 gap-4">

<div v-click="1">

- “Autoboxing” adalah proses boxing yang dilakukan secara otomatis.  

Jangan digunakan didalam loop!!!
Autoboxing akan memperlambat loop dan mengkonsumsi banyak sumber daya sia-sia.  
<br>
<br>

- “Unboxing” adalah proses ketika value dari type wrapper di-unwrap untuk mendapatkan value dalam tipe primitifnya.
</div>

<div>
<div v-click="2" class="">

```java
public static Integer tambahWrapper(Integer a, Integer b) {
    return a + b;
}

public static void main(String[] args) {
    //  Autoboxing
    Integer hasil1 = tambahWrapper(10, 20);
    Integer num1 = 80;

    // Unboxing
    int hasil2 = tambahWrapper(3, 4);
    int num2 = num1;
}
```

</div>
</div>
</div>
