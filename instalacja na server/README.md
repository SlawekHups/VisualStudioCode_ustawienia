# Przenoszenie strony na server


1. Usuwanie developerskich paczek z projektu

`composer install --no-dev`

# ssh

1. SSH

`ssh hups@85.128.190.92 -p 22`

2. Kopiowanie i ustawienie pliku nazwa domeny, baza .env

`cd .env.example .env`

`vim .env`


3. Generowanie klucza w pliku .env

`php artisan key:generate`

4. Migracja bazy danych

`php artisan migrate`

5. Optymalizacja przy konfiguracji

a. przenosi wszystko z Vendor

`composer install --optimize-autoloader --no-dev`



`https://pomoc.lh.pl/zmiana-wersji-php`

- Optymalizacja
`php artisan route:cache`

`php artisan config:cache`

`php artisan view:cache`