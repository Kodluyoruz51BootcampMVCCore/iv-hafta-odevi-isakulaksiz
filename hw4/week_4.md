# AddMvcCore Method:
MVC frameworkünü çalıştırabilmesi için minimun dependency eklemeye izin verir.Gerekli MVC servisleri için özel metodlarda eklenebilir.
Bu metodlar nelerdir?
-	ApplicationPartManager: Bir MVC uygulaması için controllerların listesini yönetmeyi sağlar.
-	DefaultFeatureProviders: Feature provider için controller ekler.
-	Default Services: Routing ekler.
-	CoreServices: Temel servisleri MVC framework için minimum dependency ile çalıştırır.
## AddMvc Method:
MVC framewokünü kullanabilmek için MVC project template izin vermek zorundasın.Bu method tüm dependencyleri projenin içersine ekler.
Bu metodlar nelerdir?
-	DataAnnotations: Data annotation modelini doğrulama ve süslemeye(decorate) izin verir.
Vb.

# Null Checker
-	İf(obj is null)
-	İf(!obj)

# First() vs FirstOrderDefault()
-	First() => Bir sıradan ilk elementi döndürür.
-	FirstOrderDefault() => Buda yine sıradan ilk elementi döndürür ama First()’e göre bir avantaja sahip o da eğer collectionda giriş kriterleriyle eşleşen bir kayıt yoksa FirstOrderDefault() null değeri işleyebilir ve bir exception atmaz.

# Single() vs SingleOrDefault()
-	Single() => Bir sıradan yalnızca bir eleman döndürür.Bunun anlamı collectionda herhangi bir kriterde sorguladığımızda veya collectiondaki kaydı filtrelediğimizde Single Extension metodu dizinin tek elemana sahip olmasını beklediği anlamına gelir.
-	SingleOrDefault() => Bir sıradan yalnızca bir eleman döndürür ama Single()’a göre avantaja sahiptir collectionda giriş kriterleriyle örtüşen bir kayıt yoksa SingleOrDefault() null değeri işleyebilir dahası bir exception fırlatmaz.