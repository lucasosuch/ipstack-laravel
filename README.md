# skapel/ipstack-laravel Paketi Dokümantasyonu
Laravel uygulamalarında IPStack API'yi kullanmak için bir paket.

- [Gereklilikler](#gereklilikler)
- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Test](#test)
- [Güncellemeler](#güncellemeler)

## Gereklilikler

- PHP >= ^8.0
- Laravel >= ^10.0

## Kurulum

Install location using `composer require`:

```bash
composer require skapelapp/ipstack-laravel:dev-main
```

## Kullanım

<h4>Servis sağlayıcı ekleme</h4>

```php
'providers' => [
    // ...
    Skapelapp\IPStackLaravel\IPStackServiceProvider::class,
],
```

<h4>Facades</h4>

```php
'aliases' => [
    // ...
    'IPStack' => Skapelapp\IPStackLaravel\Facades\IPStackFacade::class,
],
```

<h4>Yapılandırma dosyalarını yayınlamak</h4>

```php
php artisan vendor:publish --tag=ipstack-config --force
```

## Test

```php
composer test
```

## Güncellemeler
Yeni sürümler ve güncellemeler hakkında bilgi almak için <a href="https://github.com/skapelapp/ipstack-laravel/releases">GitHub Release</a> sayfamızı kontrol edin.
