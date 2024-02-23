# Interface Segregation Principle (Arayüz Ayrım Prensibi) Nedir?

<p>
Interface segregation principle, bir nesnenin yapması gereken her farklı davranış(lar)ın, o davranış(lar)a odaklanmış özel interface'ler ile eşleşmesini öneren prensiptir.
</p>

<p>
Böylece ihtiyaç olan davranışları temsil eden interface'ler eşliğinde ilgili sınıflara kazandırabilir ve hiçbir sınıfın kullanmadığı bir imzayı zorla implement etmek zorunda kalmaksızın inşa sürecine devam edebiliriz.
</p>

<img src="img/interface-segregation-principle.png">

<br>

<p>
Sınıflara ihtiyaç duymadıkları imzaları arayüzlere zorlayarak işlevsiz metotlar eklemek ISP'yi ihlal etmek demektir.
</p>

<p>
Böylece geliştiriciler açısından ihtiyaç duymayacakları metotlar intellisense'de kalabalığa sebebiyet verip kafalarını karıştırabilir.
</p>

<p>
Yahut interface'de oluşacak herhangi bir değişiklik ister istemez o değişiklikle alakası olmayan sınıflarda da side effect'ler yaratıp oradaki problemlerle ilgilenmeye zorlayabilir. Yani bakımı da lüzumsuz yere zorlaştırabilir.
</p>

<p>
Hacmi geniş olan ve davranışsal olarak farklı yetenekleri içerisinde barındıran interface'ler mümkün mertebe yeteneklerine göre parçalanarak küçültülmelidir.
</p>

<p>
Kümülatif olarak yetenekleri barındıran interface'ler sınıflara uygunlandığı taktirde çoğu sınıf için birçok yeteneğe ihtiyaç duyulmayacağı için anlamsız kalıp olarak tanımlanıp kalacaktır. Bu da istenmeyen bir durumdur.
</p>

<p>
Genellikle bu tarz istenmeyen durumlar salt olarak NotSupportedException veya NotImplementedException gibi hataların fırlatıldığı metotlarda fark edilebilmektedir. Bu tarz metotlar varsa ISP açısından olayın / inşanın değerlendirilmesinde fayda vardır.
</p>

<p>
Az önceki örneğin interface segregation principle'a göre doğru tasarımı aşağıdaki gibi olmalıdır. 
</p>

<img src="img/interface-segregation-principle-2.png">

<br>

<p>
Yazılımdaki davranışları tek bir bütün olarak tutmaktansa, birbirlerinden bağımsız olacak şekilde birden çok parçaya bölmek ideal kod yapısını ortaya çıkarır.
</p>

<p>
Interface segregation principle'ın ihlali, LSP ve SRP'nin de ihlaline sebebiyet vermektedir.
</p>

<p>
ISP, sınıf tarafından desteklenmeyecek metotların lüzumsuz yere tanımlanmamasına karşı odaklanırken; LSP ise benzer şekilde bu tarz işlevsiz metotların barındırıldığı sınıfların kendi aralarında olan değişimleri sürecinde patlama riskini ortadan kaldırmaya odaklanmaktadır.
</p>

<p>
SRP'de ise sınıfların değişmesi için yalnızca tek bir nedenin olması gerektiği söylenirken; ISP'de de hacmi büyük arayüzler yüzünden implemente edilmiş alakasız yöntemlerin değiştirilmesi gibi durumlarda ilgili sınıfta değişiklik gerekeceğinden, sınıfların sadece tek bir değişim nedeninin olması gerektiği söylenir.
</p>


