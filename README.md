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
* Tahminleme (Prediction): Elimizdeki verileri kullanarak gelecekte ne olacağını kestirmek.<br>
* İlişki Analizi: Değişkenler arasındaki ilişkinin ne kadar güçlü olduğunu anlamak.<br>
* Karar Destek: İş dünyasında riskleri azaltmak ve verilere dayalı stratejiler geliştirmek.<br>
Regresyoun tarihçesine bakacak olursak regresyonun kökeni 19. yüzyılın başlarına kadar uzanır.
Fransız matematikçi Adrien-Marie Legendre 1805 yılında, "En Küçük Kareler Yöntemi"ni (Least Squares) yayınladı. 
Bu, regresyonun hesaplanma şeklinin temelidir. Regresyon en önemli isimlerinden biri hatta isim babası olan kişi de 
İngiliz bilim insanıFrancis Galton, "Regresyon" terimini 1880'lerde ilk kullanan kişidir. Galton, uzun boylu
babaların çocuklarınınboyunun ortalamaya doğru "gerilediğini" (regression to the mean) fark etmiş ve 
bu fenomene bu ismi vermiştir.<br>

İstatistik dünyasında çok sayıda regresyon türü olsa da, en çok kullanılan çeşitleri;<br>

#### A. Basit Doğrusal Regresyon (Simple Linear Regression) :Tek bir bağımsız değişken ile
bağımlı değişken arasındaki ilişkiyi düz bir çizgi üzerinde inceler. Formülü şu şekildedir:<br>
              $$Y = \beta_0 + \beta_1 X + \epsilon$$


#### B. Çoklu Doğrusal Regresyon (Multiple Linear Regression) :Bağımlı değişkeni etkileyen birden
fazla bağımsız değişken olduğunda kullanılır. Örneğin; bir evin fiyatını (y) tahmin ederken sadece
metrekaresine ($x_{1}$) değil, oda sayısına ($x_{2}$) ve konumuna ($x_{3}$) da bakılması durumudur.

#### C. Lojistik Regresyon (Logistic Regression) :Sonucun sayısal değil, kategorik (Evet/Hayır, Geçti/Kaldı, 0/1) 
olduğu durumlarda kullanılır. Örneğin, bir e-postanın spam olup olmadığını tahmin etmek için kullanılır.

#### D. Polinom Regresyon (Polynomial Regression) :Değişkenler arasındaki ilişki düz bir çizgi değil 
de bir eğri ise tercih edilir.E. Ridge ve Lasso RegresyonVeri setinde çok fazla değişken olduğunda ve bu 
değişkenler arasında yüksek korelasyon bulunduğunda, modelin aşırı öğrenmesini (overfitting) engellemek için 
kullanılan düzenleme (regularization) teknikleridir.
# Basit Doğrusal Regresyon 
Basit doğrusal regresyon; bağımsız değişken (X)ile bağımlı değişken (Y)deki değişimi açıklamayı, bağımsız değişkendeki bir birimlik değişimin bağımlı değişken üzerindeki etkisini ölçmeyi amaçlar.
Temel amaç, bağımlı ve bağımsız değişken arasındaki ilişkiyi ifade eden doğrusal fonksiyonu bulmaktır.
Stokastik (Olasılıklı) bir model olan ve ana kütledeki ilişkiyi gösteren basit doğrusal regresyon denklemi aşağıdaki gibi ifade edilir.<br>
y=β0+β1X+ϵ <br>
Burada;<br>
* β0:Doğrunun y-eksenini kestiği yer ve regresyon sabitidir.<br>
* β1:Doğrunun eğimi veya regresyon katsayısıdır.<br>
* ϵ: Rastgele(Tesadüfi-Şans) hata değeridir.<br>

Biz kurduğumuz regresyonun doğruluğunu ve güvenilirliğini anlamak için  bazı tesler yapıyoruz bu testler  varyasyonların homojenliği testi, otokolerasyon testi, normallik testi, T-testi, Ki-Kare testi, F-testi, $$R^2$$ testi bunlar sadece teslerin birkaçı. Regresyona uygulanabilecek daha pek çok test var. 
# Regresyondaki Testerin Kullanımları ve Özellikleri 
## 1) T-Testi 
T-testi, iki farklı grubun ortalama değerleri arasında istatistiksel olarak anlamlı bir fark olup olmadığını belirlemek için kullanılan temel bir çıkarımsal istatistik yöntemidir.<br>
Gerçek dünyadaki veriler nadiren birbirinin aynısıdır. T-testi, gözlemlenen farkın sadece **şans eseri mi** oluştuğunu yoksa **belirgin bir nedene mi** dayandığını anlamamızı sağlar.
* **Eğitim:** Bir fizik dersindeki öğrencilerin notları ile bir yazı dersindeki farklı bir öğrenci grubunun notlarının karşılaştırılması.
* **Tıp:** Bir ilaç testinde, plasebo verilen (kontrol grubu) ile ilaç verilen (deney grubu) hastaların iyileşme oranlarının analizi.

#### T-Testi Varsayımları
Sağlıklı bir t-testi sonucu alabilmek için verilerin şu dört ana varsayımı karşılaması gerekir:

1.  **Ölçek Türü:** Toplanan veriler sürekli (continuous) veya sıralı (ordinal) bir ölçeğe uygun olmalıdır (Örn: IQ skorları, sınav notları).
2.  **Rastgele Örneklem:** Veriler, toplam nüfusun rastgele seçilmiş bir bölümünden toplanmalıdır.
3.  **Normal Dağılım:** Veriler grafik üzerine döküldüğünde çan eğrisi şeklinde bir normal dağılım sergilemelidir.
4.  **Varyans Homojenliği:** Grupların standart sapmalarının eşit veya birbirine çok yakın (homojen) olması gerekir.

####  T- Testinde hipotezlerin kullanılması 
 * **$H_0$ (Sıfır Hipotezi / Yokluk Hipotezi)**: İncelenen durumlar arasında bir fark veya ilişki olmadığını savunan, "statüko"yu temsil eden hipotezdir.<br>
* **$H_1$ (Alternatif Hipotez)**: Araştırmacının asıl ispatlamaya çalıştığı, değişkenler arasında anlamlı bir fark veya ilişki olduğunu öne süren hipotezdir.
T-testi, her iki veri kümesinden birer örneklem alır ve süreci **Sıfır Hipotezi ($H_0$)** üzerine kurar.

**Sıfır Hipotezi ($H_0$):** İki ortalamanın birbirine eşit olduğunu varsayar (Fark yoktur).
Formüller kullanılarak hesaplanan değerler, standart tablo değerleri ile karşılaştırılır. Bu karşılaştırma, farkın "şans aralığının" dışında olup olmadığını belirler.
**

#### Sonuçların Yorumlanması

T-testi, gruplar arasında gerçek bir fark olup olmadığını sorgular. Analiz sonucunda p-değeri ve t-skoru baz alınarak şu kararlara varılır:

| Karar | Anlamı |
| :--- | :--- |
| **Sıfır Hipotezi Reddedildi** | Farklılıklar istatistiksel olarak **anlamlıdır**. Veriler güçlüdür ve fark muhtemelen şans eseri değildir. |
| **Sıfır Hipotezi Kabul Edildi** | Farklılıklar istatistiksel olarak **anlamlı değildir**. Gruplar arasındaki fark rastlantısal olabilir. |

---

T-Testini Kullanmak
T-testi hesaplamak için üç temel veri değerine ihtiyaç vardır:<br>
1)Her veri kümesindeki ortalama değerler arasındaki fark, ortalama fark olarak da bilinir.<br>
2)Her grubun standart sapması<br>
3)Her grubun veri değerlerinin sayısı<br>
T-testi iki değer üretir: t-değeri ve serbestlik derecesi.<br>
* T-değeri veya t-skoru, iki örneklem kümesinin ortalamaları arasındaki farkın, örneklem kümeleri içindeki varyasyona oranıdır.
* Serbestlik dereceleri, bir çalışmada değişme özgürlüğüne sahip değerleri ifade eder. Bunlar, sıfır hipotezinin önemini ve geçerliliğini değerlendirmek için gereklidir.

## T testi çeşitleri 
T- tstini  çeşitli yöntemlere uygulayabilmek için bir kaç durum için kullanılan formüller vardır bunlar şu şekildedir;
#### 1)Eşleştirilmiş Örnek T-Testi Formülü:

$$
T = \frac{\text{ortalama}_1 - \text{ortalama}_2}{\frac{s_{\text{fark}}}{\sqrt{N}}}
$$

Burada:<br>
* $\text{ortalama}_1, \text{ortalama}_2$ = Örnek kümelerinin her birinin ortalama değerleri
* $s_{\text{fark}}$ = Eşleştirilmiş veri değerlerinin farklarının standart sapması
* $N$ = Örneklem boyutu (eşleştirilmiş farkların sayısı)
* $N-1$ = Serbestlik dereceleri
anlamına gelmektedir.
#### 2)Eşit Varyans veya Birleştirilmiş T-Testi Formülü

$$
\text{T değeri} = \frac{\text{ortalama}_1 - \text{ortalama}_2}{\sqrt{\frac{(n_1 - 1) \times \text{var}_1^2 + (n_2 - 1) \times \text{var}_2^2}{n_1 + n_2 - 2} \times \left( \frac{1}{n_1} + \frac{1}{n_2} \right)}}
$$
Burada:<br>
* $\text{ortalama}_1, \text{ortalama}_2$ = Örneklem kümelerinin her birinin ortalama değerleri
* $\text{var}_1, \text{var}_2$ = Örneklem kümelerinin her birinin varyansı
* $n_1, n_2$ = Her örnek kümesindeki kayıt sayısı (örneklem boyutu)
anlamına gelmektedir.
#### 4) Eşit Olmayan Varyans T-Testi Formülü

$$
\text{T değeri} = \frac{\text{ortalama}_1 - \text{ortalama}_2}{\sqrt{\left( \frac{\text{var}_1}{n_1} + \frac{\text{var}_2}{n_2} \right)}}
$$

Burada:<br>
* $\text{ortalama}_1 \text{ ve } \text{ortalama}_2$ = Örneklem kümelerinin her birinin ortalama değerleri
* $\text{var}_1 \text{ ve } \text{var}_2$ = Örneklem kümelerinin her birinin varyansı
* $n_1 \text{ ve } n_2$ = Her örnek kümesindeki kayıt sayısı (örneklem boyutu)
anlamına gelmektedir.
#### Özelte T testi:
T-testi, iki popülasyon örneğinin ortalamaları arasında istatistiksel olarak anlamlı bir fark olup olmadığını belirlemek için kullanılır. İstatistikte hipotez testinde kullanılır ve iki popülasyon arasındaki farklılıkların anlamlı mı yoksa rastgele mi olduğunu gösterebilir.<br>
T-testi hesaplaması üç veri kullanır: her veri kümesindeki ortalama değerler arasındaki fark, her grubun standart sapması ve veri değerlerinin sayısı.<br>
T-test formülünün farklı varyasyonları vardır. Hangisinin kullanılacağı farklı faktörlere bağlıdır. Ancak her varyasyon aynı istatistiksel soruyu incelemek için kullanılır.<br>



# R2: Regresyon Modelinin Performansı
Bağımsız değişken x’in, regresyon modeli ile bağımlı değişken y’i ne kadar açıkladığı yüzdesinin ölçütü olan belirtme katsayısı bir diğer adıyla determinasyon katsayısıdır ve $$R^2$$ ile gösterilir. Belirtme katsayısı, bağımlı değişkendeki değişimin yüzde kaçının bağımsız değişkenler tarafından açıklanabildiğini gösterir.
$$R^2$$, “0” ile “1” arasında değerler alır(0< $$R^2$$ <1). Değişkenler arasında doğrusal bir ilişki olduğunda, $$R^2$$ değerinin 1’e yaklaşması; bağımlı değişkendeki değişimin büyük bir kısmının bağımsız değişkenler tarafından açıklandığını gösterir. Bağımlı ve bağımsız değişken arasındaki ilişkinin derecesi ve yönünü gösteren korelasyon katsayısının(r) karesi belirtme katsayısına ($$R^2$$) eşittir. Belirtme katsayısı:<br>
$$R^2$$ =Açıklanabilen Değişim/Toplam Değişim=RKT/YOAKT<br> 
eşitliğiyle hesaplanır.<Br>
Eşitlikte verilen RKT; regresyon kareler toplamı ve YOAKT; Y ortalama ayrılış kareler toplamıdır.

Kurulan regresyon modelinin performansı, $$R^2$$ ile ölçülür. $$R2^$$, 1’e ne kadar yakınsa, regresyon o kadar anlamlıdır ve belirleyicidir. Bu konuda bilimsel bir karar verebilmek için hipotez testi yapılır.

#### Düzeltilmiş R Kare
R-kare, lineer regresyon modeli için bağımsız değişkenlerimiz (X) tarafından açıklanan bağımlı değişkenimizdeki (Y) varyasyon oranını ölçer. Düzeltilmiş R-kare sadece gerçekte bağımlı değişkeni etkileyen bağımsız değişkenler tarafından açıklanan varyasyon oranını ölçer.


### Düzeltilmiş R-Kare (Adjusted R-squared)

$$
\text{Düzeltilmiş R-kare} = 1 - \left( \frac{(1 - R^2) \times (n - 1)}{n - p - 1} \right)
$$
Burada:<br>
* **$n$:** Örneklemdeki veri sayısı
* **$p$:** Bağımsız değişken sayısı
* **$R^2$:** Belirleyicilik katsayısı (R-kare)
anlmaına gelmekteder. 

# Korelasyon Katsayısı(r)




