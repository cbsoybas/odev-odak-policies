# Ödev Odak Gizlilik Politikası

**Yürürlük tarihi:** 15.09.2026  
**Son güncelleme:** 15.09.2026  
**Veri sorumlusu / yayıncı:** Ödev Odak geliştiricisi (GitHub: cbsoybas)  
**İletişim:** [stair-stake1g@icloud.com](stair-stake1g@icloud.com)

Bu Gizlilik Politikası, Ödev Odak adlı iPhone ve iPad uygulamasının ("Uygulama") hangi kişisel verileri, hangi amaçlarla ve hangi hizmet sağlayıcılar aracılığıyla işlediğini açıklar. Uygulamayı kullanarak bu metni okuduğunuzu kabul edersiniz. Zorunlu olmayan özellikler için ayrıca gösterilen izin ve onaylar bu metnin yerine geçmez; ilgili özellik kullanılmadan önce ayrı onay alınır.

Bu metin bir hukuk danışmanlığı değildir. Yayından önce veri sorumlusu, iletişim bilgileri, saklama süreleri ve hedef kullanıcı yaşı gerçek uygulama yapılandırmasıyla karşılaştırılmalı ve gerekiyorsa hukuk danışmanı tarafından incelenmelidir.

## 1. Uygulama ne yapar?

Ödev Odak; ödevleri cihazda takip etmeye, isteğe bağlı olarak Google Classroom’dan içe aktarmaya, ödevlerin tamamlanma durumunu izlemeye, seçilen uygulamalar için kişisel odak sınırı uygulamaya ve kullanıcının seçtiği ödev fotoğrafları üzerinde otomatik bir tamamlama kontrolü çalıştırmaya yarar.

Uygulama, ödevin gerçekten kullanıcı tarafından yapıldığını, cevapların doğru olduğunu, fotoğrafın yeni çekildiğini veya bir fotoğrafta ödevin bütün sayfalarının bulunduğunu kesin olarak doğrulamaz. Fotoğraf sonucu yalnızca yardımcı bir değerlendirmedir.

## 2. İşlenen veri kategorileri

### 2.1. Hesap ve oturum bilgileri

Apple veya Google ile giriş yaptığınızda aşağıdaki bilgiler, sağlayıcının ve Supabase Auth yapılandırmasının izin verdiği ölçüde işlenebilir:

- Supabase kullanıcı kimliği;
- giriş sağlayıcısı bilgisi (Apple veya Google);
- sağlayıcı tarafından paylaşılan e-posta adresi veya Apple’ın e-posta gizleme adresi;
- görünen ad ve hesapla ilişkilendirilen temel profil bilgileri;
- oturum, erişim ve yenileme belirteçleri.

Oturum belirteçleri Uygulamanın güvenli Keychain alanında tutulur. Google Classroom bağlantısı için alınan Google erişim belirteci, ana Ödev Odak hesabından ayrı ve hesapla ilişkilendirilmiş bir Keychain kaydında tutulur. Classroom hesabı ana hesabınızın yerine geçmez ve bulut yedeğinin hesabını değiştirmez.

### 2.2. Ödev verileri

Elle girdiğiniz, fotoğraftan okuttuğunuz veya Classroom’dan içe aktardığınız şu bilgiler işlenebilir:

- ödev adı, ders adı, açıklama ve teslim tarihi;
- kaynak bilgisi (elle, fotoğraf veya Classroom);
- Classroom ödev kimliği, bağlantısı ve teslim durumu;
- tamamlandı, Classroom’da teslim edildi veya fotoğrafla doğrulandı gibi durumlar;
- doğrulama sonucu, sonuç açıklaması ve zaman bilgisi;
- çöp kutusu ve düzenleme durumları.

Fotoğraftan ödev eklerken metin, mümkün olduğu ölçüde Apple Vision ile cihaz üzerinde okunur. Kaydetmeden önce okunan metni değiştirebilir veya fotoğrafı iptal edebilirsiniz.

### 2.3. Ödev fotoğrafları ve fotoğraf kontrolü

Fotoğrafla kontrolü siz başlatır, gönderilecek fotoğrafları siz seçer ve gönderim düğmesine basmadan önce açık onay verirsiniz. Uygulama bir kontrolde en fazla dört fotoğraf gönderir. Fotoğraf ve ödev bilgileri, kontrol için HTTPS üzerinden kendi sunucu işlevimize ve yapılandırılmış üçüncü taraf yapay zekâ sağlayıcısına iletilebilir.

Fotoğraflar mevcut sunucu uygulamasında kalıcı ödev yedeğine eklenmez ve sunucunun geçici istek belleği dışında diske yazılmaması hedeflenir. Bununla birlikte ağ iletimi, barındırma günlükleri, hata kayıtları veya üçüncü taraf sağlayıcının kendi işleme kuralları üzerinde mutlak kontrol garanti edilemez. Fotoğrafta yüz, okul numarası, adres, iletişim bilgisi veya başka bir kişisel bilgi göstermeyin.

### 2.4. Google Classroom verileri

Classroom’u bağladığınızda yalnızca seçtiğiniz izinlerin kapsamındaki ders, ödev, teslim tarihi, açıklama, ders adı, Classroom bağlantısı ve size ait öğrenci teslim durumu alınır. Uygulama öğretmenlerin veya diğer öğrencilerin size ait olmayan verilerini istemez. Google’ın veri işleme ve gizlilik kuralları da uygulanır: [Google Gizlilik Politikası](https://policies.google.com/privacy).

Uygulama açıkken Classroom eşitlemesi yaklaşık dakikada bir ve uygulama yeniden öne geldiğinde yapılır. Uygulama tamamen kapalıyken arka planda sürekli eşitleme yapılmaz. Classroom’da teslim edilmiş görünen ödev, Uygulamada teslim edilmiş sayılır; fotoğrafla doğrulama yapılmadıysa bu durum ayrıca gösterilir.

### 2.5. Bulut yedeği

Giriş yapan kullanıcı için ödev kayıtlarının bir kopyası, kullanıcının Supabase hesabına bağlı `homework_backups` kaydında tutulabilir. Bu yedek ödev metadatasını ve durumlarını içerir; fotoğraf doğrulama fotoğrafları bu yedeğe eklenmez. Yedekleme ana Ödev Odak hesabına yapılır, Classroom hesabına yapılmaz.

Supabase Auth, veritabanı ve RPC işlevleri kullanılır. Supabase’in güvenlik ve veri işleme belgeleri için [Supabase Gizlilik Politikası](https://supabase.com/privacy) ve [Supabase belgeleri](https://supabase.com/docs/guides/auth) incelenmelidir.

### 2.6. Ebeveyn bağlantısı

İsteğe bağlı ebeveyn bağlantısını iki hesap da onayladığında aşağıdaki bilgiler paylaşılabilir:

- bağlantıdaki kişilerin uygulama içinde seçtiği görünen ad;
- ödev adı, ders, açıklama, teslim tarihi, çöp kutusu ve Classroom teslim durumu;
- fotoğrafla doğrulandı/doğrulanmadı durumu ve doğrulama açıklaması;
- cihazın odak sınırının uygulandığını gösteren sınırlı durum metni;
- ebeveyn tarafından gönderilen ödev düzenleme veya odak komutları.

Fotoğraflar, Classroom erişim belirteçleri ve cihazda seçilen uygulama/kategori belirteçleri ebeveyne gönderilmez. Ebeveyn bağlantısı sonlandırılabilir; sonlandırma sonrasında yeni paylaşım ve komut eşitlemesi durdurulur.

### 2.7. Ekran Süresi ve cihaz izinleri

Odak modu için seçtiğiniz uygulama, kategori ve web alanı seçimleri Apple FamilyControls ve DeviceActivity çerçeveleri aracılığıyla cihazda kullanılır. Uygulama bu seçimlerin adlarını veya içerik geçmişini sunucuda tutmayı amaçlamaz. Kamera, bildirim ve Ekran Süresi izinleri yalnızca ilgili özelliği çalıştırmak için istenir.

## 3. Amaçlar ve hukuki dayanaklar

Veriler aşağıdaki amaçlarla, uygulanabilir yerel hukuka göre gerekli hukuki dayanakla işlenir:

- hesabı oluşturmak, oturum açtırmak ve hesabı güvenli tutmak;
- ödevleri cihazda göstermek, düzenlemek, silmek ve yedeklemek;
- açıkça istediğiniz Classroom eşitlemesini yürütmek;
- siz başlattığınızda fotoğraf kontrolünü gerçekleştirmek;
- ebeveyn bağlantısını ve hesaplar arasındaki onaylı komutları yürütmek;
- kota, kötüye kullanım, hata ayıklama ve güvenlik kontrollerini yapmak;
- yasal yükümlülüklere uymak ve uyuşmazlıkları yönetmek.

Zorunlu olmayan fotoğraf kontrolü, Classroom, bulut yedeği, ebeveyn bağlantısı ve odak izni özelliklerini kullanıp kullanmamak size bırakılır. İzin vermediğinizde bu özellik çalışmaz; temel ödev takibi cihazda kullanılabilir.

## 4. Gemini ve yapay zekâ sağlayıcısı hakkında özel açıklama

Fotoğraf kontrolünde kullanılan sağlayıcı, Uygulamanın o tarihteki sunucu yapılandırmasına göre Google Gemini veya başka bir uygun sağlayıcı olabilir. Fotoğraf göndermeden önce sağlayıcı adı ve gönderimin amacı Uygulamada açıkça gösterilir.

Gemini API’nin güncel ek şartları, API’yi kullanan kişinin 18 yaşında veya daha büyük olmasını ve API istemcisinin 18 yaş altına yönelik veya bu kişilerin erişmesinin muhtemel olduğu bir hizmet olarak kullanılmamasını şart koşmaktadır. Bu nedenle:

1. Gemini ile fotoğraf kontrolünü başlatırken **18 yaşında veya daha büyük olduğunuzu ve bu özelliği kullanmaya yetkili olduğunuzu beyan etmeniz gerekir**.
2. Bu beyan bir kimlik, yüz veya biyometrik yaş doğrulaması değildir. Uygulama Gemini’nin fotoğraftan yaşınızı kesin olarak doğruladığını iddia etmez.
3. 18 yaşından küçükseniz veya yaş şartını karşılayıp karşılamadığınızdan emin değilseniz Gemini tabanlı fotoğraf kontrolünü kullanmayın.
4. Uygulama çocuklara veya 18 yaş altı öğrencilere yönelik bir dağıtımda Gemini API’sini kullanmadan önce sağlayıcının güncel şartları yeniden incelenmeli; gerekiyorsa özellik devre dışı bırakılmalı veya uygun bir sağlayıcı kullanılmalıdır.

Gemini ile ilgili güncel şartlar: [Gemini API Additional Terms](https://ai.google.dev/gemini-api/terms). Sağlayıcıya gönderilen içerik, Google’ın ilgili şartları ve gizlilik belgelerine de tabidir. Teknik bir metni Kullanım Koşulları’na eklemek, sağlayıcının yaş veya hedef kitle şartlarını değiştirmez.

## 5. Verilerin paylaşılabileceği taraflar

Veriler yalnızca işlevin gerektirdiği ölçüde şu taraflara aktarılabilir:

- Supabase: kimlik doğrulama, güvenli veritabanı, RPC ve bulut yedeği;
- Google: Google hesabı, Google Classroom API’si ve seçtiğiniz yapay zekâ sağlayıcısı Gemini ise fotoğraf kontrolü;
- Apple: Sign in with Apple, Keychain, Vision ve FamilyControls/DeviceActivity işletim sistemi hizmetleri;
- Uygulamanın barındırma, hata izleme veya e-posta/destek hizmeti sağlayıcıları, yalnızca gerçekten yapılandırılmışsa;
- kanunen yetkili kamu kurumları veya geçerli hukuki taleplerde yetkili danışmanlar.

Veriler reklam profili oluşturmak veya satılmak amacıyla paylaşılmaz. Gerçek yapılandırmada kullanılmayan bir sağlayıcı bu metinde aktif hizmet olarak değerlendirilmemelidir.

## 6. Saklama süreleri ve silme

- Hesap ve bulut yedeği, hesap açık kaldığı ve hizmeti sağlamak gerektiği sürece tutulur.
- Cihazdaki ödevler, siz silene, uygulamayı kaldırana veya hesabınızı silene kadar cihazda kalabilir.
- Fotoğraf kontrolü için gönderilen görüntüler kalıcı ödev yedeğine eklenmez; geçici işleme, teknik günlük ve üçüncü taraf saklama süresi sağlayıcının yapılandırmasına göre değişebilir.
- Ebeveyn bağlantısının verileri bağlantı sonlandırılınca yeni paylaşıma kapatılır; yasal, güvenlik veya yedekleme gerekleri için tutulması gereken kayıtlar ilgili süre sonunda silinir.
- Hesap silme işlemi Ayarlar → Hesabı sil bölümünden başlatılabilir. İşlem Supabase hesabını, bu hesaba ait bulut yedeğini, aile bağlantılarını ve uygulamanın cihazdaki hesap verilerini siler. Classroom’daki veriler Google hesabında kaldığından Google Classroom’dan ayrıca silinmelidir.

Silinen veriler yedeklerden, günlüklerden veya yasal kayıt sistemlerinden hemen ve fiziksel olarak aynı anda yok olmayabilir; bu kayıtlar yalnızca gerekli süre boyunca korunur ve sonrasında silinir veya anonimleştirilir.

## 7. Güvenlik

Aktarımda HTTPS, oturumlarda Supabase Auth ve cihazdaki oturum bilgilerinde Keychain kullanılır. Erişim yetkileri kullanıcı hesabıyla sınırlandırılmaya ve aile verileri yalnızca onaylı bağlantıya açılmaya çalışılır. İnternet üzerinden hiçbir sistem mutlak güvenlik garantisi veremez; cihazınızı, Apple/Google hesabınızı ve doğrulama bilgilerinizi korumak sizin sorumluluğunuzdadır.

## 8. Haklarınız ve talepleriniz

Uygulanabilir hukuka göre kişisel verilerinize erişme, düzeltme, silme, işlemeyi kısıtlama, itiraz etme, veri taşınabilirliği ve verdiğiniz onayı geri çekme haklarına sahip olabilirsiniz. Talep için [stair-stake1g@icloud.com](stair-stake1g@icloud.com) adresine yazabilirsiniz. Talebinizi yerine getirebilmek için hesap sahipliği doğrulaması istenebilir.

## 9. Çocuklar ve yaş sınırlamaları

Uygulamanın temel ödev listesi ile Gemini fotoğraf kontrolü aynı yaş ve hizmet koşullarına tabi değildir. Gemini özelliği için yukarıdaki 18+ beyanı zorunludur. Uygulama 18 yaş altı kişilerce kullanılacaksa veli/ebeveyn bağlantısı, Apple’ın çocuk hesabı kuralları, Google Classroom okul politikaları ve kullanılan yapay zekâ sağlayıcısının güncel koşulları ayrıca değerlendirilmelidir. Bu belge, 18 yaş altı bir kullanıcının Gemini hizmetini kullanmasına izin vermez.

## 10. Politika değişiklikleri

Hizmet, sağlayıcılar veya mevzuat değiştiğinde bu politikayı güncelleyebiliriz. Güncel sürüm uygulamada ve [Gizlilik Politikası sayfasında](https://github.com/cbsoybas/odev-odak-policies/blob/main/GIZLILIK_POLITIKASI.md) yayınlanır. Önemli değişikliklerde, uygulanabilir hukuka göre uygulama içi bildirim veya yeniden onay istenebilir.

## 11. İletişim

Gizlilik soruları, veri talepleri ve silme talepleri için:

**Veri sorumlusu:** Ödev Odak geliştiricisi (GitHub: cbsoybas)  
**İletişim:** [stair-stake1g@icloud.com](stair-stake1g@icloud.com)
**Gizlilik politikası URL’si:** https://github.com/cbsoybas/odev-odak-policies/blob/main/GIZLILIK_POLITIKASI.md
```
