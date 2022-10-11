# Assignment 6 Soal 3

<div>
Perbaiki program di bawah ini agar bisa di compile dengan tidak mengubah kode pada main method!
</div>


<div class="center">

```java
class Test {
    private final String s;

    static class Inner {
        void testMethod() {
            s = "set from inner";
            System.out.println(s);
        }
    }

    // Don't change the code below!
    // Code below must be executed without error!
    public static void main(String[] args) {
        Test.Inner inner = new Test.Inner();
        inner.testMethod();
    }
}
```

</div>