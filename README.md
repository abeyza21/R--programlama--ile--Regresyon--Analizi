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

Biz kurduğumuz regresyonun doğruluğunu ve güvenilirliğini anlamak için  bazı tesler yapıyoruz bu testler  varyasyonların homojenliği testi, otokolerasyon testi, normallik testi, T-testi, Student-T testi, Ki-Kare testi, F-testi, $$R^2$$ testi bunlar sadece teslerin birkaçı. Regresyona uygulanabilecek daha pek çok test var. 
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

### T testi çeşitleri 
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

## 2) F-Testi 
F testi, oldukça esnek bir istatistiksel test türüdür. Çok çeşitli ortamlarda kullanılabilir. F testleri, birden fazla model terimini aynı anda değerlendirebilir; bu da farklı doğrusal modellerin uyumlarını karşılaştırmalarına olanak tanır. Buna karşılık, t testleri aynı anda yalnızca bir terimi değerlendirebilir.<br>
Genel anlamlılık F-testini hesaplamak için, istatistiksel yazılımınızın karşılaştırdığı iki modelde uygun terimleri içermesi yeterlidir. Genel F-testi, belirttiğiniz modeli bağımsız değişken içermeyen modelle karşılaştırır. Bu tür model aynı zamanda sadece kesişim terimi içeren model olarak da bilinir.<br<

Genel anlamlılık F testi, doğrusal regresyon modelinizin, bağımsız değişken içermeyen bir modele göre verilere daha iyi uyup uymadığını gösterir. Bu yazıda, genel anlamlılık F testinin R-kare gibi diğer regresyon istatistikleriyle nasıl ilişkili olduğunu inceleyeceğim. R-kare, modelinizin verilere ne kadar iyi uyduğunu gösterir ve F testi bununla ilişkilidir.
F testi, oldukça esnek bir istatistiksel test türüdür. Çok çeşitli ortamlarda kullanılabilir. F testleri, birden fazla model terimini aynı anda değerlendirebilir; bu da farklı doğrusal modellerin uyumlarını karşılaştırmalarına olanak tanır. Buna karşılık, t testleri aynı anda yalnızca bir terimi değerlendirebilir.
ANOVA'da F testlerinin nasıl çalıştığına dair blog yazımı okuyun .
Genel anlamlılık F-testini hesaplamak için, istatistiksel yazılımınızın karşılaştırdığı iki modelde uygun terimleri içermesi yeterlidir. Genel F-testi, belirttiğiniz modeli bağımsız değişken içermeyen modelle karşılaştırır. Bu tür model aynı zamanda sadece kesişim terimi içeren model olarak da bilinir.
Genel anlamlılık için F testi aşağıdaki iki hipotezi içermektedir:
Sıfır hipotezi, bağımsız değişken içermeyen modelin, sizin modeliniz kadar verilere uygun olduğunu belirtir.
Alternatif hipotez, modelinizin yalnızca kesişim noktasını içeren modele göre verilere daha iyi uyduğunu söyler.
İstatistiksel çıktıda, genel F-testini ANOVA tablosunda bulabilirsiniz.

# $$R^2$$: Regresyon Modelinin Performansı
Bağımsız değişken x’in, regresyon modeli ile bağımlı değişken y’i ne kadar açıkladığı yüzdesinin ölçütü olan belirtme katsayısı bir diğer adıyla determinasyon katsayısıdır ve $$R^2$$ ile gösterilir. Belirtme katsayısı, bağımlı değişkendeki değişimin yüzde kaçının bağımsız değişkenler tarafından açıklanabildiğini gösterir.
$$R^2$$, “0” ile “1” arasında değerler alır(0< $$R^2$$ <1). Değişkenler arasında doğrusal bir ilişki olduğunda, $$R^2$$ değerinin 1’e yaklaşması; bağımlı değişkendeki değişimin büyük bir kısmının bağımsız değişkenler tarafından açıklandığını gösterir. Bağımlı ve bağımsız değişken arasındaki ilişkinin derecesi ve yönünü gösteren korelasyon katsayısının(r) karesi belirtme katsayısına ($$R^2$$) eşittir. Belirtme katsayısı:<br>
$$R^2$$ =Açıklanabilen Değişim/Toplam Değişim=RKT/YOAKT<br> 
eşitliğiyle hesaplanır.<Br>
Eşitlikte verilen RKT; regresyon kareler toplamı ve YOAKT; Y ortalama ayrılış kareler toplamıdır.

Kurulan regresyon modelinin performansı, $$R^2$$ ile ölçülür. $$R^2$$, 1’e ne kadar yakınsa, regresyon o kadar anlamlıdır ve belirleyicidir. Bu konuda bilimsel bir karar verebilmek için hipotez testi yapılır.

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

### Korelasyon Katsayısı(r)
Korelasyon katsayısı (r), iki değişken arasındaki doğrusal ilişkinin yönünü ve gücünü ölçen istatistiksel bir değerdir. Bu değer değişkenlerin birimlerinden bağımsızdır ve her zaman -1 ile 1 arasında yer alır.

r > 0 ise değişkenler arasında pozitif yönlü ilişki vardır. Yani bir değişken artarken diğeri de artma eğilimindedir.
r < 0 ise negatif yönlü ilişki vardır. Bir değişken artarken diğeri azalma eğilimindedir.
r ≈ 0 olduğunda ise değişkenler arasında zayıf veya anlamlı bir doğrusal ilişki bulunmaz.

Korelasyon katsayısının mutlak değeri 1’e yaklaştıkça ilişkinin gücü artar. Örneğin, r = 1 tam pozitif ilişkiyi, r = -1 ise tam negatif ilişkiyi ifade eder. Bu yöntem veri analizi, makine öğrenmesi ve istatistiksel modelleme çalışmalarında değişkenler arasındaki ilişkiyi incelemek için yaygın olarak kullanılmaktadır.

#### Korelasyon Katsayısı ve R² Farkı
Korelasyon katsayısı, iki değişken arasındaki doğrusal ilişkinin yönünü ve gücünü gösterir. Regresyon katsayısı ise bağımsız değişkendeki değişimin bağımlı değişken üzerindeki etkisini ifade eder.
Regresyon modelinin anlamlı olması için eğim katsayısı olan β₁’in sıfırdan farklı olması gerekir. β₁ ≠ 0 ise değişkenler arasında anlamlı bir ilişki vardır.
R² (R Kare) değeri, regresyon modelinin veriyi açıklama oranını gösterir. R² değeri 1’e yaklaştıkça modelin başarısı artar.

# Regresyon Varsayımları ve Teşhis Testleri
Bir regresyon modeli kurup $R^2$ değerini hesaplamak analiz sürecinin sadece ilk adımıdır. Elde edilen katsayıların ve tahminlerin istatistiksel olarak güvenilir (BLUE - Best Linear Unbiased Estimator) kabul edilebilmesi için modelin belirli varsayımları karşılaması gerekir. Bu varsayımların ihlal edilip edilmediği teşhis testleri (diagnostic tests) ile kontrol edilir.
## Normallik Varsayımı (Normality of Residuals)
Regresyon modelinden elde edilen hata terimlerinin (artıkların) ortalaması 0 olan normal bir dağılım göstermesi gerekir. Normallik ihlal edildiğinde hipotez testleri (T ve F testleri) güvenilirliğini kaybeder.
* Shapiro-Wilk Testi: Örneklem boyutu küçük ve orta büyüklükteki verilerde artıkların normalliğini test etmek için kullanılır.
* Q-Q Plot (Quantile-Quantile): Görsel olarak artıkların teorik normal dağılım çizgisine ne kadar uyduğunu gösterir.
Yorumlama: Shapiro-Wilk testinde $$p > 0.05$$ ise hataların normal dağıldığı ($$H_0$$) kabul edilir.
## Sabit Varyans / Eşvaryanslılık (Homoscedasticity)
Bağımsız değişkenin alacağı tüm değerler için hata terimlerinin varyansı sabit olmalıdır. Varyansın sabit olmaması durumuna Değişen Varyans (Heteroscedasticity) denir. Değişen varyans varlığında standart hatalar yanlış hesaplanır ve katsayılar güvenilmez hale gelir.
* Breusch-Pagan Testi: Hata varyansının bağımsız değişkenlerle sistematik bir ilişkisi olup olmadığını ölçer.
Yorumlama: Breusch-Pagan testinde $$p > 0.05$$ olması varyansın sabit olduğunu ($$H_0$$), yani modelin sağlıklı olduğunu gösterir.
## Otokorelasyon Olmaması (No Autocorrelation)
Hata terimlerinin birbirisinden bağımsız olması gerekir. Özellikle zaman serileri verilerinde, bir döneme ait hatanın bir sonraki dönemi etkilemesi durumuna otokorelasyon denir.
* Durbin-Watson Testi: Artıklar arasında birinci dereceden otokorelasyon olup olmadığını test eder.
Yorumlama: Durbin-Watson ($$DW$$) biyo-istatistik ve ekonometride kritik bir parametredir. $$DW$$ istatistiğinin 2'ye yakın bir değer alması otokorelasyon olmadığını gösterir. $$DW < 1.5$$ ise pozitif, $$DW > 2.5$$ ise negatif otokorelasyon riski mevcuttur.
## Çoklu Doğrusallık Olmaması (No Multicollinearity)
Çoklu regresyon modellerinde, bağımsız değişkenlerin birbiriyle yüksek düzeyde ilişkili (korelasyonlu) olmaması gerekir. Bağımsız değişkenler birbiriyle aşırı ilişkili olduğunda, model her bir değişkenin bağımlı değişken üzerindeki tekil etkisini ayırt edemez.
* VIF (Variance Inflation Factor - Varyans Şişirme Faktörü): Her bağımsız değişkenin modeldeki varyansı ne kadar artırdığını ölçer.
Yorumlama: Hesaplanan $$VIF$$ değerinin 5'in üzerinde olması orta düzeyde, 10'un üzerinde olması ise ciddi boyutta çoklu doğrusallık problemi olduğunu gösterir. VIF değeri yüksek çıkan değişkenler modelden çıkarılabilir veya dönüştürülebilir.

# Regresyon Analizinde Kestirim Yöntemleri ve Model Doğrulama
Bir regresyon modeli kurmanın temel amacı, eldeki verileri açıklamakla kalmayıp geleceğe veya görmediğimiz verilere dair doğru kestirimlerde (prediction) bulunmaktır. Ancak her veri yapısı aynı değildir; doğrusal olmayan ilişkiler, yüksek boyutlu veriler veya çoklu doğrusallık riski farklı kestirim yaklaşımlarını gerektirir.Bu yazıda, regresyon analizinde kullanılan temel kestirim yöntemlerini ve bu kestirimlerin başarısını ölçmek için uygulanan doğrulama tekniklerini inceliyoruz.
## Regresyon Kestirim Yöntemleri
Bağımlı değişkeni ($$Y$$) kestirirken verinin Karmaşıklığına ve boyutuna göre iki ana yaklaşım kullanılır:
### Parametrik Kestirim Yöntemleri
* En Küçük Kareler Yöntemi (Ordinary Least Squares - OLS):Klasik doğrusal regresyonun temelidir. Gerçek değerler ile kestirilen değerler arasındaki hata kareler toplamını ($SSE$) en aza indirmeyi amaçlar. Varsayımlar sağlandığında en verimli ve tarafsız ($BLUE$) kestirimleri sunar.
* Düzenlileştirilmiş (Regularized) Kestirim Yöntemleri:Çok fazla bağımsız değişken olduğunda veya değişkenler arasında yüksek korelasyon (çoklu doğrusallık) bulunduğunda OLS yöntemi veriyi ezberlemeye (overfitting) başlar. Bu durumda modele ceza terimi ekleyen yöntemler kullanılır:
*Ridge Regresyon ($L_2$ Penaltı): Katsayıları sıfıra yaklaştırır ancak tamamen sıfırlamaz. Çoklu doğrusallık varlığında kestirim varyansını düşürür.
*Lasso Regresyon ($L_1$ Penaltı): Önemsiz değişkenlerin katsayılarını tam olarak $$0$$ yapar. Kestirim yaparken aynı zamanda otomatik değişken seçimi (feature selection) sağlar.
* ElasticNet: Ridge ve Lasso'nun birleşimidir; hem ceza uygular hem de gruplanmış değişkenlerle başa çıkar.
### Esnek ve Eğrisel Kestirim Yöntemleri
* Polinom Regresyon (Polynomial Regression):Değişkenler arasındaki ilişki düz bir çizgi yerine eğrisel bir trend izlediğinde ($X^2, X^3$ gibi) yüksek dereceli terimler eklenerek kestirim gücü artırılır.
* Generalized Additive Models (GAM) / Splines:Veriyi parçalara bölerek her aralıkta esnek eğriler oturtan, katı doğrusallık kalıplarına uymayan karmaşık veri yapılarında yüksek kestirim başarısı gösteren parametrik olmayan yöntemlerdir.
### Kestirim Performansının Test Edilmesi (Model Validation)
Modelin başarısı, eğitildiği veri üzerindeki performansı ile değil, daha önce hiç görmediği veri (out-of-sample) üzerindeki kestirim doğruluğu ile ölçülür.<br>
Veri Bölümleme (Train / Test Split)Kestirim gücünü tarafsız sınamak için veri seti ikiye ayrılır:
* Eğitim Seti (%70 - %80): Modelin katsayılarını ve parametrelerini öğrenmek için kullanılır.
* Test Seti (%20 - %30): Modelin kestirim yeteneğini ölçmek üzere kilitli tutulur.
# Kestirim Hata Metrikleri
Kestirim modelinin başarısını ölçmek için kullanılan temel istatistiksel metrikler:
$$\text{MAE} = \frac{1}{n} \sum \vert{}y_i - \hat{y}_i\vert{}$$ <br>
$$\text{RMSE} = \sqrt{\frac{1}{n} \sum (y_i - \hat{y}_i)^2}$$ <br>
$$\text{MAPE} = \frac{100\%}{n} \sum \left\vert{} \frac{y_i - \hat{y}_i}{y_i} \right\vert{}$$ <br>
* MAE (Mean Absolute Error): Tahmin hatalarının mutlak ortalamasıdır. Yorumlaması kolaydır (gerçek birimle aynıdır).
* RMSE (Root Mean Squared Error): Hataların karesini aldığı için büyük kestirim hatalarını daha ağır cezalandırır.
* MAPE (Mean Absolute Percentage Error): Hatanın yüzde kaç olduğunu gösterir, ölçekten bağımsız karşılaştırma yapmaya yarar.



