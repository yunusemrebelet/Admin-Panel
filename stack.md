# SOFTWARES STACK

## jQuery

### jQuery Nedir?

JQuery cross-platform çalışabilen AJAX kullanımı, DOM manipülasyonu, CSS manipülasyonu gibi işlemlerinde hem daha kolay bir şekilde hem de daha az kod yazarak daha çok şey yapmamızı sağlayan bir JavaScript kütüphanesidir.

### JQuery'nin Projeye Dahil Edilmesi

JQuery'i projede kullanmak için birkaç yol mevcuttur:

1. jQuery.com üzerinden kütüphaneyi indirmek.
2. jQuery'i bilgisayarınıza indirmeden kullanmak istiyorsanız bir CDN (İçerik Dağıtım Ağı) üzerinden de projeye ekleyebilirsiniz. Şu [linki](https://developers.google.com/speed/libraries) kullanabilirsiniz.

### Örnek Bir jQuery Kullanımı

    <!DOCTYPE html>
    <html>
    <head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("#hide").click(function(){
            $("p").hide();
        });
        $("#show").click(function(){
            $("p").show();
        });
    });
    </script>
    </head>
    <body>

    <p>If you click on the "Hide" button, I will disappear.</p>

    <button id="hide">Hide</button>
    <button id="show">Show</button>

    </body>
    </html>

**_\$(document).ready(function()_** kod satırı bütün HTML sayfası yüklendikten sonra jQuery işlemlerinin yapılmasını belirtmek için kullanılır.

jQuery de DOM manipülasyonu yapmak için seçicilere ihtiyaç duyarız. Üstteki örnek kodda **_\$("p")_** bütün **"p"** taglarini seçmek için kullanılır.
Aslında jQuery'de seçiciler CSS seçicileri ile aynıdır. _**".sınıf"**_ ile _**"sınıf"**_ isimli bir class seçmiş oluruz. **_"#sınıf"_** ile _**"sınıf"**_ id sine sahip elementi seçmiş oluruz.

jQuery'de seçiciler ile ilgili daha fazla bilgi almak [için](https://www.javatpoint.com/jquery-selectors).

Örnek kodda _**hide()**_ (seçili elementi gizlemek için) ve **_show()_** (seçili elementi göstermek için) diye iki jQuery fonksiyonu mevcut. Bu ve benzeri DOM manipülasyonu, CSS manipülasyonu AJAX işlemleri ve animasyon yapma gibi işlemler jQuery ile daha kolay ve hızlı bir şekilde yapılabilir.

jQuery'nin detaylarına girmek isterseniz:

[javatpoint](https://www.javatpoint.com/jquery-tutorial)

[w3schools.com](https://www.w3schools.com/jquery/default.asp)

## Bootstrap

### Bootstrap Nedir?

Ücretsiz bir CSS framework’u olan Bootstrap, açık kaynak kodlu bir tasarım aracıdır. Telefon, tablet ve masaüstü bilgisayarlar için farklı ve cihazınızın büyüklüğüyle orantılı şekilde sitenizin görünmesini sağlayan tema ve tasarımları kolaylıkla yapabilirsiniz. Bir site için gerekli olan bütün unsurları içerisinde barındıran Bootstrap ile tasarım yaparken bu hazır unsurları kullanarak tüm cihazlara uygun tasarımlar yapmanızı sağlar. Bu da demek oluyor ki, her şeyi hazır olan kodlarla yeni bir tasarım yaratmak oldukça kolay ve pratiktir. Stiller, imajlar ve JavaScript'ler daha öncesinden Bootstrap'in içine monte edilmiştir. Yapmanız gereken tek şey bunları çağırmanızdır.

### Bootstrap Kurulumu

Npm ile kurmak için:

    npm install bootstrap

CDN ile kurmak için:

[Bootstrap CDN](https://www.bootstrapcdn.com/)

### Örnek Bootstrap Kullanımı

    <div class="card" style="width:400px">
    <img src="img_avatar1.png" alt="Card image">
    <div class="card-body">
        <h4 class="card-title">John Doe</h4>
        <p class="card-text">Some example text.</p>
        <a href="#" class="btn btn-primary">See Profile</a>
    </div>
    </div>

Bu kod satırının çıktısı şu şekilde olacaktır:

![bt](img/oo.png)

Bootstrap içerisinde belirtilen classları elementlerimize verdiğimizde kolay bir şekilde istediğimiz tasarımları ortaya çıkarabiliriz.

## Vue.js

### Vue.js Nedir?

VueJS, kullanıcı arayüzleri geliştirebilmek için açık kaynak kodlu gelişmiş bir JavaScript frameworkdür. Web geliştirmeyi basitleştirmek için en popüler frameworklerden birisidir. VueJS büyük kapsamlı projelere kolayca entegre edilebilir.

### Vue.js kullanımı

Npm ile Vue.cli kurulumu:

    npm install -g @vue/cli

CDN ile kullanmak için:

[Vue.js](https://vuejs.org/v2/guide/)

### Vue.js'de Virtual DOM

Gerçek DOM’a karşılık gelen sanal bir DOM nesnesidir, yani render edilen DOM’un bir kopyasıdır. Vue her state değişikliğinde render edilen gerçek DOM’u bütünüyle tekrar oluşturmak yerine, state değişikliğini Virtual DOM’a yansıtmaktadır. Bu sayede gerçek DOM ile ve yeni sanal(virtual) DOM arasındaki farklılıkları tespit ederek, gerçek DOM’da yapılacak değişikleri hesaplar ve tek seferde sadece gerçek DOM’da değişen elemanları yeniden render eder. Bu şekilde state her değiştiğinde ana DOM’un tüm elemanlarıyla yeniden oluşturulması maliyetinden korunulmuş ve azami performans iyileştirmesi sağlanmaktadır.

### Vue.js'de Component Yapısı

VueJS componentleri, HTML'de yeniden kullanılabilen (reusable) kullanıcı öğeleri oluşturmaya yardımcı olan çok önemli bir işlevdir.

## PHP

### PHP nedir?

PHP sunucu taraflı iletişimler için yaratılmış bir programlama dilidir. Bu nedenle form verisi toplamak, sunucuda dosya yönetmek, veritabanlarını düzenlemek vb. gibi çeşitli sunucu taraflı fonksiyonları yapabilir.

### Sunucu tarafı vs İstemci tarafı

Programlama dilleri ya istemci tarafında (frontend), ya da sunucu tarafında (backend) çalışabilir.

İstemci tarafındaki scriptler web tarayıcıları tarafından işlenir. Tarayıcınız, yani istemci, istemci taraflı scriptleri içeren bir sayfa isterse, sunucu tarayıcı için çalıştırılabilir olan kaynak kodları yollarak cevap verir.

Öte yandan sunucu taraflı programlama dili scriptlerin tarayıcılara yollamadan önce sunucularda çalıştırıldığı anlamına gelir. Yani kaynak kodu yollamadan önce web sunucuları kodları sade bir HTML formatına dönüştürmeden önce işler(çözümler).

Bundan dolayı sunucu taraflı programlama web geliştiricilerin kaynak kodlarını saklamalarına izin verirken istemci taraflı scriptler istemcinin kullanıcıları kolaylıkla görülebilir.

## Composer

Web geliştiricilerin karşılaştıkları birçok sorun, projenin bağımlılıkları (dependencies) ile ilgilidir. Projelerimize yeni paketlerin entegrasyonunu sağlarken, olması gerekenden daha fazla sorun yaşayabiliyoruz.

Bu durum özellikle PHP geliştiricileri için daha sık görülür. Bu nedenle geliştiricilerin bazı temel modülleri sürekli sıfırdan yazdığı görülür. Sonuç ise bu tür gereksiz görevler için çok fazla kaynak kaybıdır.

### Composer Nedir?

PHP için zarif ve basit bir bağımlılık yöneticisidir. Bazılarınız Python için PIP veya Node.js için NPM gibi benzer bağımlılık yöneticilerine zaten aşina olabilir. Basitçe söylemek gerekirse; Composer, projenizin tüm bağımlılıklarını tek bir yerde düzene sokacaktır.

Composer kurulum işlemleri için:

[Composer](https://getcomposer.org/doc/00-intro.md)

## AJAX

AJAX ile web sayfası yüklendikten sonra, sunucu üzerine veri göndermek ve sunucudan veri almak mümkündür. Böylece, sayfa yenilenmeden, sayfanın belirli bir bölümünün, sunucu tarafından alınan verilerle yenilenebilir.

Sunucu ile iletişimi sağlamak için XMLHttpRequest nesnesi kullanılır. Tüm modern tarayıcılar XMLHttpRequest nesnesini destekler.

### XMLHttpRequest Bileşeni ne yapar?

XMLHttpRequest web tarayıcısı üzerinde çalışan bir bileşendir. Bu bileşen asenkron bir şekilde bir web sayfasına istekte(request) bulunabilir ve yine asenkron bir şekilde isteğe karşı gelen cevabı(response) kendisini çağıran yere iletebilir. Bütün bu işlemleri siz farkına varmadan arka planda (background) yaptığı için web uygulamasına sanki bir masaüstü uygulamasıymış hissini verebilirsiniz. Bir örnek vermek gerekirse, bir web formu yaptınız ve formun sunucuya gönderilmesi için bir buton(düğme) koydunuz. Butona basıldığında client tarafında çalışan bir script aracılığıyla(örneğin javascript) bilgiler XMLHttpRequest bileşeni kullanılarak arka planda sunucuya gönderilebilir ve sunucudan istenilen cevap alınabilir. Boylece sayfada sabit kalması gereken içerikler yeniden sunucudan alınmayacağı için hem sunucu yorulmamış olacak hemde kullanıcı daha az beklemiş olacaktır.

## REST

REST( Representational State Transfer) istemci-sunucu arasında hızlı ve kolay şekilde iletişim kurulmasını sağlayan bir servis yapısıdır. REST, servis yönelimli mimari üzerine oluşturulan yazılımlarda kullanılan bir veri transfer yöntemidir. HTTP üzerinde çalışır ve diğer alternatiflere göre daha basittir, minimum içerikle veri alıp gönderdiği için de daha hızlıdır. İstemci ve sunucu arasında XML veya JSON verilerini taşıyarak uygulamaların haberleşmesini sağlar. REST standartlarına uygun yazılan web servislerine RESTful servisler denir.

## Gulp.js

### Gulp.js Nedir?

Gulp, geliştirme yaparken iş akışımızı yavaşlatan işlemleri otomatik yapmamızı sağlayan bir araçtır.

- Açık kaynak kodludur.
- Node.js ve Npm ile çalışır.
- Tekrar eden veya zaman alan işlemler için kullanılır.

### Gulp Ne İçin Kullanılır?

- Script ve style dosyalarını küçültmek için.
- Dosya birleştirmek için.
- Önbelleği temizlemek için.
- Test ve optimizasyon işlemleri için.

## E5 Vs ES6

### ECMAScript?

ECMAScript veya ES, Ecma International tarafından ECMA-262 ve ISO/IEC 16262 standartlarıyla standartlaştırılmış, markalaşmış bir betik dili spesifikasyonudur. Şu anda kendisini izleyen Javascript tabanlı olarak geliştirilmiştir. [Kaynak ve Daha Fazlası](https://tr.wikipedia.org/wiki/ECMAScript).

### Değişkenlerin Tanımlanması

ES5' de değişken tanımlamanın tek yolu **var** anahtar kelimesini kullanmaktı.

ES6' da ise değişken tanımlamak için yeni iki farklı anahtar kelime daha geldi. **let** ve **const**.

#### var

var keyword’ü aralarında en geniş kapsama sahip keyword’dür. Örneklerle inceleyecek olursak

- Sonradan tekrar değiştirilebilir

- Kodun herhangi bir noktasında tekrar tekrar tanımlanabilir.

- Sadece fonksion ile kapsanabilir (function scope) fonksiyon süslü parantezleri içerisinde var ile tanımlanan değişkene dışarıdan erişilemez.

#### let

let keyword’ü sadece tanımlandığı kapsam (block scope) içerisinden erişilebilir. Block scope’dan kasıt her bir süslü parantezin ({}) içerisidir

- Sonradan tekrar değiştirilebilir
- Aynı kapsam (scope) içerisinde sadece bir sefer tanımlanabilir. Tekrar tanımlanmaya çalıştığında kod hata verir ve çalışmayı durdurur.

#### const

const keyword’ü de let gibi sadece tanımlandığı kapsam (block scope) içerisinden erişilebilir. const adından da anlaşılabileceği gibi (constant kelimesinin kısaltılmasıdır) sabittir.

- Sonradan değiştirilemez
- Aynı kapsam (scope) içerisinde sadece bir sefer tanımlanabilir. Tekrar tanımlanmaya çalıştığında kod hata verir ve çalışmayı durdurur.

### Hangi keyword’ü ne zaman kullanmalıyız?

- Mümkün olduğunca const kullan.
- Sadece değişkenin değerini değiştirme ihtiyacın var ise let kullan.
- Eğer ES6 yazıyorsan var kullanma.

### Performans Açısından Karşılaştırma

Kısaca söylemek gerekirse ES6, ES5'den daha performanslıdır.

### Arrow Functions

ES5'de fonksiyon tanımlamak için hem **function** hem de **return** anahtar kelimelerini kullanmamız gerekiyordu.

ES6'da ise arrow function denilen yeni bir özellikle birlikte **function** anahtar kelimesine gerek duymadan fonksiyonlar tanımlayabiliyoruz.

### Spread Operator(...)

ES6 ile gelen bu yeni özellikle birlite array ve objectleri birleştirebiliyoruz.
