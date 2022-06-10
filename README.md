# LESS-CSS-Beginner-s-Guide
<p>Bu depoda, en popüler CSS ön işlemcilerinden biri olan ve Bootstrap gibi birçok framework Front-end tarafından yaygın olarak kullanılan LESS'i inceleyeceğiz.
<br>Bildiğimiz normal CSS'den farklı olarak, LESS daha çok bir programlama dili gibi çalışır. <br>LESS daha hızlı ve kolay CSS yazabilmemizi sağlayan <ins>dinamik bir araçtır</ins>.</p>
<h4>Sunduğu kolaylıklardan öne çıkanlar şu şekilde sıralabiliriz;</h4>
<ul>
  <li><strong>Variables(Değişkenler):</strong> Örneğin projenize @yazirengi diye bir renk tanımladınız. Daha sonrasında bu değişkeni tüm stil tanımlamalarınızda kullanabilirsiniz. İlerde değiştirmek istediğinizde de hepsini birden yönetmeniz mümkün oluyor.</li>
  <li><strong> Mixins (Stil Birleştirmeleri):</strong> Mixins yapısı sayesinde daha önce başka bir class için tanımladığımız stil seçeneklerini bir başka eleman için de kullanılabilir kılıyoruz. Normal CSS yazarken bu işlem bir çok kodu copy paste yapmamıza sebep olur ve satır sayısını fazlasıyla arttırırdı.</li>
 <li><strong>  Nested Rules (İç içe elemanlar):</strong> İç içe olan elemanları tanımlarken de işler kolaylaşıyor. Eskiden olduğu gibi uzun selectorler yazmamıza artık gerek yok.</li>
  <li><strong>  Operations (Dört İşlem):</strong> LESS içerisinde çarpma, bölme,toplama ve çıkarma işlemleri de yapabiliyoruz. Bu da önceden tanımlanılan değişkeni başka bir yerde kullanmak istediğimizde bu özellik sayesinde bir işleme tabi tutabiliriz.</li>
  <li><strong>  Functions (Fonksiyonlar):</strong> LESS’in fonksiyon desteği onu daha da programlama dili gibi göstermekte. Yapımcılar tarafından tanımlanmış birkaç fonksiyonu artık stil kodlarımız içinde kullanabiliyoruz.</li>
</ul>
<h2> Variables (Değişkenler)</h2>
Less stil dosyamızda normal proglama dillerinde değişken tanımlar gibi bir değişken tanımlayabiliyoruz. Örneğin bir stil özelliğini bir değişken içerisinde tanımlayarak bu stili kullanmak istediğimiz elementlerde tanımladığımız değişkenle çağrılır. Bu da olası bir durumda birgün bu stili değiştirmek istediğimizde tek tek elemenler içerisine gitmek yerine tanımlamış olduğumuz değişkende değiştirmemiz yeterlidir. Hem zamandan tasarruf ederek daha doğru bir şekilde tüm elementlerdeki bu stili değiştirmiş oluyoruz hem de can sıkıcının önüne geçmiş oluyoruz.<br><br>Aşağıda LESS-CSS ve CSS kodların karşılaştırıllması verilmiştir.<br><br>

![Adsız](https://user-images.githubusercontent.com/48285856/171798771-15629c2d-881d-4842-8bb0-cd7f29acc9e0.png)

<br>
<h2>  Mixins (Stil Birleştirmeleri)</h2>
Mixins(Stil Birleştirme), bir elementteki stil özelliklerini başka bir elemente aktarmaktır. Örneğin bir elemente bazı özellikler verdik, başka bir element için de bazı özelliklerin yanında tanımlamış olduğumuz eleemtin özelliklerini de içermesini istiyorsak o element class ını kendi classımıza eklememiz yeterliditr. Böylelikle aynı stil özelliklerini tekrar tekrar yazmamıza gerek kalmaz...<br><br>  

![Adsız](https://user-images.githubusercontent.com/48285856/171990958-46ea0b9d-62ca-479c-a9ca-f8ed0e0256a0.png)

<br>
Less'in  Mixins ile gelen harika başka bir özelliği daha var. "<strong>&</strong>" oparatörü kulllanarak bulunduğu selectoru temsil edecektir. Böylelikle daha hızlı kod yazmamızı sağlamaktadır. Yalnız bu operatörü kullanmak için ilgili selector dizinin içerisinde olmalıyız. Çünkü program ancak bu şekilde operatör hangi selectoru temsil edeceğini bilir.<br><br>

![Adsız](https://user-images.githubusercontent.com/48285856/173003577-c9a84bc7-082c-4f2f-8773-788b9070c044.png)

<br>
<h2>  Nested Rules (İç İçe Elemanlar)</h2>
Bu özelliğin amacı CSS de bir elementin alt elementlerine stil özelliği vermek istediğimizde bu alt elemente gitmek için uzunca selectorler yazmamızı ortadan kaldırmaktır. Böylelikle hem uzun selektorleri yazmamızı ortadan kaldırmış oluyoruz hem de daha anlaşılır bir yapı kullamış oluyoruz. 
<br>  

![Adsız](https://user-images.githubusercontent.com/48285856/172069820-7fb0b4e4-a646-49d0-9db3-a8c3179cd22f.png)

<br>
<h2>  Operations (Dört İşlem)</h2>
 
Stil sayfasındaki sayılara, renklere ve değişkenlere toplama, çıkarma, çarpma ve bölme gibi işlemleri LESS'te de yapabiliriz. <br>
Diyelim ki B elemanı A elemanından iki kat daha büyük olsun. Bu durumda şöyle yazabiliriz:
<br>  

![Adsız](https://user-images.githubusercontent.com/48285856/172378413-3e4c3367-599f-4d5d-972a-5f9b7fffd50e.png)

<br>
<strong>NOT:</strong> Operatörleri kullanırken operator arasına birer boşluk bırakmayı unutmayınız. Aksi takdirde yapmış olduğunuz işlemi bir değişken gibi davranacaktır.
