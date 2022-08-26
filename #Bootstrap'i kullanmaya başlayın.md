#Bootstrap'i kullanmaya başlayın

Bootstrap, güçlü, özelliklerle dolu bir ön uç araç takımıdır. Prototipten üretime kadar her şeyi dakikalar içinde oluşturun.

##Hızlı başlangıç
Bootstrap'in üretime hazır CSS ve JavaScript'ini herhangi bir derleme adımına gerek kalmadan CDN aracılığıyla dahil ederek başlayın. Bu Bootstrap CodePen demosu ile pratikte görün .


1.Proje kaynak (root) klasörunuze  **Index.html** tanımlı bir dosya oluşturun . Mobil cihazlarda [uygun yanıt verme davranışı](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) için `<meta name="viewport">` etiketi de ekleyin .

```
<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Bootstrap demo</title>
 </head>
 <body>
   <h1>Hello, world!</h1>
 </body>
</html>
```	

2.**Bootstrap'a CSS ve JS ekleyin.** CSS için `<link>`etiketini `<head>` etiketinin içerisine ekleyin. Javascript taglerini `<script>` </body> (açılır listeleri, açılır pencereleri ve araç ipuçlarını konumlandırmak için Popper dahil) içerisinde kalacak şekilde ekleyin. Daha fazlasını öğrenmek için [CDN links](#cdn-links).


```
<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Bootstrap demo</title>
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
 </head>
 <body>
   <h1>Hello, world!</h1>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa" crossorigin="anonymous"></script>
 </body>
</html>
```

Popper ve JS'mizi ayrı ayrı da dahil edebilirsiniz . Açılır listeleri, açılır pencereleri veya araç ipuçlarını kullanmayı planlamıyorsanız, Popper'ı dahil etmeyerek bazı kilobaytları kurtarın.


```
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.5/dist/umd/popper.min.js" integrity="sha384-Xe+8cL9oJa6tN/veChSP7q+mnSPaj5Bcu9mPX5F5xIGE0DVittaqT5lorf0EI7Vk" crossorigin="anonymous"></script>


<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.min.js" integrity="sha384-ODmDIVzN+pFdexxHEHFBQH3/9/vQ9uori45z4JjnFsRydbmQbmL5t1tQ0culUzyK" crossorigin="anonymous"></script>
```	

1. **Merhaba Dünya!** Bootstrapped sayfanızı görmek için tercih ettiğiniz tarayıcıda sayfayı açın. Artık kendi düzeninizi [(layout)](#https://getbootstrap.com/docs/5.2/layout/grid/) oluşturarak, düzinelerce bileşen  [(components)](#https://getbootstrap.com/docs/5.2/components/buttons/) ekleyerek ve [(resmi örneklerimizi)](#https://getbootstrap.com/docs/5.2/examples/) kullanarak Bootstrap ile oluşturmaya başlayabilirsiniz .

##CDN bağlantıları
Referans olarak, işte birincil CDN bağlantılarımız.

Tanım   |   URL
--------
```

CSS     |   https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css
JS      |   https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js

```	

İçindekiler sayfasında listelenen ek yapılarımızdan herhangi birini almak için [CDN'yi de kullanabilirsiniz](#https://getbootstrap.com/docs/5.2/getting-started/contents/).

##Sonraki adımlar

* Bootstrap'ın kullandığı bazı [önemli Global ortam ayarları](#https://getbootstrap.com/docs/5.2/getting-started/introduction/#important-globals) hakkında biraz daha bilgi edinin 
.
* İçerik bölümümüzden Bootstrap'a [nelerin dahil olduğunu](#https://getbootstrap.com/docs/5.2/getting-started/contents/#precompiled-bootstrap) ve aşağıdaki [JavaScript gerektiren bileşenlerin](#https://getbootstrap.com/docs/5.2/getting-started/introduction/#js-components) listesini okuyun .

* Biraz daha güce mi ihtiyacınız var? [Paket yöneticisi aracılığıyla](#https://getbootstrap.com/docs/5.2/getting-started/download/#package-managers) kaynak dosyaları dahil ederek Bootstrap ile oluşturmayı düşünün .

* Bootstrap'i modül olarak kullanmak `< script type="module">` mı istiyorsunuz? Lütfen [Bootstrap'ı modül olarak](#https://getbootstrap.com/docs/5.2/getting-started/javascript/#using-bootstrap-as-a-module) kullanma bölümümüze bakın.

##JS bileşenleri
Hangi bileşenlerin açıkça JavaScript ve Popper'ımızı gerektirdiğini merak ediyor musunuz? Aşağıdaki bileşenleri göster bağlantısını tıklayın. Genel sayfa yapısından emin değilseniz, örnek bir sayfa şablonu için okumaya devam edin.

JavaScript gerektiren bileşenleri 

* Eksik uyarılar
* Durumları ve onay kutusu/radyo işlevlerini arasında geçiş yapmak için düğmeler
* Tüm slayt davranışları, kontrolleri ve göstergeleri için karusel
* İçeriğin görünürlüğünü artırmak için Daralt
* Görüntüleme ve konumlandırma için açılır menüler (ayrıca, [Popper](https://popper.js.org/) gerektirir)
* Görüntüleme, konumlandırma için Modallar, ve kaydırma davranışı
* Hızlandırılmış Çekim ve OffCanvas eklentilerimizi, uyumlu davranışları uygulamak üzere genişletmeye yönelik Navbar
* İçerik bölmeleri arasında geçiş yapmak için sekme eklentili navigasyon cihazları
* Görüntüleme, konumlandırma için vazolar, ve kaydırma davranışı
* Kaydırma davranışı ve gezinme güncellemeleri için kaydırma
* Görüntüleme ve yok etmek için kızarmış ekmek
* Görüntüleme ve konumlandırma için araç ipuçları ve saksılar (ayrıca, [Popper](https://popper.js.org/) gerektirir)

## Önemli Globaller
Bootstrap'ın, tümü neredeyse yalnızca çapraz tarayıcı stillerinin *normalleştirilmesine* yönelik bir dizi önemli küresel stil ve ayar kullanır. Hadi dalalım.

###HTML5 Döküman Türü
Bootstrap, HTML5 doc tipinin kullanılmasını gerektirir. Onsuz, biraz korkak ve eksik bir stil göreceksiniz.

```html
<!doctype html>
<html lang="en">
  ...
</html>
```


###Duyarlı (Responsive Meta Tag) Meta Etiketi
Bootstrap, önce mobil cihazlar için kodu optimize ettiğimiz ve ardından CSS medya sorgularını kullanarak bileşenleri gerektiği gibi büyüttüğümüz bir strateji olan öncelikli olarak mobil için geliştirilmiştir. Tüm cihazlar için düzgün oluşturma ve dokunarak yakınlaştırma sağlamak için, duyarlı görünüm meta etiketini `<head>` etikekinize ekleyin.

```
<meta name="viewport" content="width=device-width, initial-scale=1">
```	

[Hızlı başlangıçta](https://getbootstrap.com/docs/5.2/getting-started/introduction/#quick-start) bunun bir örneğini görebilirsiniz .

###Kutu- Boyutlandırma - (Box Sizing)
CSS'de daha basit boyutlandırma için global **box-sizing** (kutu boyutu) değerini,  **content-box**(içerik kutusu ) yerine **border-box** (kenar kutusu) olarak değiştiriyoruz . Bu **padding**, bir öğenin son hesaplanan genişliğindem etkilememesini sağlar, ancak Google Haritalar ve Google Özel Arama Motoru gibi bazı üçüncü taraf yazılımlarda sorunlara neden olabilir.

Nadiren geçersiz kılmanız gerektiğinde, aşağıdakine benzer bir şey kullanın:

```
.selector-for-some-widget {
 box-sizing: content-box;
}
```

Yukarıdaki snippet ile, **::before ve ::after** aracılığıyla oluşturulan içerik dahil olmak üzere iç içe öğelerin tümü selector-for-some-widget için belirtilen .box-sizing (kutu boyutlarını) değerini alır.

CSS Püf Noktalarında [kutu modeli ve boyutlandırma](https://css-tricks.com/box-sizing/) hakkında daha fazla bilgi edinin .

###Yeniden başlat - (Reboot)

Gelişmiş tarayıcılar arası oluşturma için, tarayıcılar ve cihazlar arasındaki tutarsızlıkları düzeltmek için [Yeniden Başlatma](https://getbootstrap.com/docs/5.2/content/reboot/)'yı kullanırken, ortak HTML öğelerine biraz daha kararlı sıfırlamalar sağlarız.

##Topluluk
Bootstrap geliştirme konusunda güncel kalın ve bu faydalı kaynaklarla topluluğa ulaşın.

* Resmi Önyükleme Blogunu [okuyun ve abone olun](https://blog.getbootstrap.com/) .

* Resmi Slack odasına [katılın](https://bootstrap-slack.herokuapp.com/) .

* IRC'de diğer Bootstrapper'larla sohbet edin. ``irc.libera.chat`` Sunucuda, kanalda ``#bootstrap``.

* Stack Overflow'da uygulama yardımındabulunabilir.(tagged [bootstrap-5](https://stackoverflow.com/questions/tagged/bootstrap-5))

* Geliştiriciler, değişen paketlerde **bootstrap** anahtar sözcüğünü kullanmalıdır veya maksimum keşfedilebilirlik için [npm](https://www.npmjs.com/search?q=keywords:bootstrap) veya benzeri dağıtım mekanizmaları aracılığıyla dağıtırken Bootstrap işlevselliğine ekleyin.

En son dedikodular ve harika müzik videoları için [Twitter'da @getbootstrap](https://twitter.com/getbootstrap)'ı da takip edebilirsiniz .

#Download
Derlenmiş CSS ve JavaScript'i, kaynak kodunu almak için Bootstrap'i indirin veya npm, RubyGems ve daha fazlası gibi favori paket yöneticilerinize dahil edin.

##Derlenmiş CSS ve JS (Compiled CSS and JS)
Projenize kolayca dahil etmek için  Bootstrap v5.2.0 için kullanıma hazır derlenmiş kodu indirin :
* Derlenmiş ve küçültülmüş CSS paketleri (bkz. [CSS dosyaları karşılaştırması](https://getbootstrap.com/docs/5.2/getting-started/contents/#css-files) )
* Derlenmiş ve küçültülmüş JavaScript eklentileri (bkz. [JS dosyaları karşılaştırması](https://getbootstrap.com/docs/5.2/getting-started/contents/#js-files) )

Bu, belgeleri, kaynak dosyaları veya Popper gibi isteğe bağlı JavaScript bağımlılıklarını içermez.

[***Download***](https://github.com/twbs/bootstrap/releases/download/v5.2.0/bootstrap-5.2.0-dist.zip)

##Kaynak dosyaları (Source files)

Kaynak Sass, JavaScript ve belge dosyalarımızı indirerek Bootstrap'i kendi varlık ardışık düzeninizle derleyin. Bu seçenek bazı ek araçlar gerektirir:

* Sass kaynak dosyalarını CSS dosyalarına derlemek için [Sass derleyicisi](https://getbootstrap.com/docs/5.2/getting-started/contribute/#sass)

* CSS vendor öneki için [Autoprefixer](https://github.com/postcss/autoprefixer) 

[Oluşturma araçlarımızın (build tools)](https://getbootstrap.com/docs/5.2/getting-started/contribute/#tooling-setup) tam setine ihtiyacınız varsa , bunlar Bootstrap ve belgelerini geliştirmek için dahil edilmiştir, ancak büyük olasılıkla kendi amaçlarınız için uygun değildirler.

[***Download***](https://github.com/twbs/bootstrap/archive/v5.2.0.zip)

##Örnekler

Örneklerimizi indirip incelemek isterseniz, hali hazırda oluşturulmuş [örneklere](https://getbootstrap.com/docs/5.2/examples/) göz atabilirsiniz:

[***Örnekleri İndir***](https://github.com/twbs/bootstrap/releases/download/v5.2.0/bootstrap-5.2.0-examples.zip)

##jsDelivr aracılığıyla CDN
Bootstrap'in derlenmiş CSS ve JS'sinin önbelleğe alınmış sürümünü projenize sunmak için [jsDelivr](https://www.jsdelivr.com/) ile indirme işlemini atlayın .

```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">


<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa" crossorigin="anonymous"></script>
```


Derlenmiş JavaScript'imizi kullanıyorsanız ve Popper'ı ayrı olarak dahil etmeyi tercih ediyorsanız, Popper'ı tercihen bir CDN aracılığıyla JS'mizden önce ekleyin.

```
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.5/dist/umd/popper.min.js" integrity="sha384-Xe+8cL9oJa6tN/veChSP7q+mnSPaj5Bcu9mPX5F5xIGE0DVittaqT5lorf0EI7Vk" crossorigin="anonymous"></script>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.min.js" integrity="sha384-ODmDIVzN+pFdexxHEHFBQH3/9/vQ9uori45z4JjnFsRydbmQbmL5t1tQ0culUzyK" crossorigin="anonymous"></script>
```

##Paket yöneticileri

En popüler paket yöneticilerinden bazılarıyla Bootstrap'in kaynak dosyalarını hemen hemen her projeye ekleyin. Paket yöneticisi ne olursa olsun, Bootstrap, resmi derlenmiş sürümlerimizle eşleşen bir kurulum için bir [Sass derleyicisi](https://getbootstrap.com/docs/5.2/getting-started/contribute/#sass) ve Otomatik Ön Düzeltici [(Autoprefixer)](https://github.com/postcss/autoprefixer) gerektirir .

###npm

Bootstrap'i Node.js destekli uygulamalarınıza [npm paketiyle](https://www.npmjs.com/package/bootstrap) yükleyin :

```sh
npm install bootstrap@5.2.0
```


``const bootstrap = require('bootstrap')`` veya ``import bootstrap from 'bootstrap'``Bootstrap'in tüm eklentilerini bir önyükleme nesnesine yükler. ``Bootstrap`` modülünün kendisi tüm eklentilerimizi dışa aktarır. ``/js/dist/*.js ``dosyalarını paketin üst düzey dizini altına yükleyerek Bootstrap eklentilerini tek tek manuel olarak yükleyebilirsiniz .

Bootstrap's ``package.json``, aşağıdaki anahtarların altında bazı ek meta veriler içerir:

* ``sass`` - Bootstrap'in ana [Sass](https://sass-lang.com/)  kaynak dosyasının yolu
* ``style``- varsayılan ayarlar kullanılarak önceden derlenmiş olan Bootstrap'in küçültülmemiş CSS'sine giden yol (özelleştirme yok)

 
>Başlangıç ​​projemizle npm üzerinden Bootstrap ile başlayın! Bootstrap'i kendi npm projenizde nasıl oluşturacağınızı ve özelleştireceğinizi görmek için [twbs/bootstrap-npm-starter](https://github.com/twbs/bootstrap-npm-starter) şablon deposuna gidin. Sass derleyicisi, Autoprefixer, Stylelint, PurgeCSS ve Bootstrap Simgelerini içerir.


###Yarn
Node.js destekli uygulamalarınıza [yarn](https://yarnpkg.com/en/package/bootstrap) paketiyle Bootstrap yükleyin :

```sh
$ yarn add bootstrap@5.2.0
```


###RubyGems
[Bundler](https://bundler.io/) ( önerilir ) ve [RubyGems](https://rubygems.org/) kullanarak Ruby uygulamalarınıza Bootstrap'i aşağıdaki satırı ekleyerek yükleyin [Gemfile:](https://bundler.io/gemfile.html)

```sh
$ gem 'bootstrap', '~> 5.2.0'
```

Alternatif olarak, Bundler kullanmıyorsanız, şu komutu çalıştırarak gem'i yükleyebilirsiniz:

```sh
$ gem install bootstrap -v 5.2.0
```

Daha fazla ayrıntı için gem'in [BENİOKU](https://github.com/twbs/bootstrap-rubygem/blob/master/README.md)'suna bakın.

###Yaratıcı (Composer)
Ayrıca [Composer](https://getcomposer.org/) kullanarak Bootstrap's Sass ve JavaScript'i yükleyebilir ve yönetebilirsiniz :

```sh
$ composer require twbs/bootstrap:5.2.0
```

###NuGet
.NET Framework'te geliştirme yapıyorsanız, [NuGet](https://www.nuget.org/) kullanarak Bootstrap'in CSS'sini veya Sass ve JavaScript'i de yükleyebilir ve yönetebilirsiniz . NuGet, ön uç varlıkları için değil, derlenmiş kod için tasarlandığından, daha yeni projeler [libman](https://docs.microsoft.com/en-us/aspnet/core/client-side/libman/) veya başka bir yöntem kullanmalıdır.


```powershell
Install-Package bootstrap
```

```powershell
Install-Package bootstrap.sass
```




#İçerik (Contents)
Önceden derlenmiş ve kaynak kodu çeşitlerimiz de dahil olmak üzere Bootstrap'a neler dahil olduğunu keşfedin.

##Önceden Derlenmiş Önyükleme (Precompiled Bootstrap ):
İndirdikten sonra sıkıştırılmış klasörü açın ve şöyle bir şey göreceksiniz:

bootstrap/
├── css/
│   ├── bootstrap-grid.css
│   ├── bootstrap-grid.css.map
│   ├── bootstrap-grid.min.css
│   ├── bootstrap-grid.min.css.map
│   ├── bootstrap-grid.rtl.css
│   ├── bootstrap-grid.rtl.css.map
│   ├── bootstrap-grid.rtl.min.css
│   ├── bootstrap-grid.rtl.min.css.map
│   ├── bootstrap-reboot.css
│   ├── bootstrap-reboot.css.map
│   ├── bootstrap-reboot.min.css
│   ├── bootstrap-reboot.min.css.map
│   ├── bootstrap-reboot.rtl.css
│   ├── bootstrap-reboot.rtl.css.map
│   ├── bootstrap-reboot.rtl.min.css
│   ├── bootstrap-reboot.rtl.min.css.map
│   ├── bootstrap-utilities.css
│   ├── bootstrap-utilities.css.map
│   ├── bootstrap-utilities.min.css
│   ├── bootstrap-utilities.min.css.map
│   ├── bootstrap-utilities.rtl.css
│   ├── bootstrap-utilities.rtl.css.map
│   ├── bootstrap-utilities.rtl.min.css
│   ├── bootstrap-utilities.rtl.min.css.map
│   ├── bootstrap.css
│   ├── bootstrap.css.map
│   ├── bootstrap.min.css
│   ├── bootstrap.min.css.map
│   ├── bootstrap.rtl.css
│   ├── bootstrap.rtl.css.map
│   ├── bootstrap.rtl.min.css
│   └── bootstrap.rtl.min.css.map
└── js/
    ├── bootstrap.bundle.js
    ├── bootstrap.bundle.js.map
    ├── bootstrap.bundle.min.js
    ├── bootstrap.bundle.min.js.map
    ├── bootstrap.esm.js
    ├── bootstrap.esm.js.map
    ├── bootstrap.esm.min.js
    ├── bootstrap.esm.min.js.map
    ├── bootstrap.js
    ├── bootstrap.js.map
    ├── bootstrap.min.js
    └── bootstrap.min.js.map


Bu, Bootstrap'in en temel biçimidir: hemen hemen her web projesinde hızlı açılan kullanım için önceden derlenmiş dosyalar. Derlenmiş CSS ve JS'nin ( bootstrap.*) yanı sıra derlenmiş ve küçültülmüş CSS ve JS'yi ``( bootstrap.min.*)`` sağlıyoruz. [Kaynak haritalar(Source Map)](https://developers.google.com/web/tools/chrome-devtools/javascript/source-maps) ``( bootstrap.*.map)`` belirli tarayıcıların geliştirici araçlarıyla kullanılabilir. Paketlenmiş JS dosyaları ( ``bootstrap.bundle.js`` ve küçültülmüş ``bootstrap.bundle.min.js``) Popper'ı içerir .


##CSS dosyaları

Bootstrap, derlenmiş CSS'mizin bir kısmını veya tamamını dahil etmek için bir avuç seçenek içerir.
| CSS files | Layout | Content | Components | Utilities |
| --- | --- | --- | --- | --- |
| `bootstrap.css`<br> `bootstrap.min.css`<br> `bootstrap.rtl.css`<br> `bootstrap.rtl.min.css` | Included | Included | Included | Included |
| `bootstrap-grid.css`<br> `bootstrap-grid.rtl.css`<br> `bootstrap-grid.min.css`<br> `bootstrap-grid.rtl.min.css` | [Only grid system](https://getbootstrap.com/docs/5.2/layout/grid/) | — | — | [Only flex utilities](https://getbootstrap.com/docs/5.2/utilities/flex/) |
| `bootstrap-utilities.css`<br> `bootstrap-utilities.rtl.css`<br> `bootstrap-utilities.min.css`<br> `bootstrap-utilities.rtl.min.css` | — | — | — | Included |
| `bootstrap-reboot.css`<br> `bootstrap-reboot.rtl.css`<br> `bootstrap-reboot.min.css`<br> `bootstrap-reboot.rtl.min.css` | — | [Only Reboot]((https://getbootstrap.com/docs/5.2/content/reboot/)) | — | — |


##JS dosyaları
Benzer şekilde, derlenmiş JavaScript'imizin bir kısmını veya tamamını dahil etme seçeneklerimiz var.

| JS Files | Popper |
| --- | --- |
| `bootstrap.bundle.js`<br> `bootstrap.bundle.min.js`<br> | Included |
| `bootstrap.js`<br> `bootstrap.min.js`<br> | – |


##Önyükleme kaynak kodu (Bootstrap source code)
Bootstrap kaynak kodu indirmesi, kaynak Sass, JavaScript ve belgelerle birlikte önceden derlenmiş CSS ve JavaScript varlıklarını içerir. Daha spesifik olarak, aşağıdakileri ve daha fazlasını içerir:

```
bootstrap/
├── dist/
│   ├── css/
│   └── js/
├── site/
│   └──content/
│      └── docs/
│          └── 5.2/
│              └── examples/
├── js/
└── scss/
```

``scss/`` ve ``js/`` CSS ve JavaScript'imizin kaynak kodudur. ``dist/``Klasör, yukarıdaki önceden derlenmiş indirme bölümünde listelenen her şeyi içerir . ``site/docs/`` Klasörü, belgelerimizin ve kaynak kodunu,  ``examples/`` klasörü de Bootstrap'in kullanımını içerir. Bunun ötesinde, dahil edilen diğer herhangi bir dosya, paketler, lisans bilgileri ve geliştirme için destek sağlar.


#Tarayıcılar ve Cihazlar
Her biri için bilinen tuhaflıklar ve hatalar dahil olmak üzere Bootstrap tarafından desteklenen modernden eskiye tüm tarayıcılar ve cihazlar hakkında bilgi edinin.


##Desteklenen tarayıcılar
Bootstrap , tüm büyük tarayıcıların ve platformların en son, kararlı sürümlerini destekler.

Doğrudan veya platformun web görünümü API'si aracılığıyla WebKit, Blink veya Gecko'nun en son sürümünü kullanan alternatif tarayıcılar açıkça desteklenmez. Ancak, Bootstrap (çoğu durumda) bu tarayıcılarda da düzgün şekilde görüntülenmeli ve çalışmalıdır. Daha spesifik destek bilgileri aşağıda verilmiştir.

Desteklenen tarayıcı yelpazemizi ve sürümlerini şurada bulabilirsiniz.[browserslistrc file ](https://github.com/twbs/bootstrap/blob/v5.2.0/.browserslistrc)

```sh
# https://github.com/browserslist/browserslist#readme


>= 0.5%
last 2 major versions
not dead
Chrome >= 60
Firefox >= 60
Firefox ESR
iOS >= 12
Safari >= 12
not Explorer <= 11

```

Bu tarayıcı sürümlerini yönetmek için [Browserslist](https://github.com/browserslist/browserslist)'i kullanan CSS önekleri aracılığıyla amaçlanan tarayıcı desteğini işlemek için Autoprefixer kullanıyoruz. Bu araçları projelerinize nasıl entegre edeceğiniz konusunda belgelerine bakın.

###Mobil cihazlar
Genel olarak konuşursak, Bootstrap her büyük platformun varsayılan tarayıcılarının en son sürümlerini destekler. Proxy tarayıcılarının (Opera Mini, Opera Mobile'ın Turbo modu, UC Tarayıcı Mini, Amazon Silk gibi) desteklenmediğini unutmayın.

| | Chrome | Firefox | Safari | Android Browser &amp; WebView |
| --- | --- | --- | --- | --- |
| **Android** | Supported | Supported | <span class="text-muted">&mdash;</span> | v6.0+ |
| **Windows** | Supported | Supported | Supported | <span class="text-muted">&mdash;</span> |

###Masaüstü tarayıcılar

Benzer şekilde, çoğu masaüstü tarayıcısının en son sürümleri desteklenir.

| | Chrome | Firefox | Microsoft Edge | Opera | Safari |
| --- | --- | --- | --- | --- | --- |
| **Mac** | Supported | Supported | Supported | Supported | Supported |
| **Windows** | Supported | Supported | Supported | Supported | <span class="text-muted">&mdash;</span> |

Firefox için, en son normal kararlı sürüme ek olarak, Firefox'un en son [Genişletilmiş Destek Sürümü (ESR)](https://www.mozilla.org/en-US/firefox/enterprise/) sürümünü de destekliyoruz.

Resmi olmayan bir şekilde, Bootstrap, resmi olarak desteklenmese de Linux için Chromium ve Chrome'da ve Linux için Firefox'ta yeterince iyi görünmeli ve davranmalıdır.

###Internet Explorer

Internet Explorer desteklenmiyor. **Internet Explorer desteğine ihtiyacınız varsa lütfen Bootstrap v4'ü kullanın.**

##Mobil cihazlarda modlar ve açılır menüler 
(Modals and dropdowns on mobile)

###Taşma ve kaydırma(Overflow and scrolling)

Öğe için destek overflow: hidden;, ``<body>``iOS ve Android'de oldukça sınırlıdır. Bu amaçla, bu cihazların tarayıcılarından herhangi birinde bir modalın üstünü veya altını geçtiğinizde ``<body>``içerik kaymaya başlar. Bkz. Chrome hatası #175502 (Chrome v40'ta düzeltildi) ve [WebKit hatası #153852](https://bugs.webkit.org/show_bug.cgi?id=153856) .

###iOS metin alanları ve kaydırma

iOS 9.2'den itibaren, bir kip açıkken, bir kaydırma hareketinin ilk dokunuşu bir metinsel ``<input>``veya a sınırı içindeyse, kipin kendisi yerine kipin altındaki içerik kaydırılacaktır ``<textarea>``. WebKit hatası #153856'ya ``<body>`` bakın .

###Gezinme Çubuğu Açılır Listeleri

Öğe , .dropdown-backdropz-indekslemenin karmaşıklığı nedeniyle gezinmede iOS'ta kullanılmaz. Bu nedenle, gezinme çubuklarındaki açılır listeleri kapatmak için, doğrudan açılır öğeye ([veya iOS'ta bir tıklama olayını başlatacak herhangi bir başka öğeye](https://developer.mozilla.org/en-US/docs/Web/API/Element/click_event#Safari_Mobile) ) tıklamanız gerekir.

###Tarayıcı yakınlaştırma

Sayfa yakınlaştırma, kaçınılmaz olarak hem Bootstrap'ta hem de web'in geri kalanında bazı bileşenlerde görüntü oluşturma kusurları sunar. Soruna bağlı olarak, sorunu çözebiliriz (önce arama yapın ve gerekirse bir sorun açın). Ancak, genellikle geçici çözümlerden başka doğrudan bir çözümleri olmadığı için bunları görmezden gelme eğilimindeyiz.

###Doğrulayıcılar

Bootstrap, eski ve sorunlu tarayıcılara mümkün olan en iyi deneyimi sağlamak için, tarayıcılardaki hataları gidermek için belirli tarayıcı sürümlerine özel CSS'yi hedeflemek için çeşitli yerlerde [CSS tarayıcı hack'lerini](http://browserhacks.com/) kullanır. Bu saldırılar anlaşılır bir şekilde CSS doğrulayıcılarının geçersiz olduklarından şikayet etmelerine neden olur. Birkaç yerde, henüz tam olarak standartlaştırılmamış son teknoloji CSS özelliklerini de kullanıyoruz, ancak bunlar yalnızca aşamalı geliştirme için kullanılıyor.
Bu doğrulama uyarıları, CSS'mizin korsan olmayan kısmı tam olarak doğrulandığından ve hileli kısımlar, korsan olmayan kısmın düzgün çalışmasına müdahale etmediğinden pratikte önemli değildir, bu nedenle bu özel uyarıları kasten görmezden gelmemizin nedeni budur.
HTML belgelerimiz de benzer şekilde, belirli bir Firefox hatası için bir geçici çözüm eklediğimiz için bazı önemsiz ve önemsiz HTML doğrulama uyarılarına sahiptir .


#JavaScript
İsteğe bağlı JavaScript eklentilerimizle Bootstrap'a hayat verin. Her bir eklenti, verilerimiz ve programatik API seçeneklerimiz ve daha fazlası hakkında bilgi edinin.


##Bireysel veya derlenmiş

Eklentiler tek tek dahil edilebilir (Bootstrap'in bireysel ``js/dist/*.js`` dosyasını kullanarak) veya tümü aynı anda ``bootstrap.js`` veya küçültülmüş olarak ``bootstrap.min.js``(her ikisini birden dahil etmeyin) dahil edilebilir.
Bir paketleyici (Webpack, Parsel, Vite…) kullanıyorsanız, UMD'ye hazır ``/js/dist/*.js `` dosyaları kullanabilirsiniz .

##JavaScript çerçeveleriyle kullanım

Bootstrap CSS herhangi bir çerçeve ile kullanılabilirken ,  DOM hakkında tam bilgi sahibi olduğunu varsayan **Bootstrap JavaScript, React, Vue ve Angular gibi JavaScript çerçeveleriyle tam uyumlu değildir** . Hem Bootstrap hem de çerçeve aynı DOM öğesini mutasyona uğratmaya çalışabilir ve bu da "açık" konumda takılı kalan açılır listeler gibi hatalara neden olabilir.

Bu tür çerçeveleri kullananlar için daha iyi bir alternatif , Bootstrap JavaScript **yerine** çerçeveye özel bir paket kullanmaktır. İşte en popüler seçeneklerden bazıları:

* React: [React Bootstrap](https://react-bootstrap.github.io/)
* Vue: [BootstrapVue](https://bootstrap-vue.org/) (şu anda yalnızca Vue 2 ve Bootstrap 4'ü destekler)
* Açısal: [ng-önyükleme](https://ng-bootstrap.github.io/)
  
##Bootstrap'i modül olarak kullanma

>**Kendin dene!** Bootstrap'i ES modülü olarak kullanmak için kaynak kodunu ve çalışma demosunu [twbs/examples deposundan](https://github.com/twbs/examples/tree/main/sass-js-esm) indirin . Ayrıca örneği [StackBlitz'de de açabilirsiniz](https://stackblitz.com/github/twbs/examples/tree/main/sass-js-esm?file=index.html) .

[Hedeflenen tarayıcılarınız destekliyorsa](https://caniuse.com/es6-module) , Bootstrap'i tarayıcıda bir modül olarak kullanmanıza izin veren ``ESM( bootstrap.esm.js ve .bootstrap.esm.min.js)`` olarak oluşturulmuş bir Bootstrap sürümü sunuyoruz. 

```
<script type="module">
  import { Toast } from 'bootstrap.esm.min.js'


  Array.from(document.querySelectorAll('.toast'))
    .forEach(toastNode => new Toast(toastNode))
</script>
```

JS paketleyicileri ile karşılaştırıldığında, tarayıcıda ESM kullanmak, modül adı yerine tam yolu ve dosya adını kullanmanızı gerektirir. [Tarayıcıda JS modülleri hakkında daha fazlasını okuyun.](https://v8.dev/features/modules#specifiers) Bu yüzden yukarıdaki 'bootstrap' yerine 'bootstrap.esm.min.js' kullanıyoruz. Bununla birlikte, Popper'ı JavaScript'imize şu şekilde içe aktaran Popper bağımlılığımız nedeniyle bu daha da karmaşık hale gelir:

``import * as Popper from "@popperjs/core"``


Bunu olduğu gibi denerseniz, konsolda aşağıdakine benzer bir hata görürsünüz:

``Uncaught TypeError: Failed to resolve module specifier "@popperjs/core". Relative references must start with either "/", "./", or "../".``

İsteğe bağlı modül adlarını çözmek ve yolları tamamlamak için  ``importmap`` kullanabilirsiniz. [Hedeflenen tarayıcılarınız](https://caniuse.com/?search=importmap) ``importmap`` desteklemiyorsa , [es-module-shims](https://github.com/guybedford/es-module-shims) projesini  kullanmanız gerekecektir . Bootstrap ve Popper için şu şekilde çalışır:

```<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
   <title>Hello, modularity!</title>
 </head>
 <body>
   <h1>Hello, modularity!</h1>
   <button id="popoverButton" type="button" class="btn btn-primary btn-lg" class="btn btn-lg btn-danger" data-bs-toggle="popover" title="ESM in Browser" data-bs-content="Bang!">Custom popover</button>

   <script async src="https://cdn.jsdelivr.net/npm/es-module-shims@1/dist/es-module-shims.min.js" crossorigin="anonymous"></script>
   <script type="importmap">
   
   {
     "imports": {
       "@popperjs/core": "https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.5/dist/umd/popper.min.js",
       "bootstrap": "https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.esm.min.js"
     }
   }
   </script>
   <script type="module">
     import * as bootstrap from 'bootstrap'

     new bootstrap.Popover(document.getElementById('popoverButton'))
   </script>
 </body>
</html>
```

##Bağımlılıklar
Bazı eklentiler ve CSS bileşenleri diğer eklentilere bağlıdır. Eklentileri tek tek eklerseniz, bu bağımlılıkları belgelerde kontrol ettiğinizden emin olun.

Açılır listelerimiz, açılır pencerelerimiz ve araç ipuçlarımız da [Popper](https://popper.js.org/)'a bağlıdır .

##Veri Öznitelikleri
Hemen hemen tüm Bootstrap eklentileri, veri öznitelikleri ile yalnızca HTML aracılığıyla etkinleştirilebilir ve yapılandırılabilir (tercih ettiğimiz JavaScript işlevselliğini kullanma yöntemimiz). **Tek bir öğe üzerinde yalnızca bir dizi veri özniteliği kullandığınızdan emin olun** (örneğin, aynı düğmeden bir  ipucu aracını ve modu tetikleyemezsiniz.)

Seçenekler veri öznitelikleri veya JavaScript aracılığıyla iletilebildiğinden, ``data-bs-animation="{value}"`` örneğinde olduğu gibi ``data-bs-`` öğesine bir seçenek  adı ekleyebilirsiniz. Seçenekler veri öznitelikleri aracılığıyla aktarılırken seçenek adının durum tipini “ camelCase ”den “ kebab-case ” olarak değiştirdiğinizden emin olun. Örneğin, ``data-bs-customClass="beautifier"` yerine ```data-bs-custom-class="beautifier"``kullanın .

Bootstrap 5.2.0'dan itibaren, tüm bileşenler , bir JSON dizesi olarak basit bileşen yapılandırmasını barındırabilen **deneysel** bir ayrılmış veri özniteliği ``data-bs-config`` destekler. Bir öğe ``data-bs-config='{"delay":0, "title":123}'`` ve ``data-bs-title="456"`` özniteliklere sahip olduğunda, nihai ``title`` değer ``456`` olacak ve ayrı veri öznitelikleri ``data-bs-config.`` üzerinde verilen değerleri geçersiz kılar.  Ek olarak, mevcut veri öznitelikleri, ``data-bs-delay='{"show":0,"hide":150}'`` gibi JSON değerlerini barındırabilir .

##Seçiciler
Performans nedenleriyle DOM öğelerini sorgulamak için yerel querySelector ve ``.querySelectorAll`` yöntemlerini kullanıyoruz, bu nedenle [geçerli seçiciler](https://www.w3.org/TR/CSS21/syndata.html#value-def-identifier) kullanmanız gerekir . Eğer ``collapse:Example`` gibi özel seçiciler kullanıyorsanız , bunlardan kaçındığınızdan emin olun

##Olaylar
Bootstrap, çoğu eklentinin benzersiz eylemleri için özel etkinlikler sağlar. Genellikle bunlar (belirli bir özneyi ya da zamana bağlayan bir çekim olmaksızın) fiilin temel biçimi (mastar) ve [geçmiş ortaç](https://tr.wiktionary.org/wiki/past_participle) biçiminde gelir - 
burada mastar (örn. show) bir olayın başlangıcında tetiklenir ve geçmiş ortaç biçimi (örn. shown) bir eylemin tamamlanmasıyla tetiklenir.

Tüm mastar olayları ``preventDefault()`` işlevsellik sağlar. Bu, bir eylemin yürütülmesini başlamadan önce durdurma yeteneği sağlar. Bir olay işleyicisinden ``false`` döndürmek de otomatik olarak ``preventDefault()`` öğesini çağırır.

```js
const myModal = document.querySelector('#myModal')

myModal.addEventListener('show.bs.modal', event => {
 if (!data) {
   return event.preventDefault() // stops modal from being shown
 }
})
```	

##Programatik API
Tüm yapıcılar isteğe bağlı bir seçenekler nesnesini kabul eder veya hiçbir şey kabul etmez (bu, bir eklentiyi varsayılan davranışıyla başlatır):

```js
const myModalEl = document.querySelector('#myModal')

const modal = new bootstrap.Modal(myModalEl) // initialized with defaults

const configObject = { keyboard: false }
const modal1 = new bootstrap.Modal(myModalEl, configObject) // initialized with no keyboard
```

Belirli bir eklenti örneği almak istiyorsanız, her eklenti bir ``getInstance`` yöntem sunar. Örneğin, bir örneği doğrudan bir öğeden almak için:

``bootstrap.Popover.getInstance(myPopoverEl)``


Bu yöntem, istenen öğe üzerinden bir örnek başlatılmazsa null döndürür.

Alternatif olarak, ``getOrCreateInstance`` bir DOM öğesiyle ilişkili örneği almak veya başlatılmamış olması durumunda yeni bir tane oluşturmak için kullanılabilir.

```js
bootstrap.Popover.getOrCreateInstance(myPopoverEl, configObject)
```
	

Bir örneğin başlatılmamış olması durumunda, ikinci argüman olarak isteğe bağlı bir yapılandırma nesnesini kabul edebilir ve kullanabilir.

##Yapıcılarda CSS seçicileri

``getInstance`` ve yöntemlerine ek olarak , tüm eklenti oluşturucuları ilk argüman olarak ``getOrCreateInstance`` bir DOM öğesini veya geçerli bir [CSS seçicisini](https://getbootstrap.com/docs/5.2/getting-started/javascript/#selectors) kabul edebilir. ``querySelector ``Eklentilerimiz yalnızca tek bir öğeyi desteklediğinden , bu yöntemle eklenti öğeleri bulunur .

```js
const modal = new bootstrap.Modal('#myModal')
const dropdown = new bootstrap.Dropdown('[data-bs-toggle="dropdown"]')
const offcanvas = bootstrap.Offcanvas.getInstance('#myOffcanvas')
const alert = bootstrap.Alert.getOrCreateInstance('#myAlert')
```

##Asenkron fonksiyonlar ve geçişler

Tüm programatik API yöntemleri zaman uyumsuzdur ve geçiş başlatıldığında, ancak bitmeden önce arayana geri döner . Geçiş tamamlandıktan sonra bir eylemi gerçekleştirmek için ilgili olayı dinleyebilirsiniz.

```js
const myCollapseEl = document.querySelector('#myCollapse')

myCollapseEl.addEventListener('shown.bs.collapse', event => {
 // Action to execute once the collapsible area is expanded
})
```

Ek olarak, geçiş yapan bir bileşen üzerindeki bir **yöntem çağrısı yok sayılacaktır** .

```js
const myCarouselEl = document.querySelector('#myCarousel')
const carousel = bootstrap.Carousel.getInstance(myCarouselEl) // Retrieve a Carousel instance

myCarouselEl.addEventListener('slid.bs.carousel', event => {
 carousel.to('2') // Will slide to the slide 2 as soon as the transition to slide 1 is finished
})

carousel.to('1') // Will start sliding to the slide 1 and returns to the caller
carousel.to('2') // !! Will be ignored, as the transition to the slide 1 is not finished !!
```	

##Dispose yöntemi

dispose Yöntemi hemen sonrasında kullanmak doğru gibi görünse hide()de yanlış sonuçlara yol açacaktır. İşte problem kullanımına bir örnek:

```js
const myModal = document.querySelector('#myModal')
myModal.hide() // it is asynchronous

myModal.addEventListener('shown.bs.hidden', event => {
  myModal.dispose()
})
```

	

##Varsayılan ayarları
Eklentinin ``Constructor.Default`` nesnesini değiştirerek bir eklentinin varsayılan ayarlarını değiştirebilirsiniz:

```js
// changes default for the modal plugin's `keyboard` option to false
bootstrap.Modal.Default.keyboard = false
```


##Yöntemler ve özellikler
Her Bootstrap eklentisi, aşağıdaki yöntemleri ve statik özellikleri ortaya çıkarır.

| Yöntem | Tanım |
| --- | --- |
| `dispose` | Bir elemanın kipini yok eder. (DOM öğesinde depolanan verileri kaldırır) |
| `getInstance` | Bir DOM öğesiyle ilişkili mod örneğini almanızı sağlayan *statik* yöntem. |
| `getOrCreateInstance` | ir DOM öğesiyle ilişkili mod örneğini almanıza veya başlatılmamış olması durumunda yeni bir tane oluşturmanıza izin veren statik yöntem.|

| Statik özellik | Tanım |
| --- | --- |
| `NAME`  | Eklenti adını döndürür. (Örnek: bootstrap.Tooltip.NAME) |
| `VERSION`  | VERSIONBootstrap eklentilerinin her birinin sürümüne , eklentinin kurucusunun özelliği aracılığıyla erişilebilir (Örnek: bootstrap.Tooltip.VERSION) |

## Sanitizer
Araç ipuçları ve Popover'lar, HTML'yi kabul eden seçenekleri sterilize etmek için yerleşik Sanitizer kullanır.

Varsayılan ``allowList`` değer aşağıdaki gibidir:

```js
const ARIA_ATTRIBUTE_PATTERN = /^aria-[\w-]*$/i
const DefaultAllowlist = {
// Global attributes allowed on any supplied element below.
'*': ['class', 'dir', 'id', 'lang', 'role', ARIA_ATTRIBUTE_PATTERN],
a: ['target', 'href', 'title', 'rel'],
area: [],
b: [],
br: [],
col: [],
code: [],
div: [],
em: [],
hr: [],
h1: [],
h2: [],
h3: [],
h4: [],
h5: [],
h6: [],
i: [],
img: ['src', 'srcset', 'alt', 'title', 'width', 'height'],
li: [],
ol: [],
p: [],
pre: [],
s: [],
small: [],
span: [],
sub: [],
sup: [],
strong: [],
u: [],
ul: []
}
```

Bu varsayılan izin listesine yeni değerler eklemek istiyorsanız aşağıdakileri yapabilirsiniz:

```js
const myDefaultAllowList = bootstrap.Tooltip.Default.allowList

// To allow table elements
myDefaultAllowList.table = []

// To allow td elements and data-bs-option attributes on td elements
myDefaultAllowList.td = ['data-bs-option']

// You can push your custom regex to validate your attributes.
// Be careful about your regular expressions being too lax
const myCustomRegex = /^data-my-app-[\w-]+/
myDefaultAllowList['*'].push(myCustomRegex)
```


DOMPurify gibi özel bir kitaplık kullanmayı tercih ettiğiniz için sanitizeri atlamak istiyorsanız , aşağıdakileri yapmalısınız:

```js
const yourTooltipEl = document.querySelector('#yourTooltip')
const tooltip = new bootstrap.Tooltip(yourTooltipEl, {
  sanitizeFn(content) {
    return DOMPurify.sanitize(content)
  }
})
```

	

İsteğe bağlı olarak jQuery kullanarak

**Bootstrap 5'te jQuery'ye ihtiyacınız yok **, ancak bileşenlerimizi jQuery ile kullanmak hala mümkün. Bootstrap nesnede algılarsa jQuery, window tüm bileşenlerimizi jQuery'nin eklenti sistemine ekler. Bu, aşağıdakileri yapmanızı sağlar:

```js
$('[data-bs-toggle="tooltip"]').tooltip() // to enable tooltips, with default configuration

$('[data-bs-toggle="tooltip"]').tooltip({ boundary: 'clippingParents', customClass: 'myClass' }) // to initialize tooltips with given configuration

$('#myTooltip').tooltip('show') // to trigger `show` method
```


Aynı şey diğer bileşenlerimiz için de geçerli.

### No conflict
Bazen Bootstrap eklentilerini diğer UI çerçeveleriyle birlikte kullanmak gerekir. Bu durumlarda, zaman zaman ad alanı çakışmaları meydana gelebilir. Böyle bir durumda, .noConflictdeğerini geri almak istediğiniz eklentiyi arayabilirsiniz.

```js
const bootstrapButton = $.fn.button.noConflict() // return $.fn.button to previously assigned value
$.fn.bootstrapBtn = bootstrapButton // give $().bootstrapBtn the Bootstrap functionality
```

Bootstrap, Prototype veya jQuery UI gibi üçüncü taraf JavaScript kitaplıklarını resmi olarak desteklemez. Ad alanlı olaylara rağmen .noConflict, kendi başınıza düzeltmeniz gereken uyumluluk sorunları olabilir.

###jQuery olayları
Bootstrap, ``window`` nesnesinde ``jQuery`` varsa ve ``<body>`` üzerinde ayarlanmış ``data-bs-no-jquery`` özniteliği yoksa ``jQuery``'yi algılar. jQuery bulunursa, Bootstrap, jQuery'nin olay sistemi sayesinde olayları yayacaktır. Yani Bootstrap olaylarını görmek istiyorsanız,``addEventListener`` yerine jQuery yöntemlerini ( ``.on, .one``) kullanmak zorunda kalacaksınız 

```js
$('#myTab a').on('shown.bs.tab', () => {
  // do something...
})
```


##Devre Dışı JavaScript

JavaScript devre dışı bırakıldığında Bootstrap eklentilerinin özel bir geri dönüşü yoktur. Bu durumda kullanıcı deneyimini önemsiyorsanız ``<noscript>``, durumu (ve JavaScript'in nasıl yeniden etkinleştirileceğini) kullanıcılarınıza açıklamak ve/veya kendi özel yedeklerinizi eklemek için kullanın.

##Bootstrap ve Web Paketi

Webpack kullanarak Bootstrap'in CSS ve JavaScript'ini projenize nasıl dahil edeceğinize ve paketleyeceğinize dair resmi kılavuz.

## Kurulum

Bootstrap ile sıfırdan bir Webpack projesi oluşturuyoruz, bu nedenle gerçekten başlayabilmemiz için bazı önkoşullar ve ön adımlar var. Bu kılavuz, Node.js'nin kurulu olmasını ve terminal hakkında biraz bilgi sahibi olmanızı gerektirir.

1. **Bir proje klasörü oluşturun ve npm'yi kurun.** Klasörü oluşturacağız ve bize tüm etkileşimli soruları sormasını önlemek my-project için -y argümanla npm'yi başlatacağız .

```sh
mkdir my-project && cd my-project
npm init -y
```	

2. **Webpack'i yükleyin.** Daha sonra Webpack geliştirme bağımlılıklarımızı kurmamız gerekiyor: ``webpack`` Webpack'in çekirdeği için, ``webpack-cli ``böylece Webpack komutlarını terminalden çalıştırabiliriz ``webpack-dev-server``  ve böylece yerel bir geliştirme sunucusu çalıştırabiliriz. Bu --save-dev bağımlılıkların yalnızca geliştirme kullanımı için olduğunu ve üretim için olmadığını belirtmek için kullanıyoruz.

```
npm i --save-dev webpack webpack-cli webpack-dev-server
```	

3. **Bootstrap'i yükleyin.** Artık Bootstrap'i kurabiliriz. Açılır listelerimiz, açılır pencerelerimiz ve araç ipuçlarımız, konumları için ona bağlı olduğundan, Popper'ı da kuracağız. Bu bileşenleri kullanmayı düşünmüyorsanız, burada Popper'ı atlayabilirsiniz.
```sh
npm i --save bootstrap @popperjs/core
```	

4. **Ek bağımlılıklar yükleyin.** Webpack ve Bootstrap'a ek olarak, Bootstrap'in CSS ve JS'sini Webpack ile düzgün bir şekilde içe aktarmak ve paketlemek için birkaç bağımlılığa daha ihtiyacımız var. Bunlar arasında Sass, bazı yükleyiciler ve Autoprefixer bulunur.

```sh  
npm i --save-dev autoprefixer css-loader postcss-loader sass sass-loader style-loader
```

Artık gerekli tüm bağımlılıkları yüklediğimize göre, proje dosyalarını oluşturmaya ve Bootstrap'i içe aktarmaya başlayabiliriz.

## Proje Yapısı
Klasörü zaten oluşturduk my-project ve npm'yi başlattık. Şimdi proje yapısını tamamlamak için ``src`` ve klasörlerimizi de oluşturacağız. Aşağıdakileri ``dist``'den çalıştırın my-project veya aşağıda gösterilen klasör ve dosya yapısını manuel olarak oluşturun.

```sh
mkdir {dist,src,src/js,src/scss}
touch dist/index.html src/js/main.js src/scss/styles.scss webpack.config.js
```	

İşiniz bittiğinde, projenizin tamamı şöyle görünmelidir:


```
my-project/
├── dist/
│   └── index.html
├── src/
│   ├── js/
│   │   └── main.js
│   └── scss/
│       └── styles.scss
├── package-lock.json
├── package.json
└── webpack.config.js
```	

Bu noktada, her şey doğru yerde, ancak Webpack çalışmayacak çünkü henüz ``webpack.config.js.``'yi doldurmadık. 

##Web Paketini Yapılandır
Bağımlılıklar yüklendiğinde ve proje klasörümüz kodlamaya başlamamız için hazır olduğunda, artık Webpack'i yapılandırabilir ve projemizi yerel olarak çalıştırabiliriz.

1. Editörünüzde **webpack.config.js** açın. Boş olduğu için, sunucumuzu başlatabilmemiz için ona bazı ortak kalıp yapılandırması eklememiz gerekecek. Yapılandırmanın bu kısmı, Webpack'e projemizin JavaScript'ini, derlenmiş kodun nereye ( dist) çıktısını alacağını ve geliştirme sunucusunun nasıl davranması gerektiğini ( dist hot reload ile klasörden çekerek) aramasını söyler.

```sh
const path = require('path')

module.exports = {
 entry: './src/js/main.js',
 output: {
   filename: 'main.js',
   path: path.resolve(__dirname, 'dist')
 },
 devServer: {
   static: path.resolve(__dirname, 'dist'),
   port: 8080,
   hot: true
 }
}
```

2. Daha sonra ``dist/index.html`` dolduruyoruz  Bu, Web paketinin, daha sonraki adımlarda ekleyeceğimiz birlikte verilen CSS ve JS'yi kullanmak için tarayıcıya yükleyeceği HTML sayfasıdır. Bunu yapmadan önce, bir önceki adımdaki JS'yi oluşturması ve dahil etmesi için ona bir ``output`` vermeliyiz .

```sh
<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Bootstrap w/ Webpack</title>
 </head>
 <body>
   <div class="container py-4 px-3 mx-auto">
     <h1>Hello, Bootstrap and Webpack!</h1>
     <button class="btn btn-primary">Primary button</button>
   </div>
   <script src="./main.js"></script>
 </body>
</html>
```	

Bootstrap'ın CSS'sinin Webpack tarafından ne zaman yüklendiğini görebilmemiz için ``div class="container"`` ve ``<button>``ile birlikte buraya biraz Bootstrap stili ekliyoruz.

3. **Şimdi Webpack'i çalıştırmak için bir ``npm`` betiğine ihtiyacımız var.** Aşağıda gösterilen komut dosyasını açın ``package.json`` ve ``start`` ekleyin (test komut dosyasına zaten sahip olmalısınız). Yerel Webpack dev sunucumuzu başlatmak için bu betiği kullanacağız.

```sh
{
 // ...
 "scripts": {
   "start": "webpack serve --mode development",
   "test": "echo \"Error: no test specified\" && exit 1"
 },
 // ...
}
```

4. **Ve son olarak, Webpack'i başlatabiliriz**. my-project klasörden Terminalinizdeki yeni eklenen npm komut dosyasını çalıştırın :

```sh   
$ npm start
```
![webpack çalışıyor](https://getbootstrap.com/docs/5.2/assets/img/guides/webpack-dev-server.png)

Bu kılavuzun sonraki ve son bölümünde, Webpack yükleyicilerini ayarlayacağız ve tüm Bootstrap CSS ve JavaScript'lerini içe aktaracağız.

## Boostrap'ı İçeaktar

Bootstrap'i Webpack'e içe aktarmak, ilk bölümde kurduğumuz yükleyicileri gerektirir. Bunları npm ile kurduk, ancak şimdi Webpack'in bunları kullanacak şekilde yapılandırılması gerekiyor.

1. **Yükleyicileri** ``webpack.config.js``'de ayarlayın. Yapılandırma dosyanız şimdi tamamlandı ve aşağıdaki kod parçasıyla eşleşmelidir. Buradaki tek yeni kısım ``module`` bölümü.

```js
const path = require('path')

module.exports = {
 entry: './src/js/main.js',
 output: {
   filename: 'main.js',
   path: path.resolve(__dirname, 'dist')
 },
 devServer: {
   static: path.resolve(__dirname, 'dist'),
   port: 8080,
   hot: true
 },
 module: {
   rules: [
     {
       test: /\.(scss)$/,
       use: [
         {
           loader: 'style-loader'
         },
         {
           loader: 'css-loader'
         },
         {
           loader: 'postcss-loader',
           options: {
             postcssOptions: {
               plugins: () => [
                 require('autoprefixer')
               ]
             }
           }
         },
         {
           loader: 'sass-loader'
         }
       ]
     }
   ]
 }
}	

```

İşte tüm bu yükleyicilere neden ihtiyacımız olduğunun bir özeti. style-loader, CSS'yi HTML sayfasının ``<head>`` bölümündeki bir ``<style>`` öğesine enjekte eder, ``css-loader`` ``@import`` ve ``url()`` kullanımına yardımcı olur, Autoprefixer için ``postcss-loader`` gereklidir ve ``sass-loader`` Sass kullanmamıza izin verir.

```
<style><head>css-loader@importurl()postcss-loadersass-loader
```	

1. **Şimdi Bootstrap'ın CSS'sini içe aktaralım.** ``src/scss/styles.scss`` Bootstrap'in tüm kaynak Sass'larını içe aktarmak için aşağıdakini ekleyin.

```sh
// Import all of Bootstrap's CSS
@import "~bootstrap/scss/bootstrap";
```	

İsterseniz stil sayfalarımızı tek tek de içe aktarabilirsiniz. Ayrıntılar için Sass içe aktarma [belgelerimizi okuyun ](https://getbootstrap.com/docs/5.2/customize/sass/#importing).

3. **Ardından CSS'yi yüklüyoruz ve Bootstrap'ın JavaScript'ini içe aktarıyoruz.** CSS'yi yüklemek ve tüm Bootstrap JS'lerini içe aktarmak için aşağıdakileri ekleyin ``src/js/main.js`` . Popper, Bootstrap aracılığıyla otomatik olarak içe aktarılacaktır.


```sh
// Import our custom CSS
import '../scss/styles.scss'

// Import all of Bootstrap's JS
import * as bootstrap from 'bootstrap'
```

Paket boyutlarını düşük tutmak için JavaScript eklentilerini gerektiği gibi tek tek de içe aktarabilirsiniz:

```sh
import Alert from 'bootstrap/js/dist/alert'

// or, specify which plugins you need:
import { Tooltip, Toast, Popover } from 'bootstrap'
```	

Bootstrap eklentilerinin nasıl kullanılacağı hakkında daha fazla bilgi için [JavaScript belgelerimizi okuyun](https://getbootstrap.com/docs/5.2/getting-started/javascript/) .



4. Ve işin bitti! 🎉 Bootstrap'in kaynak Sass ve JS'si tamamen yüklendiğinde, yerel geliştirme sunucunuz artık böyle görünmelidir.
![Bootstrap ile çalışan Webpack dev sunucusu ](https://getbootstrap.com/docs/5.2/assets/img/guides/webpack-dev-server-bootstrap.png)




Artık kullanmak istediğiniz Bootstrap bileşenlerini eklemeye başlayabilirsiniz. Ek özel Sass'ı nasıl ekleyeceğiniz ve yapınızı yalnızca Bootstrap's CSS ve JS'nin ihtiyacınız olan kısımlarını içe aktararak nasıl optimize edeceğiniz konusunda eksiksiz Webpack örnek projesini kontrol ettiğinizden emin olun .


# Bootstrap & Parcel
Parcel kullanarak projenize Bootstrap'in CSS ve JavaScript'ini nasıl dahil edeceğinize ve paketleyeceğinize dair resmi kılavuz.

## Setup
Bootstrap ile sıfırdan bir Parsel projesi oluşturuyoruz, bu nedenle gerçekten başlayabilmemiz için bazı önkoşullar ve ön adımlar var. Bu kılavuz, Node.js'nin kurulu olmasını ve terminal hakkında biraz bilgi sahibi olmanızı gerektirir.

1. ``Bir proje klasörü oluşturun ve npm'yi kurun.`` Klasörü oluşturacağız ve bize tüm etkileşimli soruları sormasını önlemek my-project için -y argümanla npm'yi başlatacağız .

```sh
mkdir my-project && cd my-project
npm init -y
```

2.** Parsel yükleyin.** Web paketi klavuzumuzun aksine, burada yalnızca tek bir oluşturma aracı bağımlılığı vardır. Parsel, dil dönüştürücülerini (Sass gibi) algıladıkça otomatik olarak kuracaktır. Bu ``--save-dev`` bağımlılığın yalnızca geliştirme amaçlı olduğunu ve üretim için olmadığını belirtmek için kullanıyoruz.

```sh
npm i --save-dev parcel
```	

3. **Bootstrap'i yükleyin.** Artık Bootstrap'i kurabiliriz. Açılır listelerimiz, açılır pencerelerimiz ve araç ipuçlarımız, konumları için ona bağlı olduğundan, Popper'ı da kuracağız. Bu bileşenleri kullanmayı düşünmüyorsanız, burada Popper'ı atlayabilirsiniz.

```sh
npm i --save bootstrap @popperjs/core
```	

Artık gerekli tüm bağımlılıkları yüklediğimize göre, proje dosyalarını oluşturmaya ve Bootstrap'i içe aktarmaya başlayabiliriz.

## Proje Yapısı
Klasörü zaten oluşturduk my-project ve npm'yi başlattık. Şimdi ``src`` proje yapısını tamamlamak için klasörümüzü, stil sayfamızı ve JavaScript dosyamızı da oluşturacağız. Aşağıdakileri ``my-project``'den çalıştırın  veya aşağıda gösterilen klasör ve dosya yapısını manuel olarak oluşturun.

```sh
mkdir {src,src/js,src/scss}
touch src/index.html src/js/main.js src/scss/styles.scss
```	

İşiniz bittiğinde, projenizin tamamı şöyle görünmelidir:

``my-project``
my-project/
├── src/
│   ├── js/
│   │   └── main.js
│   ├── scss/
│   │   └── styles.scss
│   └── index.html
├── package-lock.json
└── package.json
``my-project``	

Bu noktada her şey doğru yerde ancak Parcel sunucumuzu başlatmak için bir HTML sayfasına ve npm betiğine ihtiyaç duyuyor.

## Parsel Yapılandır
Bağımlılıklar kurulu ve proje klasörümüz kodlamaya başlamamız için hazır, artık Parsel'i yapılandırabilir ve projemizi yerel olarak çalıştırabiliriz. Parselin kendisi tasarım gereği yapılandırma dosyası gerektirmez, ancak sunucumuzu başlatmak için bir npm komut dosyasına ve bir HTML dosyasına ihtiyacımız var.

1. **src/index.html dosyasını doldurun.** Parselin oluşturulacak bir sayfaya ihtiyacı var, bu nedenle index.html sayfamızı CSS ve JavaScript dosyalarımız dahil bazı temel HTML'yi ayarlamak için kullanıyoruz.

```sh
<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Bootstrap w/ Parcel</title>
   <link rel="stylesheet" href="scss/styles.scss">
   <script type="module" src="js/main.js"></script>
 </head>
 <body>
   <div class="container py-4 px-3 mx-auto">
     <h1>Hello, Bootstrap and Parcel!</h1>
     <button class="btn btn-primary">Primary button</button>
   </div>
 </body>
</html>
```	

Bootstrap'ın CSS'sinin Webpack tarafından ne zaman yüklendiğini görebilmemiz için ``div class="container`` ve  ``<button>`` ile birlikte buraya biraz Bootstrap stili ekliyoruz.

Parsel, Sass kullandığımızı otomatik olarak algılayacak ve bunu desteklemek için ``Sass Parcel ``eklentisini yükleyecektir.  Ancak dilerseniz manuel olarak da çalıştırabilirsiniz 

```sh
$ npm i --save-dev @parcel/transformer-sass.
```
2. **Parsel npm komut dosyalarını ekleyin.** Açın ``package.json`` ve aşağıdaki ``start`` betiği scripts nesneye ekleyin. Bu betiği Parsel geliştirme sunucumuzu başlatmak ve oluşturduğumuz HTML dosyasını ``dist`` dizine derlendikten sonra işlemek için kullanacağız.
   
```sh
{
  // ...
  "scripts": {
    "start": "parcel serve src/index.html --public-url / --dist-dir dist",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  // ...
}
```

1. **Ve son olarak, Parsel'i başlatabiliriz.** ``my-project`` klasörden terminalinizde ki yeni eklenen npm komut dosyasını çalıştırın :

```sh  
$ npm start
```
![Parsel geliştirme sunucusu çalışıyor ](https://getbootstrap.com/docs/5.2/assets/img/guides/parcel-dev-server.png)



Bu kılavuzun sonraki ve son bölümünde, Bootstrap'in tüm CSS ve JavaScript'lerini içe aktaracağız.

## Import Bootstrap # 
Bootstrap'i Parsel'e aktarmak için iki aktarma gerekli, biri``styles.scss``, diğeri de ``main.js``.

1. **Bootstrap'in CSS'sini içe aktarın.**  Bootstrap'in ``src/scss/styles.scss`` tüm kaynak Sass'larını içe aktarmak için aşağıdakini ekleyin .
   
```sh   
// Import all of Bootstrap's CSS
@import "~bootstrap/scss/bootstrap";
```	

İsterseniz stil sayfalarımızı tek tek de içe aktarabilirsiniz. Ayrıntılar için Sass içe aktarma belgelerimizi okuyun .

1. Bootstrap'in JS'sini içe aktarın. Tüm Bootstrap JS'lerini içe aktarmak için ``src/js/main.js`` aşağıdakini ekleyin . Popper, Bootstrap aracılığıyla otomatik olarak içe aktarılacaktır.

```sh
// Import all of Bootstrap's JS
import * as bootstrap from 'bootstrap'
```	

Paket boyutlarını düşük tutmak için JavaScript eklentilerini gerektiği gibi tek tek de içe aktarabilirsiniz:

```sh
import Alert from 'bootstrap/js/dist/alert'

// or, specify which plugins you need:
import { Tooltip, Toast, Popover } from 'bootstrap'
```	

Bootstrap eklentilerinin nasıl kullanılacağı hakkında daha fazla bilgi için JavaScript belgelerimizi okuyun .
  
3. Ve işin bitti! 🎉 Bootstrap'in kaynak Sass ve JS'si tamamen yüklendiğinde, yerel geliştirme sunucunuz artık böyle görünmelidir.

![Bootstrap ile çalışan Parsel dev sunucusu](https://getbootstrap.com/docs/5.2/assets/img/guides/parcel-dev-server-bootstrap.png) 

Artık kullanmak istediğiniz Bootstrap bileşenlerini eklemeye başlayabilirsiniz. Ek özel Sass'ı nasıl ekleyeceğiniz ve yapınızı yalnızca Bootstrap's CSS ve JS'nin ihtiyacınız olan kısımlarını içe aktararak optimize etmek için tam Parsel örnek projesini kontrol ettiğinizden emin olun .

# Boostrap & Vite
Vite kullanarak projenize Bootstrap'in CSS ve JavaScript'ini nasıl dahil edeceğinize ve paketleyeceğinize dair resmi kılavuz.

## Setup

Bootstrap ile sıfırdan bir Vite projesi oluşturuyoruz, bu nedenle gerçekten başlayabilmemiz için bazı önkoşullar ve ön adımlar var. Bu kılavuz, Node.js'nin kurulu olmasını ve terminal hakkında biraz bilgi sahibi olmanızı gerektirir.

1. **Bir proje klasörü oluşturun ve npm'yi kurun**. Klasörü oluşturacağız ve bize tüm etkileşimli soruları sormasını önlemek ``my-project için`` ``-y`` argümanıyla ``npm``'yi başlatacağız .

```sh
mkdir my-project && cd my-project
npm init -y
```

2. Vite'ı yükleyin. Web paketi kılavuzumuzun aksine, burada yalnızca tek bir oluşturma aracı bağımlılığı vardır. Bu --save-dev bağımlılığın yalnızca geliştirme amaçlı olduğunu ve üretim için olmadığını belirtmek için kullanıyoruz.

```sh
npm i --save-dev vite
```	

3. **Bootstrap'i yükleyin.** Artık Bootstrap'i kurabiliriz. Açılır listelerimiz, açılır pencerelerimiz ve araç ipuçlarımız, konumları için ona bağlı olduğundan, Popper'ı da kuracağız. Bu bileşenleri kullanmayı düşünmüyorsanız, burada Popper'ı atlayabilirsiniz.

```sh
npm i --save bootstrap @popperjs/core

```
4. **Ek bağımlılık yükleyin**. Vite ve Bootstrap'a ek olarak, Bootstrap'ın CSS'sini düzgün bir şekilde içe aktarmak ve paketlemek için başka bir bağımlılığa (Sass) ihtiyacımız var.

```
npm i --save-dev sass
```	

Artık gerekli tüm bağımlılıkları yüklediğimize ve ayarladığımıza göre, proje dosyalarını oluşturmaya ve Bootstrap'i içe aktarmaya başlayabiliriz.

## Proje Yapısı
Klasörü zaten oluşturduk. my-project ve npm'yi başlattık. Şimdi src proje yapısını tamamlamak için klasörümüzü, stil sayfamızı ve JavaScript dosyamızı da oluşturacağız. Aşağıdakileri ``my-project``'den çalıştırın veya aşağıda gösterilen klasör ve dosya yapısını manuel olarak oluşturun.

```sh
mkdir {src,src/js,src/scss}
touch src/index.html src/js/main.js src/scss/styles.scss vite.config.js

```	

İşiniz bittiğinde, projenizin tamamı şöyle görünmelidir:
```sh
my-project/
├── src/
│   ├── js/
│   │   └── main.js
│   └── scss/
│   |   └── styles.scss
|   └── index.html
├── package-lock.json
├── package.json
└── vite.config.js
```	

Bu noktada her şey doğru yerde ama Vite çalışmayacak çünkü henüz ``vite.config.js``’yi doldurmadık. 

## Vite'ı Yapılandır
Bağımlılıklar yüklendiğinde ve proje klasörümüz kodlamaya başlamamız için hazır olduğunda, artık Vite'ı yapılandırabilir ve projemizi yerel olarak çalıştırabiliriz.

1. ``Editörünüzde açın vite.config.js``. Boş olduğu için, sunucumuzu başlatabilmemiz için ona bazı ortak kalıp yapılandırması eklememiz gerekecek. Yapılandırmanın bu kısmı, Vite'a projemizin JavaScript'ini ve geliştirme sunucusunun nasıl davranması gerektiğini ( src hot reload ile klasörden çekerek) aramasını söyler.

```sh
const path = require('path')

export default {
 root: path.resolve(__dirname, 'src'),
 server: {
   port: 8080,
   hot: true
 }
}
```
2. **Ardından src/index.html’i dolduruyoruz.** Bu, Vite'ın daha sonraki adımlarda ekleyeceğimiz paketlenmiş CSS ve JS'yi kullanmak için tarayıcıya yükleyeceği HTML sayfasıdır.
```sh
<!doctype html>
<html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Bootstrap w/ Vite</title>
 </head>
 <body>
   <div class="container py-4 px-3 mx-auto">
     <h1>Hello, Bootstrap and Vite!</h1>
     <button class="btn btn-primary">Primary button</button>
   </div>
   <script type="module" src="./js/main.js"></script>
 </body>
</html>
```	

Bootstrap'ın CSS'sinin Vite tarafından ne zaman yüklendiğini görebilmemiz için d``iv class="container"`` ve ``<button>`` ile birlikte buraya biraz Bootstrap stili ekliyoruz.

3. Şimdi Vite'ı çalıştırmak için bir npm betiğine ihtiyacımız var. Aşağıda gösterilen komut dosyasını açın ``package.json`` ve ``start`` komutu verelim  (test komut dosyasına zaten sahip olmalısınız). Yerel Vite dev sunucumuzu başlatmak için bu betiği kullanacağız.

```js
{
 // ...
 "scripts": {
   "start": "vite",
   "test": "echo \"Error: no test specified\" && exit 1"
 },
 // ...
}
	
```
4. **Ve son olarak, Vite'ı başlatabiliriz.**  Terminalinizde ki ``my-project`` klasörden yeni eklenen npm komut dosyasını çalıştırın :

```sh
npm start
```	
![Vite geliştirici sunucusu çalışıyor](https://getbootstrap.com/docs/5.2/assets/img/guides/vite-dev-server-bootstrap.png)

Artık kullanmak istediğiniz Bootstrap bileşenlerini eklemeye başlayabilirsiniz. Ek özel Sass'ı dahil etme ve yalnızca gerekli olan Bootstrap CSS ve JS parçalarını içe aktararak oluşturma işlemini optimize etme hakkında bilgi almak için [Vite Örnek projesinin](https://github.com/twbs/examples/tree/main/vite) tamamına göz atmayı unutmayın.
  

<!-- Bu kılavuzun sonraki ve son bölümünde, Bootstrap'in tüm CSS ve JavaScript'lerini içe aktaracağız.
Önyüklemeyi İçe Aktar
      1. Bootstrap'in Sass içe aktarımını vite.config.js. içerisinde yapacağız. Yapılandırma dosyanız şimdi tamamlandı ve aşağıdaki kod parçasıyla eşleşmelidir. Buradaki tek yeni kısım resolve (çözümleme) bölümdür; bunu, içeri aktarmayı olabildiğince basit tutmak için .node_modules kaynak dosyalarımıza bir takma ad eklemek için kullanıyoruz 
const path = require('path')

export default {
 root: path.resolve(__dirname, 'src'),
 resolve: {
   alias: {
     '~bootstrap': path.resolve(__dirname, 'node_modules/bootstrap'),
   }
 },
 server: {
   port: 8080,
   hot: true
 }
}
	

      2. Şimdi Bootstrap'ın CSS'sini içe aktaralım. src/scss/styles.scss Bootstrap'in tüm kaynak Sass'larını içe aktarmak için aşağıdakini ekleyin .
// Import all of Bootstrap's CSS
@import "~bootstrap/scss/bootstrap";
	

İsterseniz stil sayfalarımızı tek tek de içe aktarabilirsiniz. Ayrıntılar için Sass içe aktarma belgelerimizi okuyun .
      3. Ardından CSS'yi yüklüyoruz ve Bootstrap'ın JavaScript'ini içe aktarıyoruz. src/js/main.jsCSS'yi yüklemek ve tüm Bootstrap JS'lerini içe aktarmak için aşağıdakileri ekleyin . Popper, Bootstrap aracılığıyla otomatik olarak içe aktarılacaktır.
// Import our custom CSS
import '../scss/styles.scss'

// Import all of Bootstrap's JS
import * as bootstrap from 'bootstrap'
	

      4. Paket boyutlarını düşük tutmak için JavaScript eklentilerini gerektiği gibi tek tek de içe aktarabilirsiniz:
import Alert from 'bootstrap/js/dist/alert';

// or, specify which plugins you need:
import { Tooltip, Toast, Popover } from 'bootstrap';
	

Bootstrap eklentilerinin nasıl kullanılacağı hakkında daha fazla bilgi için JavaScript belgelerimizi okuyun .
      5. Ve işin bitti! 🎉 Bootstrap'in kaynak Sass ve JS'si tamamen yüklendiğinde, yerel geliştirme sunucunuz artık böyle görünmelidir.
   
Bootstrap ile çalışan Vite dev sunucusu 
Artık kullanmak istediğiniz Bootstrap bileşenlerini eklemeye başlayabilirsiniz. Ek özel Sass'ı nasıl ekleyeceğinizi ve yalnızca Bootstrap CSS ve JS'nin ihtiyacınız olan kısımlarını içe aktararak yapınızı nasıl optimize edeceğinizi öğrenmek için eksiksiz Vite örnek projesini kontrol ettiğinizden emin olun . -->

# Ulaşılabilirlik - (Accessibility)
Bootstrap'ın erişilebilir içerik oluşturmaya yönelik özelliklerine ve sınırlamalarına kısa bir genel bakış.
Bootstrap, kullanımı kolay bir hazır stiller, düzen araçları ve etkileşimli bileşenler çerçevesi sağlayarak geliştiricilerin görsel olarak çekici, işlevsel açıdan zengin ve kullanıma hazır web siteleri ve uygulamalar oluşturmasına olanak tanır.

## Genel bakış ve sınırlamalar
Bootstrap ile oluşturulan herhangi bir projenin genel erişilebilirliği, büyük ölçüde yazarın işaretlemesine, ek stiline ve içerdikleri komut dosyasına bağlıdır. Ancak bunların doğru bir şekilde uygulanması şartıyla, Bootstrap ile [WCAG 2.1](https://www.w3.org/TR/WCAG/) (A/AA/AAA), [Bölüm 508](https://www.section508.gov/) ve benzer erişilebilirlik standartları ve gerekliliklerini karşılayan web siteleri ve uygulamalar oluşturmak tamamen mümkün olmalıdır.

## Yapısal işaretleme
Bootstrap'in stili ve düzeni, çok çeşitli biçimlendirme yapılarına uygulanabilir. Bu belge, geliştiricilere Bootstrap'in kullanımını göstermek ve olası erişilebilirlik sorunlarının ele alınabileceği yollar da dahil olmak üzere uygun semantik işaretlemeyi göstermek için en iyi uygulama örneklerini sağlamayı amaçlamaktadır.

## Etkileşimli bileşenler
Bootstrap'in kalıcı iletişim kutuları, açılır menüler ve özel araç ipuçları gibi etkileşimli bileşenleri, dokunma, fare ve klavye kullanıcıları için çalışmak üzere tasarlanmıştır. İlgili [WAI - ARIA](https://www.w3.org/WAI/standards-guidelines/aria/) rolleri ve niteliklerinin kullanılması yoluyla, bu bileşenler yardımcı teknolojiler (ekran okuyucular gibi) kullanılarak da anlaşılabilir ve çalıştırılabilir olmalıdır.
Bootstrap bileşenleri bilerek oldukça genel olacak şekilde tasarlandığından, yazarların bileşenlerinin kesin yapısını ve işlevselliğini daha doğru bir şekilde iletmek için JavaScript davranışının yanı sıra daha fazla ARIA rolleri ve nitelikleri eklemesi gerekebilir . Bu genellikle belgelerde belirtilir.


## Renk kontrastı
Şu anda Bootstrap'in varsayılan paletini oluşturan bazı renk kombinasyonları (çerçeve boyunca düğme varyasyonları, uyarı varyasyonları, form doğrulama göstergeleri gibi şeyler için kullanılır) yetersiz renk kontrastına neden olabilir (önerilen WCAG 2.1 metin rengi kontrast oranı olan 4.5:1'in altında). ve WCAG 2.1 metin dışı renk kontrast oranı 3:1 ), özellikle açık renkli bir arka plana karşı kullanıldığında. Yazarların, kendi özel renk kullanımlarını test etmeleri ve gerektiğinde, yeterli renk kontrast oranları sağlamak için bu varsayılan renkleri manuel olarak değiştirmeleri/genişletmeleri önerilir.

## Görsel olarak gizli içerik
Görsel olarak gizlenmesi gereken, ancak ekran okuyucular gibi yardımcı teknolojiler tarafından erişilebilir kalması gereken içerik, .visually-hidden sınıf kullanılarak şekillendirilebilir. Bu, ek görsel bilgilerin veya ipuçlarının (renk kullanımıyla ifade edilen anlam gibi) görsel olmayan kullanıcılara da iletilmesi gereken durumlarda faydalı olabilir.

```sh
<p class="text-danger">
 <span class="visually-hidden">Danger: </span>
 This action is not reversible
</p>
```	

Geleneksel "atlama" bağlantıları gibi görsel olarak gizlenmiş etkileşimli kontroller için .visually-hidden-focusable sınıfı kullanın. Bu, odaklanıldığında kontrolün görünür olmasını sağlayacaktır (görebilen klavye kullanıcıları için). Dikkat, önceki sürümlerdeki eşdeğer .sr-only ve sınıflarla karşılaştırıldığında, Bootstrap 5'ler bağımsız bir sınıftır ve sınıfla birlikte kullanılmamalıdır. .sr-only-focusable.visually-hidden-focusable.visually-hidden

```sh
<a class="visually-hidden-focusable" href="#content">Skip to main content</a>
```	

## Azaltılmış hareket
Bootstrap, prefers-reduced-motion medya özelliği için destek içerir . Kullanıcının azaltılmış hareket tercihini belirlemesine izin veren tarayıcılarda/ortamlarda, Bootstrap'teki çoğu CSS geçiş efekti (örneğin, kalıcı bir iletişim kutusu açıldığında veya kapatıldığında veya karusellerde kayan animasyon) devre dışı bırakılır ve anlamlı animasyonlar ( döndürücüler gibi) yavaşlayacaktır.
Destekleyen tarayıcılarda prefers-reduced-motion ve kullanıcının azaltılmış hareketi tercih edeceğini açıkça belirtmediği durumlarda (yani, burada prefers-reduced-motion: no-preference), Bootstrap özelliği kullanarak düzgün kaydırma sağlar scroll-behavior.


Ek kaynaklar:
- [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG/)
- [The A11Y Project](https://www.a11yproject.com/)
- [MDN accessibility documentation](https://developer.mozilla.org/en-US/docs/Web/Accessibility)
- [Tenon.io Accessibility Checker](https://tenon.io/)
- [Color Contrast Analyser (CCA)](https://www.tpgi.com/color-contrast-checker/)
- ["HTML Codesniffer" bookmarklet for identifying accessibility issues](https://github.com/squizlabs/HTML_CodeSniffer)
- [Microsoft Accessibility Insights](https://accessibilityinsights.io/)
- [Deque Axe testing tools](https://www.deque.com/axe/)
- [Introduction to Web Accessibility](https://www.w3.org/WAI/fundamentals/accessibility-intro/)



# RFS
Bootstrap'in yeniden boyutlandırma motoru, görünüm alanları ve cihazlar arasında kullanılabilir alanı daha iyi kullanmak için genel CSS özelliklerini duyarlı bir şekilde ölçeklendirir.


## RFS nedir?

Bootstrap'in yan projesi RFS , başlangıçta yazı tipi boyutlarını yeniden boyutlandırmak için geliştirilmiş bir birim yeniden boyutlandırma motorudur (dolayısıyla Duyarlı Yazı Tipi Boyutlarının kısaltmasıdır). Günümüzde RFS, çoğu CSS özelliğini , ``margin, padding, border-radius`` ve hatta `box-shadow` gibi birim değerleriyle yeniden ölçeklendirme yeteneğine sahiptir.

Mekanizma, tarayıcı görünüm alanının boyutlarına göre uygun değerleri otomatik olarak hesaplar. Duyarlı ölçekleme davranışını etkinleştirmek için ``rem`` ve viewport birimlerinin bir karışımıyla ``calc()`` işlevlerine derlenecektir.

## RFS'yi kullanma

Karışımlar Bootstrap'a dahildir ve Bootstrap's scss. RFS, gerekirse [bağımsız olarak da ](https://github.com/twbs/rfs/tree/v9.0.6#installation) kurulabilir .

## Karışımları kullanma

``rfs()`` karışımı için kısayolları vardır . Kaynak Sass ve derlenmiş CSS için aşağıdaki örneğe bakın. ``font-size, margin, margin-top, margin-right, margin-bottom, margin-left, padding, padding-top, padding-right, padding-bottom, and padding-left``.

```sh
.title {
 @include font-size(4rem);
}

.title {
 font-size: calc(1.525rem + 3.3vw);
}

@media (min-width: 1200px) {
 .title {
   font-size: 4rem;
 }
}
	
```

Karışıma başka herhangi bir özellik şu şekilde iletilebilir rfs():
```sh
.selector {
 @include rfs(4rem, border-radius);
}

!importantayrıca istediğiniz değere eklenebilir:
.selector {
 @include padding(2.5rem !important);
}
```

## Fonksiyonları kullanma

İçeriği kullanmak istemediğinizde ayrıca iki işlev vardır:

* rfs-value() rem bir px değerei iletilirse bir değeri rem değerine dönüştürür, diğer durumlarda aynı sonucu verir.
 
* rfs-fluid-value() özelliğin yeniden ölçeklendirilmesi gerekiyorsa bir değerin değişken sürümünü döndürür.
 
Bu örnekte, yalnızca kesme noktasının altında stil uygulamak için Bootstrap'ın yerleşik duyarlı kesme noktası karışımlarındanlg birini kullanıyoruz .

```sh
.selector {
 @include media-breakpoint-down(lg) {
   padding: rfs-fluid-value(2rem);
   font-size: rfs-fluid-value(1.125rem);
 }
}

@media (max-width: 991.98px) {
 .selector {
   padding: calc(1.325rem + 0.9vw);
   font-size: 1.125rem; /* 1.125rem is small enough, so RFS won't rescale this */
 }
}
```	

## Genişletilmiş belgeler
RFS, Bootstrap organizasyonu altında ayrı bir projedir. RFS ve yapılandırması hakkında daha fazla bilgiyi [GitHub](https://github.com/twbs/rfs/tree/v9.0.6) deposunda bulabilirsiniz .


# RTL

Bileşenlerimiz ve yardımcı programlarımız genelinde Bootstrap'ta sağdan sola metin desteğini nasıl etkinleştireceğinizi öğrenin.


## Yakından Tanıyın
İlk olarak Başlarken Giriş sayfamızı okuyarak Bootstrap'ı tanımanızı öneririz . Üzerinden geçtikten sonra, RTL'nin nasıl etkinleştirileceğini öğrenmek için [burayı okumaya devam edin](https://getbootstrap.com/docs/5.2/getting-started/introduction/).

Ayrıca, RTL'ye yaklaşımımızı güçlendirdiği için [RTLCSS](https://rtlcss.com/) projesini de okumak isteyebilirsiniz .

>Deneysel Özellik
RTL özelliği hala deneyseldir ve muhtemelen kullanıcı geri bildirimlerine göre gelişecektir. Bir şey mi gördünüz veya önereceğiniz bir gelişme var mı? [Bir konu açın](https://github.com/twbs/bootstrap/issues/new) , görüşlerinizi almak isteriz.

## Gerekli HTML
Bootstrap destekli sayfalarda RTL'yi etkinleştirmek için iki katı gereksinim vardır.
1. ``dir="rtl"`` üzerinde <html> ayarlayın .
2. ``lang`` Öğeye gibi uygun lang="ar"bir öznitelik ekleyin <html>.

Oradan, CSS'mizin bir RTL sürümünü eklemeniz gerekecek. Örneğin, RTL'nin etkin olduğu derlenmiş ve küçültülmüş CSS'mizin stil sayfası:

```sh
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.rtl.min.css" integrity="sha384-+4j30LffJ4tgIMrq9CwHvn0NjEvmuDCOfk6Rpg2xg7zgOxWWtLtozDEEVvBPgHqE" crossorigin="anonymous">
```	

## Başlangıç ​​şablonu
Bu değiştirilmiş RTL başlangıç ​​şablonunda yansıtılan yukarıdaki gereksinimleri görebilirsiniz.

```sh
<!doctype html>
<html lang="ar" dir="rtl">
 <head>
   <!-- Required meta tags -->
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">

   <!-- Bootstrap CSS -->
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.rtl.min.css" integrity="sha384-+4j30LffJ4tgIMrq9CwHvn0NjEvmuDCOfk6Rpg2xg7zgOxWWtLtozDEEVvBPgHqE" crossorigin="anonymous">

   <title>مرحبًا بالعالم!</title>
 </head>
 <body>
   <h1>مرحبًا بالعالم!</h1>

   <!-- Optional JavaScript; choose one of the two! -->

   <!-- Option 1: Bootstrap Bundle with Popper -->
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa" crossorigin="anonymous"></script>

   <!-- Option 2: Separate Popper and Bootstrap JS -->
   <!--
   <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.5/dist/umd/popper.min.js" integrity="sha384-Xe+8cL9oJa6tN/veChSP7q+mnSPaj5Bcu9mPX5F5xIGE0DVittaqT5lorf0EI7Vk" crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.min.js" integrity="sha384-ODmDIVzN+pFdexxHEHFBQH3/9/vQ9uori45z4JjnFsRydbmQbmL5t1tQ0culUzyK" crossorigin="anonymous"></script>
   -->
 </body>
</html>
	
```

## RTL örnekleri
Birkaç [RTL örneğimizden](https://getbootstrap.com/docs/5.2/examples/#rtl) biriyle başlayın .

## Yaklaşmak
Bootstrap'te RTL desteği oluşturma yaklaşımımız, CSS'mizi nasıl yazdığımızı ve kullandığımızı etkileyen iki önemli kararla birlikte gelir:
1. **İlk olarak [RTLCSS](https://rtlcss.com/) projesi ile kurmaya karar verdik** . Bu bize, LTR'den RTL'ye geçerken değişiklikleri ve geçersiz kılmaları yönetmek için bazı güçlü özellikler sunar. Ayrıca, bir kod tabanından iki Bootstrap sürümü oluşturmamıza da olanak tanır.
   
2. **İkinci olarak, mantıksal özellikler yaklaşımını benimsemek için bir avuç yönlü sınıfı yeniden adlandırdık.** Çoğunuz, esnek yardımcı programlarımız sayesinde mantıksal özelliklerle zaten etkileşime girdiniz; bunlar, left ve right lehinde start ve end  gibi yön özelliklerinin yerini alıyor. Bu, sınıf adlarını ve değerlerini herhangi bir ek yük olmadan LTR ve RTL için uygun hale getirir.
   
Örneğin, ``.ml-3`` için ``margin-left`` yerine  ``.ms-3`` kullanın.

Kaynak Sass veya derlenmiş CSS aracılığıyla RTL ile çalışmak, varsayılan LTR'mizden çok farklı olmamalıdır.


## Kaynaktan özelleştir

[Özelleştirme](https://getbootstrap.com/docs/5.2/customize/sass/) söz konusu olduğunda , tercih edilen yol değişkenlerden, haritalardan ve karışımlardan yararlanmaktır. Bu yaklaşım, [RTLCSS'nin nasıl çalıştığı] (https://rtlcss.com/learn/getting-started/why-rtlcss/sayesinde derlenmiş dosyalardan sonradan işlenmiş olsa bile RTL için aynı şekilde çalışır .

## Özel RTL değerleri

[RTLCSS değer yönergelerini](https://rtlcss.com/learn/usage-guide/value-directives/) kullanarak bir değişken çıktısını RTL için farklı bir değer yapabilirsiniz. Örneğin, ``$font-weight-bold`` tüm kod tabanının ağırlığını azaltmak için ``/*rtl: {value}*/`` sözdizimini kullanabilirsiniz:

``$font-weight-bold: 700 #{/* rtl:600 */} !default;``

Bu, varsayılan CSS ve RTL CSS'miz için aşağıdakilere çıktı verir:

```sh
/* bootstrap.css */
dt {
 font-weight: 700 /* rtl:600 */;
}

/* bootstrap.rtl.css */
dt {
 font-weight: 600;
}
```

## Alternatif yazı tipi yığını

Özel bir yazı tipi kullanıyorsanız, tüm yazı tiplerinin Latin olmayan alfabeyi desteklemediğini unutmayın.`` /*rtl:insert: {value}*/`` Pan-Avrupa'dan Arapça ailesine geçmek için, yazı tipi ailelerinin adlarını değiştirmek için yazı tipi yığınınızda kullanmanız gerekebilir .

Örneğin, Helvetica NeueLTR için yazı tipinden Helvetica Neue ArabicRTL için yazı tipine geçmek için Sass kodunuz şöyle görünebilir:

```sh
$font-family-sans-serif:
 Helvetica Neue #{"/* rtl:insert:Arabic */"},
 // Cross-platform generic font family (default user interface font)
 system-ui,
 // Safari for macOS and iOS (San Francisco)
 -apple-system,
 // Chrome < 56 for macOS (San Francisco)
 BlinkMacSystemFont,
 // Windows
 "Segoe UI",
 // Android
 Roboto,
 // Basic web fallback
 Arial,
 // Linux
 "Noto Sans",
 // Sans serif fallback
 sans-serif,
 // Emoji fonts
 "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji" !default;

```

## LTR ve RTL aynı anda
Aynı sayfada hem LTR hem de RTL'ye mi ihtiyacınız var? [RTLCSS String Maps](https://rtlcss.com/learn/usage-guide/string-map/) ``@import ``sayesinde bu oldukça basittir.

```sh
@Import'lerinizi bir sınıfla sarın ve RTLCSS için özel bir yeniden adlandırma kuralı belirleyin:
/* rtl:begin:options: {
 "autoRename": true,
 "stringMap":[ {
   "name": "ltr-rtl",
   "priority": 100,
   "search": ["ltr"],
   "replace": ["rtl"],
   "options": {
     "scope": "*",
     "ignoreCase": false
   }
 } ]
} */
.ltr {
 @import "../node_modules/bootstrap/scss/bootstrap";
}
/*rtl:end:options*/
```	

Sass'ı ve ardından RTLCSS'yi çalıştırdıktan sonra, CSS dosyalarınızdaki her seçicinin başına ``.ltr`` ve ``.rtl`` RTL dosyaları için eklenir. Artık her iki dosyayı da aynı sayfada kullanabilirsiniz ve bir veya diğer yönü kullanmak için bileşen sarmalayıcılarınızda ``.ltr`` veya ``.rlt`` öğelerini kullanabilirsiniz.

## Edge vakaları ve bilinen sınırlamalar
Bu yaklaşım anlaşılabilir olmakla birlikte, lütfen aşağıdakilere dikkat edin:

1. .ltr ve .rtl arasında geçiş yaparken , ``dir`` ve ``lang`` özelliklerini eklediğinizden emin olun. 

2. Her iki dosyayı da yüklemek gerçek bir performans darboğazı olabilir: biraz [optimizasyon](https://getbootstrap.com/docs/5.2/customize/optimize/) düşünün ve belki de bu dosyalardan birini [eşzamansız olarak yüklemeyi deneyin .](https://www.filamentgroup.com/lab/load-css-simpler/)

3. Bu şekilde yerleştirme stilleri, form-validation-state()miksimizin amaçlandığı gibi çalışmasını engelleyecektir, bu nedenle biraz kendi başınıza ince ayar yapmanızı gerektirir. [#31223](https://github.com/twbs/bootstrap/issues/31223'e bakın .

## The breadcrumb case
breadcrumb separator , kendi yepyeni değişkenini gerektiren tek durumdur - ``yani $breadcrumb-divider-flipped`` varsayılan olarak ``$breadcrumb-divider``

Ek kaynaklar

- [RTLCSS](https://rtlcss.com/)
- [RTL Styling 101](https://rtlstyling.com/posts/rtl-styling)



# Katkıda bulunmak

Belge oluşturma komut dosyalarımız ve testlerimizle Bootstrap'in geliştirilmesine yardımcı olun.

##Tool kurulumları

Bootstrap , belgeleri oluşturmak ve kaynak dosyaları derlemek için npm komut dosyalarını kullanır. package.json'umuz , kod derlemek, testleri çalıştırmak ve daha fazlası için bu komut dosyalarını barındırır. Bunlar, depomuz ve belgelerimiz dışında kullanılmak üzere tasarlanmamıştır.

Yapı sistemimizi kullanmak ve belgelerimizi yerel olarak çalıştırmak için Bootstrap'in kaynak dosyalarının ve Node.js dosyasının bir kopyasına ihtiyacınız olacak. Bu adımları izleyin ve sallanmaya hazır olmalısınız:

1. Bağımlılıklarımızı yönetmek için kullandığımız Node.js'yi indirip yükleyin .
2. Ya Bootstrap'in kaynaklarını indirin ya da Bootstrap deposunu çatallayın .
3. /bootstrapKök dizine gidin ve package.jsonnpm install içinde listelenen yerel bağımlılıklarımızı yüklemek için çalıştırın .

Tamamlandığında, komut satırından sağlanan çeşitli komutları çalıştırabileceksiniz.

## npm komut dosyalarını kullanma

Paketimiz.json , projeyi geliştirmek için çok sayıda görev içerir. npm runTerminalinizdeki tüm npm komut dosyalarını görmek için çalıştırın . Birincil görevler şunları içerir:
| Görev | Tanım |
| --- | --- |
| `npm start` | CSS ve JavaScript'i derler, belgeleri oluşturur ve yerel bir sunucu başlatır. |
| `npm run dist` | dist/Derlenmiş dosyalarla dizini oluşturur. [Sass](https://sass-lang.com/), [Autoprefixer](https://github.com/postcss/autoprefixer), ve [terser](https://github.com/terser/terser). kullanır.|
| `npm test` | Çalıştırdıktan sonra testleri yerel olarak çalıştırır `npm run dist` |
| `npm run docs-serve` | Belgeleri yerel olarak oluşturur ve çalıştırır. |

## SASS
Bootstrap, Sass kaynak dosyalarımızı CSS dosyalarına derlemek için [Dart Sass](https://sass-lang.com/dart-sass)'ı kullanır (oluşturma sürecimize dahildir) ve kendi varlık işlem hattınızı kullanarak Sass'ı derliyorsanız aynısını yapmanızı öneririz. Daha önce Bootstrap v4 için Node Sass'ı kullandık, ancak Node Sass dahil olmak üzere LibSass ve bunun üzerine inşa edilen paketler artık kullanımdan kaldırıldı .

Dart Sass, 10'luk bir yuvarlama hassasiyeti kullanır ve verimlilik nedenleriyle bu değerin ayarlanmasına izin vermez. Bu hassasiyeti, örneğin küçültme sırasında olduğu gibi, oluşturulan CSS'nin sonraki işlemleri sırasında düşürmeyiz, ancak bunu yapmayı seçtiyseniz, tarayıcı yuvarlama ile ilgili sorunları önlemek için hassasiyeti en az 6 olarak korumanızı öneririz.

## Autoprefixer
Bootstrap, derleme sırasında bazı CSS özelliklerine satıcı öneklerini otomatik olarak eklemek için [Autoprefixer](https://github.com/postcss/autoprefixer) 'ı (yapı sürecimize dahildir) kullanır. Bunu yapmak, v3'te bulunanlar gibi satıcı karışımlarına olan ihtiyacı ortadan kaldırırken CSS'mizin önemli kısımlarını tek seferde yazmamıza izin vererek zamandan ve koddan tasarruf etmemizi sağlar.
Autoprefixer aracılığıyla desteklenen tarayıcıların listesini GitHub depomuzda ayrı bir dosyada tutuyoruz. Ayrıntılar için [browserslistrc](https://github.com/twbs/bootstrap/blob/v5.2.0/.browserslistrc) 'ye bakın .

## RTLCSS
Bootstrap, derlenmiş CSS'yi işlemek ve bunları RTL'ye dönüştürmek için [RTLCSS](https://rtlcss.com/)'yi ``padding-left`` kullanır – temel olarak yatay yöne duyarlı özellikleri karşıtlarıyla değiştirir. CSS'imizi yalnızca bir defa yazmamıza ve RTLCSS [kontrol](https://rtlcss.com/learn/usage-guide/control-directives/) ve değer yönergelerini kullanarak küçük değişiklikler yapmamıza izin verir.

## Yerel belgeler
Belgelerimizi yerel olarak çalıştırmak, [hugo-bin](https://www.npmjs.com/package/hugo-bin) npm paketi aracılığıyla yüklenen Hugo'nun kullanılmasını gerektirir . Hugo, bize temel içerikler, Markdown tabanlı dosyalar, şablonlar ve daha fazlasını sağlayan son derece hızlı ve oldukça genişletilebilir bir statik site oluşturucudur. Nasıl başlayacağınız aşağıda açıklanmıştır:

1. Tüm bağımlılıkları yüklemek için yukarıdaki [araç kurulumunu](https://getbootstrap.com/docs/5.2/getting-started/contribute/#tooling-setup) çalıştırın .
2. Kök dizinden komut satırında /bootstrapçalıştırın .npm run docs-serve
3. http://localhost:9001/Tarayıcınızda açın ve voilà.

Belgelerini okuyarak Hugo'yu kullanma hakkında daha fazla bilgi edinin .

## Sorun giderme
Bağımlılıkları yüklemeyle ilgili sorunlarla karşılaşırsanız, önceki tüm bağımlılık sürümlerini (genel ve yerel) kaldırın. Ardından, yeniden çalıştırın npm install.