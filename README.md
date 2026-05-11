# R İSTATİSTİK HAKKINDA GENEL BİLGİLER 
R, istatistiksel hesaplama, veri analizi ve grafiksel gösterimler için veri bilimcileri ve istatistikçiler tarafından dünya çapında yaygın olarak kullanılan güçlü ve açık kaynaklı bir programlama dilidir.
R programlama dilinin şüphesiz en önemli özelliği açık kaynak kodlu ve ücretsiz olmasıdır. Diğer özellikleri ise şu şekildedir;<br>
Diğer programlar ile kıyaslandığında (SPSS, WEKA vb.) en kapsamlı istatistiksel analiz paketidir. R standart istatistiksel testler, doğrusal ve doğrusal olmayan modelleme, klasik istatistik testleri, zaman serileri analizi, sınıflandırma, kümeleme gibi istatistiksel ve gelişmiş grafiksel çizim teknikleri sunmaktadır.
Çapraz Platformdur. GNU / Linux, Macintosh ve Microsoft Windows gibi değişik işletim sistemleri üzerinde 32 ve 64 bit olarak çalışabilir.<br>
Açık kaynak kodlu olmasının sağladığı avantajlardan birisi de biyo-bilişim, veri madenciliği, istatistik gibi konularda 15,000’in üzerinde paket mevcuttur ve kullanıcıların kendi paketlerini, objelerini oluşturmasını destekler.
Microsoft Excel, Microsoft Access, Oracle, MySQL ve SQLite, Hadoop, SAS ve SPSS gibi birçok araç ile entegre şekilde çalışabilir, data import- export işlemlerini gerçekleştirebilir.
PDF, JPG, PNG ve SVG formatlarında çıktı alınabilmesinin yanı sıra, LATEX ve HTML için tablo ve grafik çıktısı alınabilir.<br>
Verinin ekranda ya da basılı bir eserde görüntülenebilmesine olanak veren geniş, graﬁksel özellikler sunar.
Olumsuz özelliklerinden de bahsedecek olursak;
Program ara yüzü (R Terminal) kullanıcı dostu değildir. (Birçok mevcut ara yüzü bulunmakla birlikte ben RStudio’yu tercih ediyorum).
Türkçe doküman yetersizliği vardır.
Veriyi işlenecek hale getirmek zaman alıcı ve hataya açık bir süreç olabilir.
Tüm işlemler bellekte gerçekleştirilir. Yani, çok büyük veriler üzerinde işlem yapmak için belleğin veri seti için yeterli olması gerekir.
R Programlama Nasıl İndirilir?<br>
Windows için ; <br>
https://cran.r-project.org/bin/windows/base/<br>
MAC için ;  <br>
https://cran.r-project.org/bin/macosx/<br>
Linux için ; <br>
https://cran.r-project.org/bin/linux/ubuntu/fullREADME.html<br>
İndirdiğiniz versiyonun çalışıp çalışmadığını cmd de den R yazarak kontrol edebilirsiniz.
R nin arayüzü kullanıma çok uygun olduğunu düşünmediğimden RStudio'nun arayüzünü kullanıcam onun içinde
https://posit.co/products/open-source/rstudio buradan inidrme yapabilirsiniz.
Kurulumları gerçekleştirdikten sonra YouTube üzerinden R ın ilk kullanımı ile ilgili bilgilere ulaşabilirsiniz.
# Regresyon Nedir? Regresyon Çeşitleri Nelerdir?
Regresyon analizi, veri bilimi ve istatistiğin temel taşlarından biridir.
En basit tabiriyle; bir bağımlı değişken ile bir veya daha fazla bağımsız değişken arasındaki 
ilişkiyi anlamak ve geleceğe dair tahminlerde bulunmak için kullanılan matematiksel bir yöntemdir.<br>
Hayatta her şey birbiriyle bağlantılıdır. "Hava sıcaklığı artarsa dondurma satışları ne kadar artar?" veya
"Eğitim yılı arttıkça gelir ne kadar yükselir?" gibi soruların cevabını net bir matematiksel modelle vermek istersiniz.
Peki neden kullanılır?<br>
Tahminleme (Prediction): Elimizdeki verileri kullanarak gelecekte ne olacağını kestirmek.<br>
İlişki Analizi: Değişkenler arasındaki ilişkinin ne kadar güçlü olduğunu anlamak.<br>
Karar Destek: İş dünyasında riskleri azaltmak ve verilere dayalı stratejiler geliştirmek.<br>
Regresyoun tarihçesine bakacak olursak regresyonun kökeni 19. yüzyılın başlarına kadar uzanır.
Fransız matematikçi Adrien-Marie Legendre 1805 yılında, "En Küçük Kareler Yöntemi"ni (Least Squares) yayınladı. 
Bu, regresyonun hesaplanma şeklinin temelidir. Regresyon en önemli isimlerinden biri hatta isim babası olan kişi de 
İngiliz bilim insanıFrancis Galton, "Regresyon" terimini 1880'lerde ilk kullanan kişidir. Galton, uzun boylu
babaların çocuklarınınboyunun ortalamaya doğru "gerilediğini" (regression to the mean) fark etmiş ve 
bu fenomene bu ismi vermiştir.<br>

İstatistik dünyasında çok sayıda regresyon türü olsa da, en çok kullanılan çeşitleri;<br>

A. Basit Doğrusal Regresyon (Simple Linear Regression) :Tek bir bağımsız değişken ile
bağımlı değişken arasındaki ilişkiyi düz bir çizgi üzerinde inceler. Formülü şu şekildedir:<br>
              $$Y = \beta_0 + \beta_1 X + \epsilon$$


B. Çoklu Doğrusal Regresyon (Multiple Linear Regression) :Bağımlı değişkeni etkileyen birden
fazla bağımsız değişken olduğunda kullanılır. Örneğin; bir evin fiyatını (y) tahmin ederken sadece
metrekaresine ($x_{1}$) değil, oda sayısına ($x_{2}$) ve konumuna ($x_{3}$) da bakılması durumudur.

C. Lojistik Regresyon (Logistic Regression) :Sonucun sayısal değil, kategorik (Evet/Hayır, Geçti/Kaldı, 0/1) 
olduğu durumlarda kullanılır. Örneğin, bir e-postanın spam olup olmadığını tahmin etmek için kullanılır.

D. Polinom Regresyon (Polynomial Regression) :Değişkenler arasındaki ilişki düz bir çizgi değil 
de bir eğri ise tercih edilir.E. Ridge ve Lasso RegresyonVeri setinde çok fazla değişken olduğunda ve bu 
değişkenler arasında yüksek korelasyon bulunduğunda, modelin aşırı öğrenmesini (overfitting) engellemek için 
kullanılan düzenleme (regularization) teknikleridir.
# Basit Doğrusal Regresyon 
Basit doğrusal regresyon; bağımsız değişken (X)ile bağımlı değişken (Y)deki değişimi açıklamayı, bağımsız değişkendeki bir birimlik değişimin bağımlı değişken üzerindeki etkisini ölçmeyi amaçlar.
Temel amaç, bağımlı ve bağımsız değişken arasındaki ilişkiyi ifade eden doğrusal fonksiyonu bulmaktır.
Stokastik (Olasılıklı) bir model olan ve ana kütledeki ilişkiyi gösteren basit doğrusal regresyon denklemi aşağıdaki gibi ifade edilir.<br>
y=β0+β1X+ϵ
Burada;<br>
β0:Doğrunun y-eksenini kestiği yer ve regresyon sabitidir.<br>
β1:Doğrunun eğimi veya regresyon katsayısıdır.<br>
ϵ: Rastgele(Tesadüfi-Şans) hata değeridir.<br>
Biz kurduğumuz regresyonun doğruluğunu ve güvenilirliğini anlamak için  bazı tesler yapıyoruz bu testler  varyasyonların homojenliği testi,otokolerasyon testi, normallik testi 


# R2: Regresyon Modelinin Performansı
Bağımsız değişken x’in, regresyon modeli ile bağımlı değişken y’i ne kadar açıkladığı yüzdesinin ölçütü olan belirtme katsayısı bir diğer adıyla determinasyon katsayısıdır ve R2 ile gösterilir. Belirtme katsayısı, bağımlı değişkendeki değişimin yüzde kaçının bağımsız değişkenler tarafından açıklanabildiğini gösterir.
R2, “0” ile “1” arasında değerler alır(0<R2<1). Değişkenler arasında doğrusal bir ilişki olduğunda, R2 değerinin 1’e yaklaşması; bağımlı değişkendeki değişimin büyük bir kısmının bağımsız değişkenler tarafından açıklandığını gösterir. Bağımlı ve bağımsız değişken arasındaki ilişkinin derecesi ve yönünü gösteren korelasyon katsayısının(r) karesi belirtme katsayısına (R2) eşittir. Belirtme katsayısı:
R2=Açıklanabilen Değişim/Toplam Değişim=RKT/YOAKT eşitliğiyle hesaplanır.
Eşitlikte verilen RKT; regresyon kareler toplamı ve YOAKT; Y ortalama ayrılış kareler toplamıdır.

Kurulan regresyon modelinin performansı, R2 ile ölçülür. R2, 1’e ne kadar yakınsa, regresyon o kadar anlamlıdır ve belirleyicidir. Bu konuda bilimsel bir karar verebilmek için hipotez testi yapılır.

# Düzeltilmiş R Kare
R-kare, lineer regresyon modeli için bağımsız değişkenlerimiz (X) tarafından açıklanan bağımlı değişkenimizdeki (Y) varyasyon oranını ölçer. Düzeltilmiş R-kare sadece gerçekte bağımlı değişkeni etkileyen bağımsız değişkenler tarafından açıklanan varyasyon oranını ölçer.

Düzeltilmiş R kare= $$ 1-(1 – R2 )*n-1/n-p-1$$ <br>
n: Örneklemdeki veri sayısı<br>
p: bağımsız değişken sayısı<br>

# Korelasyon Katsayısı(r)




