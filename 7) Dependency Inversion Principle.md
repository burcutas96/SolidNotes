# Dependency Inversion Principle (Bağımlılığın Tersine Çevrilmesi Prensibi) Nedir?

<p>
Dependency inversion principle, bir sınıfın herhangi bir türe olan bağımlılık durumuna karşı dikkatimizi çeken ve bu bağımlılığın mümkün mertebe tersine çevrilmesini öneren bir ilkedir.
</p>

<p>
Dependency inversion principle; olayı, kurgudaki aktörü herhangi bir davranışa bağımlı kılma, davranışları aktöre bağımlı kıl. Bunu yapabilecek şekilde düşüncen olsun diyor.
</p>

<p>
Bu prensip, geliştiricinin herhangi bir türe bağımlı olmadığını bilakis türlerin / yani nesnelerin geliştiriciye bağımlı olduğunu savunur.
</p>

<p>
Bu ilkeyi anlayabilmek için birkaç örnek üzerinden istişare etmekte fayda vardır. 
</p>

<img src="img/dependecy-inversion.png">

<br><br>

<p>
Yazılım üzerinden örnek;
</p>

<p>
Yanlış olan:
</p>

<img src="img/dependecy-inversion-2.png">

<br>

<p>
Dependeny inversion ile doğru olan:
</p>

<img src="img/dependecy-inversion-3.png">

<br>

<p>
Özetle; yazılımda gidişat tek bir davranışa bağımlı olmamalı, bilakis davranışlar sizin kararınıza bağımlı olmalı... 
</p>

<p>
Dependency inversion prensibi, bir sınıfın concrete (somut) sınıflara değil, onların abstraction'larına bağlı olması gerektiğini önerir. Böylece o sınıf herhangi bir somut sınıfa bağımlı olmayacak, tam tersine somut sınıf(lar) ilgili sınıfa bağımlılık sergiliyor olacaktır. 
</p>

<p>
Böylece hiçbir sınıf concrete (somut) yapılanmalara değil onların abstraction'larına soyut yapılarına güvenecektir.
</p>


<img src="img/dependecy-inversion-4.png">

<br>

<p>
Son olarak;
</p>


<p>
Dependency inversion prensibi, sınıflar arasındaki bağımlılığı soyutlamakta, uygulamanın ihtiyaca göre davranış değişikliğine istikrar getirmekte ve sistem açısından sürdürülebilirlik  ve ölçeklenebilirliği sağlamaktadır.
</p>
