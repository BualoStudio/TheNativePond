# The Native Pond Vaatler Listesi

![flatbreadlist_background](/background/tr/FBL-docs-bg-tr.png)

> [!WARNING]
> 1. Bu listedeki her şey havada kalan vaatlerdir; ne nihai görünümü ne de gerçek uygulamayı temsil eder.
> 2. Bu listedeki bazı içerikler ekip toplantılarında tartışılmamıştır.
> 3. Bu listedeki bazı içerikler için fizibilite çalışması yapılmamıştır.
> 4. Bu liste, fan yapımı ve türev çalışmalar için yol gösterici öneriler sunabilir.
> 5. Ekip, bu listeyle ilgili sonraki tüm adımları atma ve listenin nihai yorum hakkını saklı tutar.

---

## 🎮 Kontrol Sistemi

Akıcı hareket ve iyi bir kamera açısı, oyunun oynanabilirliğini garantileyen en önemli unsurlardır. **Karakter mutlaka hareket edebilmeli!**

### Hareket

- Oyuncu, karakteri **harita** üzerinde hareket ettirir ve özel konumlarda (ör. balık tutma platformu) bir tuşa basarak ya da özel konumun küçük koordinat alanına girerek o **özel konuma** geçiş animasyonunu **tetikler**.
- Oyunla dokunmatik butonlar (mobil), klavye (masaüstü) ve oyun kumandası aracılığıyla **etkileşime** girilir; tuş atamaları özelleştirilebilir.

### Kamera Açısı

- Haritanın özel olmayan bölgelerinde **üçüncü şahıs** kamera açısı kullanılır.
- Haritanın özel bölgelerinde (ör. balık tutma platformu) **birinci şahıs** kamera açısı kullanılır ve o özel bölgenin içi (varsa) gösterilir.
- Harita, kamera açısını takip ederek **hareket eder**.

---

## 🗺️ Harita Sistemi

Masaya kapanıp **harita** yap! Haritada gerçekten her şey var!

### Yakınlaştırma ve Yön

- Harita, kamera açısıyla birlikte **dönmez**.
- Harita **yakınlaştırılıp uzaklaştırılabilir**.
- Harita "**kuzey yukarı, güney aşağı, batı solda, doğu sağda**" yön mantığını izler.

### Sınırlar

- Oyun haritasının **sınırları** vardır; yani oyuncu **haritanın kenarından** geçemez.
- Oyuncu sınırı aşmaya çalıştığında oyun, oyuncuyu **zorla geri çeker** ve şu metni gösterir: "* Tanıdık bir his yükseliyor — sanki şunu duyuyorsun: 'Önümüzdeki bölgeyi sonra keşfedelim!' Sonra keşfedemeyeceğini bilsen de yine de denemek istiyorsun."
- Sınırlar belirgin **doğal engeller** (ör. büyük dağlar) ya da **insan yapımı çitler** (ör. Huizhou tarzı mimarinin duvarları) olabilir.

### Hava Durumu

- Hava durumunun **türleri** şunlardır:
	- Güneşli.
	- Yağmurlu.
	- Fırtınalı.
	- Karlı.
- Hava durumu **değişimi** şunlara göre belirlenebilir:
	1. Oyuncunun elle ayarlamasına göre.
	2. Bir bölgenin iklim özelliklerine benzerliğe göre.
	3. Tamamen rastgele bir olasılığa göre.

### Mevsimler

- Mevsimler her **90 saatte** bir değişir.
- Mevsimlerin **türleri** şunlardır:
	- İlkbahar.
	- Yaz.
	- Sonbahar.
	- Kış.

### Fotoğraf Makinesi

- Oyuncu, herhangi bir konumda (GUI arayüzü hariç) klavyede bir tuşa basarak, bir butona tıklayarak ya da kumandada bir tuşa basarak **fotoğraf çekebilir**.
- **Fotoğraf çekerken** oyun, çekimi belirtmek için tam ekran **beyaz ışık** gösterir. Bu nedenle oyunun başlangıç ekranına **ışığa duyarlı epilepsi** uyarı ekranı eklenmesi gerekebilir.
- **Fotoğraf çekerken** oyun, ekrandaki tüm öğeleri (GUI öğeleri hariç) otomatik olarak **yakalar** ve bir **çerçeve** ekler.
- Oyun, fotoğrafı paylaşabilmen için **belirlenen klasöre** **kaydeder**.

### Balık Tutma Göleti

- Balık tutma göleti, oyunun en temel özel bölgesidir; **balık tutma platformu**, **gölet** ve **küçük tekne**den oluşur.

#### Balık Tutma Platformu

- Göletin en **güney** ucunda bulunur.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; karakter oturma pozisyonuna geçer ve o özel bölgenin görsel arayüzü gösterilir.
- Balık tutma platformu **balık tutmak** için kullanılır.

#### Gölet

- Haritanın en **kuzey** ucunda bulunur.
- Oyuncu bu özel bölgeye **girdiğinde** karakter **yüzme** durumuna geçer.

#### Küçük Tekne

- Göletin **herhangi bir yerinde** bulunur (bu, oyuncunun tekneyi en son park ettiği konuma bağlıdır).
- Oyuncu bu özel bölgeye **girdiğinde** karakter **sürüş** durumuna geçer ve o özel bölgenin görsel arayüzü gösterilir.
- Oyuncu, küçük tekneyle **gölette** gezinebilir.

### Çadır

- Haritanın ortasının hafif **güneybatısında** bulunur.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; o özel bölgenin görsel arayüzü gösterilir.
- Çadır, **kampın** kalbidir.
- Çadırın **içi** ve **boyutu**, Robinson Crusoe'daki çadırın tasarımından esinlenebilir.

### Tarla

- Tarla, çadırın **güneydoğu** tarafındadır.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; o özel bölgenin görsel arayüzü gösterilir.
- Tarla **ekim** için kullanılır.

### Pazar

- Pazar, haritanın **doğu**sundadır.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; o özel bölgenin görsel arayüzü gösterilir.
- Pazar **alışveriş** için kullanılır.

### Ağaç

- Çadırın **güneydoğusunda** bulunur.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; karakter oturma pozisyonuna geçer.
- Ağaçta bazen (ör. sonbaharda) **elmalar** belirir. Elmalar, oyuncu tarafından **uzun bir tahta sopayla** düşürülüp **toplanabilir**.
- Oyuncu **ağacın** altında bir süre (yaklaşık 1 dakika) durduğunda oyun, "[W]'ye basılı tutarak meditasyona başla" yüzen butonunu gösterir; oyuncu W'ye bastığında, butona tıkladığında ya da kumandada bir tuşa bastığında **meditasyona** girer. Oyuncu **meditasyon** yaparken oyun, tam ekran **görsel efektler** (çeşitli fizik formülleri) gösterir ve oyuncunun **elma** tarafından vurulma ihtimali vardır.

### Kamp Ateşi

- Çadırın **doğu**sunda, çok uzak olmayan bir yerde bulunur.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; o özel bölgenin görsel arayüzü gösterilir.
- Kamp ateşi **yakılabilir** ve ışık sağlar.
- Kamp ateşi **yemek pişirmek** için kullanılabilir.

### Sihirli Deniz Kabuğu

- Oyuncu, su kenarındaki **kumsalda** **sihirli deniz kabuğunu** alabilir.
- Oyuncu sihirli deniz kabuğunu **aldığında** karakter üfleme durumuna geçer ve kamera açısı otomatik olarak yakınlaşır. Bu sırada oyuncu hareket edemez. Aynı zamanda bu özel eşyanın görsel arayüzü gösterilir.
- Sihirli deniz kabuğu, oyuncunun çalabileceği 7 **tona** sahiptir.
- Sihirli deniz kabuğunun birden fazla **çeşidi** vardır; farklı çeşitlerin **tınıları** farklıdır.

### Posta Kutusu

- Çadırın **güney** tarafındadır.
- Oyuncu bu özel bölgeye **girdiğinde** kamera açısı otomatik olarak yakınlaşır ve birinci şahıs açıya geçer; o özel bölgenin görsel arayüzü gösterilir.
- Posta kutusu **posta alıp göndermek** için kullanılır.

---

## 🎣 Balıkçılık Sistemi

Oyuncu, **balık tutma platformunda** **olta** kullanarak balık tutabilir.

### Türler

- Oyunun **balık tutma göleti**nde hem **deniz balığı türleri** hem **tatlı su balığı türleri** yakalanabilir. Balıkların yanı sıra **koleksiyonlar** da yakalanabilir.
	1. Bu, oyuncunun seçtiği **balık tutma platformuna** göre belirlenebilir (ör. deniz kenarındaki platformda yalnızca deniz balıkları, göl kenarındaki platformda yalnızca tatlı su balıkları yakalanabilir).
	2. Bu, her balık türünün yakalanma **olasılığına** göre belirlenebilir (yani aynı deniz kenarı platformda, olasılıklara bağlı olarak hem deniz hem tatlı su balıkları yakalanabilir).
- Her balık türünü yakalama **olasılığı** şunlara göre belirlenir:
	1. **Gerçek hayatta** her balık türünü yakalama olasılığına göre. Bu bir değer aralığı olabilir; bu aralık, hava durumu ve mevsim gibi çeşitli faktörlere göre ayarlanır, sabit kalmaz.
	2. Tamamen **rastgele** bir olasılığa göre.
- Koleksiyon yakalama **olasılığı** şunlara göre belirlenir:
	1. Oyuncunun geçmişteki **ısırma oranına** göre.
	2. Sabit bir aralıktaki rastgele **olasılığa** göre.
	3. Tamamen **rastgele** bir olasılığa göre.

### Isırma Oranı

Bu arada belirtelim: ısırma oranı, balığın **oltayı ısırma** olasılığıdır; balığın en sonunda yakalanma olasılığı değildir.

- Oyunun **ısırma oranı** şu faktörlerin birlikte etkisiyle belirlenir:
	- Oyuncunun oltasının iğnesinde yem olup olmadığı.
	- Oyuncunun döküntü yem (groundbait) atıp atmadığı.
	- İğnedeki yemin türü.
	- Oyun saati (ör. gündüz, gece).
	- Gece kafa lambasının açık olup olmadığı.
	- Oyunun hava durumu.
	- Oyunun mevsimi.
- Oyunun ısırma oranı ayrıca şunlara göre de belirlenebilir:
	1. Oyuncunun geçmişteki ısırma oranına göre.
	2. Tamamen rastgele bir olasılığa göre.

### Yakalama Oranı

Adı üstünde: yakalama oranı, balığın en sonunda yakalanma olasılığıdır.

- Oyunun **yakalama oranı** şu faktörlerin birlikte etkisiyle belirlenir:
	- Balığın oltayı ısırıp ısırmadığı.
	- Oyuncunun oltayı çekme anı (ne çok erken ne çok geç).
	- Misinanın kopma oranı.
	- Olta iğnesinin boyutu.

### Olta

- Olta; **kamış**, **şamandıra**, **iğne** ve **misina**dan oluşur.
- Olta takımının her parçasının **dayanıklılığı** vardır; dayanıklılık düştükçe takımın hasar görme olasılığı artar. Olta hasar gördüğünde, hasar gören parçanın **değiştirilmesi** gerekir.

#### Kamış

- **Kamış**, **olta takımının** bir parçasıdır.
- Oyuncu, **ticaret sistemi**ni kullanarak kamış satın alabilir; ör. 2,7 metrelik ve 3,6 metrelik kamışlar.
- Farklı uzunluktaki kamışların atış ve çekiş süreleri farklıdır.

#### Şamandıra

- **Şamandıra**, **olta takımının** bir parçasıdır; oyuncu, şamandıranın **hareketine** bakarak oltayı çekip çekmeyeceğine karar verebilir.
- Oyuncu, **ticaret sistemi**ni kullanarak şamandıra satın alabilir; ör. sıradan ve ışıklı şamandıralar.
- Farklı balık türlerinin oltayı ısırdığında şamandıranın hareketi farklıdır; bu, gerçek hayatta balıkların oltayı ısırdığındaki şamandıra hareketleri temel alınarak belirlenir.
- Şamandıranın **görünürlüğü** (yani kurşun ağırlığı) ayarlanabilir, böylece oyuncu daha rahat gözlem yapar.

#### İğne

- **İğne**, **olta takımının** bir parçasıdır ve balık yakalamanın temelidir.
- Oyuncu, **ticaret sistemi**ni kullanarak iğne satın alabilir; ör. küçük ve büyük boy iğneler.
- İğnenin boyutu, oyuncunun büyük ya da küçük balık yakalayıp yakalayamayacağını belirleyen en önemli faktördür.
- İğneye **yem** takılabilir.

#### Misina

- **Misina**, **olta takımının** bir parçasıdır.
- Oyuncu, **ticaret sistemi**ni kullanarak misina satın alabilir; ör. sıradan 0,8 numara ve kaliteli 2,0 numara misinalar.
- Farklı misinaların **kopma oranı** farklıdır; bu, şu faktörlerin birlikte etkisiyle belirlenebilir:
	- Misinanın kalitesi.
	- Misinanın kullanım süresi ya da dayanıklılığı.

### Yem

- Oyuncu, **ticaret sistemi**ni kullanarak yem satın alabilir; ör. sıradan yem ve kırmızı solucan.
- Satın alınan yem toz halindeyse, toz yemin su ekleme ve yoğurma gibi adımlarla yeme dönüştürülmesi gerekir.
- Farklı yemlerin **ısırma oranı** farklıdır.
- Yem sarf malzemesidir; oyuncunun yemi kalmadığında ve deniz kabuğu sayısı (balık satışından kazanılanlar dahil) bir paket yem almaya yetmediğinde, oyun ertesi gün **posta kutusuna** ücretsiz ikmal bırakır.

### Döküntü Yem (Groundbait)

- Oyuncu, **ticaret sistemi**ni kullanarak döküntü yem satın alabilir; ör. fermente soya posası ve eski mısırın şarapta bekletilmiş hali.
- Farklı döküntü yemlerin **ısırma oranı** farklıdır.
- Döküntü yem, ısırma oranını büyük ölçüde artırabilir.

### Kafa Lambası

- Oyuncu, **ticaret sistemi**ni kullanarak kafa lambası satın alabilir; ör. sıradan kafa lambası ve mavi ışıklı gece balıkçılığı lambası.
- Farklı kafa lambalarının **ısırma oranı** ve görsel etkileri farklıdır.
- Geceleri kafa lambası, oyuncunun su yüzeyini ve şamandırayı görmesini sağlar.
- Geceleri kafa lambası balıkları ürkütüp ısırma oranını düşürebilir.

### Koleksiyonlar

- Koleksiyonlar temel olarak **denize atılmış şişeler**, **hatıralar** ve **hikâye parçaları** olarak ayrılır.
- Oyuncu koleksiyonları şu yollarla **elde edebilir**:
	- Balık tutarak.
	- Cat'in hediyesi olarak.

#### Denize Atılmış Şişe

- Denize atılmış şişelerde **mektup kâğıtları** bulunur.
- Mektup kâğıtlarının çoğu, oyunculara cesaret veren **motivasyon sözleridir**.

#### Hatıralar

- Bazı hatıralar **çadırda** **sergilenebilir**.

#### Hikâye Parçaları

- Hikâye parçaları, oyuncuları **köylülerin** hikâyelerini öğrenmeye yönlendirir.
- Tüm hikâye parçaları toplandığında oyuncu, **köylülerin** hikâyesini eksiksiz ve ayrıntılı biçimde öğrenmek için uzun bir hikâye bölümünün kilidini açabilir.

---

## 🍳 Yemek Pişirme Sistemi

**Yiyecek** yap ve yemeyi dene!

### Mutfak Gereçleri

- Mutfak gereçleri üç bölümden oluşur: **ocak**, **kesme tahtası** ve **mutfak aletleri**.

#### Ocak

- Ocak, yemeği **ısıtmak** için kullanılır.
- Ocak şuralarda **bulunabilir**:
	1. Çadırın içinde.
	2. Çadırın dışında ama çadıra yakın.
- Ocak, oyuncunun bazı **mutfak aletlerini** (ör. tava) yerleştirmesine olanak tanır.
- Ocağı kullanmadan önce ocağa **yakıt** eklemek gerekir.
- Oyuncunun, yaptığı yiyeceğin yenilebilir olması için **ateşi kontrol etmesi** gerekir.

#### Kesme Tahtası

- Kesme tahtası, yemeği **doğramak** için kullanılır.
- Kesme tahtası, oyuncunun bazı **malzemeleri** (ör. Çin lahanası) ve **yarı mamul yiyecekleri** yerleştirmesine olanak tanır.
- Oyuncu, bazı **mutfak aletlerini** (ör. bıçak) kullanarak kesme tahtasında kesim yapabilir.

#### Mutfak Aletleri

- Mutfak aletleri, oyuncunun malzemeleri rahatça **işlemesini** sağlar.
- Mutfak aletleri şunları içerir:
	- Büyük kazan.
	- Tava.
	- Buhar sepeti.
	- Porselen kase.
	- Mutfak bıçağı.
	- Oklava.

### Tarifler

- Oyuncu, **tariflere** göre yiyecek yapabilir. Genel olarak tarife uyulduğunda yiyecek her zaman başarıyla yapılır.
- Oyuncu ayrıca tarife **uymayıp** kendi yöntemini de deneyebilir.

### Yiyecekler

- Oyuncu, tüm **yiyecek yapım sürecini** tamamladığında **yiyeceği** elde eder.
- Oyuncu şu yiyecekleri yapabilir:
	- Sade erişte (un, hamur yoğurma, şerit kesme ve kaynar suda pişirme sürecinin tamamıyla elde edilir).
	- Buğulama doldurulmuş ekmek (un, hamur yoğurma, hamur açma, iç harç yapma, doldurma ve buharda pişirme sürecinin tamamıyla elde edilir).
	- Sahanda yumurta (yumurta kırma, ocağı yakma ve çevirme sürecinin tamamıyla elde edilir).
	- Izgara balık (kamp ateşinde balık közlenerek elde edilir).
	- Tarif edilemez nesne (yiyecek yapımında başarısızlıkla elde edilir).
	- Kömür (tarife uymadan yiyecek yapılmaya çalışılır ve başarısız olunursa elde edilir).

### Yeme

- Oyuncu **yiyeceği** yaptıktan sonra yemeyi deneyebilir.
- Oyuncu, ilgili **yiyeceğe** ya da **yiyeceğin bir parçasına** tıklayarak yiyebilir.
- Oyuncu **yiyeceği** yerken rahatlatıcı bir **ses efekti**, iç ısıtan bir **metin** ve yiyeceğin ya da parçasının animasyonla **kaybolması** yeme eylemini temsil eder.
- Özellikle oyuncu **tarif edilemez nesneyi** yediğinde şu durumlardan biri tetiklenebilir:
	1. Karakter bayılır ve bir süre sonra uyanır.
	2. Karakter bir süre mide bulantısı görsel efekti yaşar.
	3. Hiçbir şey olmaz.

---

## ⛺️ Kamp Sistemi

Yalnızca **çadır** güvenlik hissi verir!

### Depolama

- **Çadırda** oyuncu, sahip olduğu **eşyaları** görüntüleyebilir.
- Oyuncunun **sahip olduğu** eşyalar şunları içerir:
	- Balıklar.
	- Koleksiyonlar.
	- Balıkçılık takımları.
	- Ekinler.
- Bazı eşyalar (ör. bazı koleksiyonlar) **sergilenebilir**.

### Başarımlar

- **Çadırda** oyuncu, kazandığı **başarımları** görüntüleyebilir.

### Yatak

- **Gün batımında** ve **gece**, oyuncu yatağa tıklayarak **uyuyabilir** ve geceyi atlayabilir.
- Oyuncu ertesi günün **gün doğumunda** ya da **sabahında** uyanır; oyuncu **biraz daha uyumayı** seçerek uyumaya devam edebilir.

### Duygu Geri Dönüşüm Kutusu

- Geri dönüştürülebilir çöp kutusuna benzeyen bu kutu, oyuncunun **gerçek hayatta** yaşadığı üzücü şeyleri yazmasına, sonra kâğıdı buruşturup duygu geri dönüşüm kutusuna atmasına olanak tanır!

### Günlük

- Oyuncu, **günlüğüne** her gün yaşadıklarını yazabilir (ister oyundaki ister gerçek hayattaki).
- Oyun, oyuncunun **günlüğün** belirli sayfalarını paylaşabilmesi için **belirlenen klasöre** dışa aktarmasına olanak tanır.

### Albüm

- Albüm, oyuncunun **resim kâğıdına** çizdiği tüm **eserleri** gösterir.
- Albümün tamamı, paylaşabilmesi için **belirlenen klasöre** tek bir dosya olarak dışa aktarılabilir.

---

## 🐚 Ticaret Sistemi

Bu karpuz olgun mu?

### Satın Alma

- Oyuncu, **pazardan** ürün satın alabilir.
- Pazarda oyuncu, çeşitli mesleklerden **köylülerle** konuşabilir.
- Oyuncu köylülerle **konuşurken** **özel bir hikâye** tetiklenebilir; bu özel hikâye tamamlandığında **indirim** alınabilir.
- Oyuncu pazardan şu **türlerde** ürün satın alabilir:
	- Balıkçılık takımları (ör. kamış).
	- Ekin tohumları (ör. buğday tohumu).
	- İşlenmiş ekinler (ör. un).
	- Sebzeler (ör. Çin lahanası).
	- Yakıt (ör. kömür).
	- Yiyecek baharatları (ör. tuz).
	- Resim kâğıdı (ör. 1:1 resim kâğıdı).
	- Pullar.

### Satış

- Oyuncu, **pazarda** ürün satabilir.
- Oyuncu pazarda şu **türlerde** ürün satabilir:
	- Balıklar.
	- Bazı koleksiyonlar.
- Oyuncu balık satarken **günün balık fiyatı** esas alınır.
- **Günün balık fiyatı** iki türe ayrılır: **taze balık** ve **stok balık**; hiçbir fiyat sabit değildir. Günün balık fiyatı şu faktörlerin birlikte etkisiyle belirlenebilir:
	- Oyunun hava durumu.
	- Oyunun mevsimi.
	- Sabit bir aralıktaki rastgele bir değer.

### Para Birimi

- Oyun, para birimi olarak **deniz kabuğu** kullanır.
- Oyuncu deniz kabuğunu şu yollarla **elde edebilir**:
	- Alışverişle.
	- Balık tutarak.
	- Cat'in hediyesi olarak.

---

## 🌽 Ekin Sistemi

**Ekin ek**, **sula ve gübrele**, sonra **hasat et**.

### Ekin

- Ekin dikmek için **ekin tohumu** sahibi olmak gerekir.
- Ekin **süreci** şöyledir: toprağı düzleştir, tohumları serp, üzerini toprakla ört, sula, gübrele.
- Tohumun çimlenme koşulları: **yeterli nem**, **uygun sıcaklık** ve **bol oksijen**.
- Ekin ekerken oyuncunun **dikkate alması** gerekenler:
	- Oyunun hava durumu.
	- Oyunun mevsimi.

### Büyüme

- Ekin büyürken oyuncu **sulamaya** ve **gübrelemeye** ara vermeden devam etmelidir.
- Ekin, belirli aralıklarla (yaklaşık 90 saatte bir) bir sonraki **büyüme aşamasına** **geçer**.

### Hasat

- Ekin **tamamen olgunlaştığında** oyuncu **ekini** ve **ekin tohumlarını** hasat edebilir.

---

## 🐱 CatGPT

Kediciğinle **sohbet et** ya da **kediyi sev** ฅ՞•ﻌ•՞ฅ.

### Sohbet

- Oyuncu, Cat'e **mesaj gönderebilir**.
- Cat, oyuncuya belirli ağırlıklara göre **yanıt verir**; ağırlıklar şunlara göre belirlenebilir:
	1. Oyuncunun gönderdiği mesajın uzunluğuna göre.
	2. Tamamen rastgele bir olasılığa göre.
- Cat, çeşitli tonlarda ve tınılarda "**Meow**" yanıtları vererek oyuncuya duygusal değer katar.

### Kediyi Sevme

- Oyuncu, Cat'in **kafasına** hafifçe dokunarak kediyi sevebilir.
- Kediyi severken Cat'in üzerinden "**Meow**" yazılı mesajlar uçar ve çeşitli tonlarda ve tınılarda "**Meow**" sesleri oyuncuya duygusal değer katar.

### Hediye

- Cat, ertesi sabah oyuncu uyandığında oyuncuya bir **hediye** verebilir.
- Cat'in oyuncuya **hediye** verip vermeyeceği şunlara göre belirlenebilir:
	1. Oyuncunun dün Cat ile sohbet etme ya da kediyi sevme sayısına göre.
	2. Oyuncunun geçmişte Cat ile sohbet etme ya da kediyi sevme sayısına göre.
	3. Tamamen rastgele bir olasılığa göre.
- Hediye **türleri** şunları içerebilir:
	- Balıklar.
	- Deniz kabuğu.
	- Bazı koleksiyonlar (çok küçük bir olasılıkla).

### Başka Nesneler de...

- Cat'in dışında oyuncu, sohbet edebileceği ya da sevebileceği **başka nesneler** de seçebilir. Bu **başka nesneler**, **tanıtım hikâyesinde** görünen **ekip üyeleri** olabilir.

---

## 🖌️ Çizim Sistemi

Son derece gerçekçi kâğıt ve boyalarla **resim yap** ve kaydet.

### Resim Kâğıdı

- Resim kâğıdı, gerçek kâğıttan farksızdır; **yayılma (akma)**, **yeniden boyama** ve **renk karıştırma** gibi işlevlere olanak tanır.
- Oyuncu, **ticaret sistemi**ni kullanarak resim kâğıdı satın alabilir; ör. 1:1 ve 3:4 boyutunda kâğıtlar.

### Palet

- Varsayılan olarak 8 temel renk sunulur; oyuncu **fırçayla** boya alıp **palette** renkleri karıştırabilir.
- Boyama türü **suluboya** ya da **guaj** olabilir.
- Renk karıştırırken iki rengin boyası **fırça** aracılığıyla karıştırılır; karıştırılmayan boya kendi rengini korur ve karışım rengi, oyuncunun karıştırma derecesine göre belirlenir.

### Fırça

- Fırça, boyayı ya da suyu resim kâğıdına **sürebilir**.

### Kaydetme

- Oyuncunun çizdiği eserler **albüme** **kaydedilir**.
- Oyuncu, eserleri paylaşabilmesi için **belirlenen klasöre** **dışa aktarabilir**.

---

## 📬 Posta Kutusu Sistemi

**Posta** al ve gönder.

### Gelen Posta

- Oyuncu şu postaları **alabilir**:
	- Oyuncunun kendine gönderdiği mektuplar.
	- Ücretsiz yem ikmalleri.
	- Bayram dilekleri.
	- Doğum günü dilekleri.

### Giden Posta

- Oyuncu şu postaları **gönderebilir**:
	- Gelecekteki kendine mektuplar.
- Posta gönderirken mektuba **pul** yapıştırılmalıdır.

---

## 📺 Görsel Arayüz

Akıcı **doğrusal olmayan animasyonlar**, oyunculara her zaman iyi bir görsel deneyim yaşatır.

### Kontroller

- Kontroller, etkileşim davranışlarını ve olaylarını **tetikleyebilir**.
- Kontroller, Today@PolarBay ile aynı tasarım stilini korumalıdır.
- Kontroller **basıldığında** anında küçülmeli, ardından doğrusal olmayan bir biçimde geri yaylanmalıdır.
- Kontrollerin **konumu** ve **boyutu** özelleştirilebilir.

### Kartlar

- Kartlarla **etkileşime** girilemez.
- Kartlar, Today@PolarBay ile aynı tasarım stilini korumalıdır.
- Kartlar, görece **düzenli** arka planları göstermek için kullanılır; ör. sırt çantası arayüzü.

### Göz Koruyucu Yeşil Ekran

- Oyuncu **balık tutarken** **uzun süre** boyunca **şamandıraya** odaklanmak zorunda kaldığı için özel olarak **göz koruyucu yeşil ekran** tasarlanmıştır.
- Göz koruyucu yeşil ekran, belirli aralıklarla **tam ekran kaplanarak** oyuncuyu **zorunlu mola vermeye** iter.
- Göz koruyucu yeşil ekranın **aralık süresi** ve **kaplama süresi** ayarlardan değiştirilebilir ya da kapatılabilir.
- Göz koruyucu yeşil ekran, oyuncunun topladığı **denize atılmış şişelerdeki** **mektup kâğıtlarının** içeriğini gösterir.

### Renk Temaları

- Oyunda **iki** renk teması bulunabilir: beyaz tema ve siyah tema.
- Beyaz ve siyah temalar şu koşullara göre **değişebilir**:
	1. Gerçek hayattaki gece-gündüz durumuna göre.
	2. Oyundaki gece-gündüz durumuna göre.
	3. Oyuncunun ayarlar arayüzünde elle yaptığı ayara göre.

### Parçacık Efektleri

- Parçacık efektleri, **özel olaylarla** oluşur; ör. teknenin su yüzeyinde ilerlemesi.
- Parçacık efektlerinin sayısı **ayarlardan** değiştirilebilir ya da kapatılabilir; böylece performans sorunları önlenir.

### Gelişmiş Malzemeler

- Gelişmiş malzemeler, yani **akrilik** malzemeler.
- Oyuncu, gelişmiş malzemeleri **ayarlardan** açıp kapatabilir.
- Gelişmiş malzemeler açıldığında, oyuncunun kontrolleri, kartları vb. GUI öğelerinin **boş alanları** yarı saydam, bulanık bir malzemeye dönüşür.

---

## 🕒 Zaman Sistemi

**Zaman** hep çok hızlı akar; o kadar hızlı ki çoğu şeyi kaçırırız.

### Zaman Dönüşümü

- Oyundaki **bir gün**, gerçek hayattaki **bir saattir**.
- Oyun zamanının gerçek zamana dönüşüm oranı **1:24**'tür.

### Zaman Dilimleri

- Oyundaki **gündüz** ve **gece** sürelerinin her biri **30 dakikadır**.
- **Bir gün** (60 dakika) içinde oyunun zaman dilimleri şöyle ayrılır:
	- Gün doğumu: 1-2. dakikalar.
	- Sabah: 2-10. dakikalar.
	- Öğle: 11-20. dakikalar.
	- Öğleden sonra: 21-28. dakikalar.
	- Gün batımı: 29-30. dakikalar.
	- Gece: 31-60. dakikalar.

---

## 💾 Kayıt Sistemi

Mevcut **oyun ilerlemeni** **kaydet**; böylece balıklarımız ve tuzumuz da güvende olur.

### Kayıt

- **Kayıt** sayfasında oyuncu, **kayıt al** butonuna tıklayarak mevcut ilerlemeyi **kaydedebilir**.
- **Kayıt** sayfasında oyuncu, **kayıt yükle** butonuna tıklayarak kaydedilmiş kayıtları **yükleyebilir**.
