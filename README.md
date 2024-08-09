## State Yönetimi 

- State : uygulamadaki bileşenlerin sahip olduğu bilgi ve özelliklerdir.

- Props Drilling: Bileşenlerin yukarıdan (parent component) aşağıya (child component) veri taşımasıdır.

- Context: Uygulamadaki state'i bütün bileşenler tarafından erişilebilen ve oluşturduğumuz merkezlerden yönettiğimiz state yönetim aracıdır. Birden fazla merkez var.

- Redux : Bileşenlerin sahip olduğu ve merkezi olarak tutulması gereken statelerin yönetildiği merkezi state yönetim aracıdır. Tek merkezi state vardır.

## Neden Context Yerine Redux?

- Kod tekrarını önler
- Performansı daha iyidir
- Bileşenler içerisindeki karışıklığı azaltır.
- Hata ayıklama daha kolaydır.
- Orta ve büyük ölçekli projelerde state yönetimini daha kolay hale getirir.

## Kütüphaneler
- bootstrap
- json-server
- react-redux
- redux
- uuid

# Redux ile ilgili bilinmesi gerekenler 

1. Store : uygulamanın bütün bileşenleri tarafından erişilebilen ve yönetilebilen state deposu 
2. Reducer : aksiyondan aldığı talimata (emir) göre store'da tutulan state'in nasıl değişeceğine karar veren fonksiyondur.
3. Action (emir , haber, talimat) : Store'daki state'i güncellemek için reducer'a gönderdiğimiz nesnedir.

-- Action iki değerli bir nesne döndürür.
- TYPE : zorunludur. Actionun görevini tanımlayan bir string değerdir.
- PAYLOAD : opsiyoneldir. Actionun verisidir.