# Konversi antara Wrapper dan Primitive


<div class="grid grid-cols-2 gap-4">

<div v-click="1" class="">

Primitive -> Wrapper

```java
public static void main(String[] args){
    //  Variable primitif
    int pri = 10;

    //  Constructor sudah diharamkan mulai dari Java 9
    Integer obj1 = new Integer(pri);

    //  Pakai factory method
    Integer obj2 = Integer.valueOf(pri);
    Integer obj2 = Integer.valueOf(10);

}
```

</div>

<div v-click="2" class="">

Wrapper -> Primitive

```java
public static void main(String[] args) {
    //  Wrapper Object
    Integer obj1 = Integer.valueOf(10);
    Character obj2 = Character.valueOf('A');

    //  Konversi ke primitif
    int pri1 = obj1.intValue();
    char pri2 = obj2.charValue();
}
```

</div>
</div>
