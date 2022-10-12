# Fungsi Type Wrapper

<div class="text-sm">

**Type Wrapper** dari java.lang bersifat **IMMUTABLE**.


</div>
<br>
<div class="grid grid-cols-2 gap-4">
<div class='flex-row'>
<div class='text-orange text-4xl font-extrabold'>01</div>
<div class='font-light text-sm'>Untuk melakukan modifikasi value dari argumen dalam method. Dengan syarat, object harus bersifat Mutable.</div>
</div>
<div class='flex-row'>
<div class='text-orange text-4xl font-extrabold'>02</div>
<div class='font-light text-sm'>Class-class dalam package java.util semuanya bekerja dengan object saja. Tidak bisa dengan tipe primitif.</div>
</div>
<div class='flex-row'>
<div class='text-orange text-4xl font-extrabold'>03</div>
<div class='font-light text-sm'>Class-class pada Java Collection Framework seperti Vector dan Linked List hanya bisa menyimpan object saja.</div>
</div>
<div class='flex-row'>
<div class='text-orange text-4xl font-extrabold'>04</div>
<div class='font-light text-sm'>Konkurensi pada Java seperti multithreading hanya bisa bekerja dengan object.</div>
</div>
</div>
<br>
<br>
<div class='text-sm text-justify mt-4 font-light'>

**Mutable Object** adalah object yang isi/konten-nya bisa berubah setelah instansiasi. Ketika suatu object Integer ditambahkan dengan angka lain, maka akan dibuat object Integer baru dari hasil operasinya dan **TIDAK MENGUBAH** object yang lama karena wrapper class Integer bersifat **IMMUTABLE**.

</div>