# RickAndMorty.WebApi

RickAndMorty.WebApi, popüler Rick and Morty API'sini kullanarak karakterleri ve bölümleri çekip yerel bir veritabanına kaydeden bir ASP.NET Core Web API projesidir. Proje aynı zamanda bu veritabanından verileri sorgulama ve alma yetenekleri sağlar.

## Proje Yapısı

### 1. Models
- **Character**: Rick and Morty karakterlerinin temel özelliklerini içeren model.
- **Episode**: Dizinin bölümleri hakkında bilgileri içeren model.
- **EpisodeCharacter**: Karakterlerin hangi bölümlerde göründüğünü tanımlayan ilişki modeli.
- **Location**: Karakterlerin bulundukları yerlerin bilgilerini içeren model.
- **Origin**: Karakterlerin kökenlerine ait bilgileri içeren model.

### 2. Controllers
- **ValuesController**: Rick and Morty API'sinden veri çeken ve bunları veritabanına kaydeden, aynı zamanda bu verileri dönen kontrolör.

## Kullanılan Teknolojiler ve Kütüphaneler
- **ASP.NET Core Web API**
- **Entity Framework Core**: Veritabanı işlemleri için kullanılır.
- **Swashbuckle (Swagger)**: API dokümantasyonu için kullanılır.
- **Microsoft.EntityFrameworkCore.SqlServer**: SQL Server için Entity Framework Core sağlayıcısı.

## API Uç Noktaları

### `GET api/values/GetAllUsingRickAndMortyAPI`
Rick and Morty API'sinden bölümleri ve karakterleri çeker, veritabanına kaydeder.

### `GET api/values/GetAllEpisode`
Veritabanındaki tüm bölümleri, ilgili karakterlerle birlikte getirir.

### `GET api/values/GetAllCharacter`
Veritabanındaki tüm karakterleri getirir.

