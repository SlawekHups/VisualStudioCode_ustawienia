# VisualStudioCode_ustawienia

1. Active File In Status Bar
`roscop.activefileinstatusbar`
2. Blade formatter for VS Code
`apility.beautify-blade`
3. Bracket Pair Colorizer 2
`coenraads.bracket-pair-colorizer-2`
4. CSS Peek
`pranaygp.vscode-css-peek`
5. Edit csv
`janisdd.vscode-edit-csv`
6. EditorConfig for VS Code
`editorconfig.editorconfig`
7. helloCode
`hellocodepublisher.hellocode`
8. Image preview
`kisstkondoros.vscode-gutter-preview`
9. Image Resizer - Resize from the menu
`lukapetrovic.image-resizer`
10. Image To Base64 clipboard
`green-csv.img-contextual`
11. IntelliSense for CSS class names in HTML
`zignd.html-css-class-completion`
12. Jira and Bitbucket (Atlassian Labs)
`atlassian.atlascode`
13. Laravel Blade Snippets
`onecentlin.laravel-blade`
14. Material Icon Theme
`pkief.material-icon-theme`
15. Mithril Emmet
`fallenmax.mithril-emmet`
16. Path Intellisense
`christian-kohler.path-intellisense`
17. PHP Intelephense
`bmewburn.vscode-intelephense-client`
18. Polacode
`fy.polacode-with-copy`
19. Polacode-2020
`jeff-hykin.polacode-2019`
20. Polish Language Pack for Visual Studio Code
`ms-ceintl.vscode-language-pack-pl`
21. Prettier - Code formatter
`esbenp.prettier-vscode`
22. Prettier - Code formatter
`esbenp.prettier-vscode`
23. TODO Highlight
`wayou.vscode-todo-highlight`
24. Unofficial ClearCase SCM Commands
`openningia.vscode-clearcase`
25. Vetur
`octref.vetur`
26. YAML
`redhat.vscode-yaml`
27. Polacode
`pnp.polacode`




###


PRZY PIERWSZYM URUCHOMIENIU PROJEKTU NA NOWYM  RODOWISKU
UMIE   KOD W MIEJSCU DOCELOWYM
Możesz wykorzysta  do tego celu GITa lub sFTP Pamiętaj, że domena musi wskazywa  na folder public
Pozostała część aplikacji powinna by  niedostępna z zewnątrz
CP .ENV.EXAMPLE .ENV
Uruchom komendę będąc w folderze gł wym aplikacji
Powstawnie nowy plik .env na bazie szablonu, gdzie uzupełnij koniecznie dostęp do bazy danych oraz parametry APP_URL i APP_NAME
COMPOSER INSTALL --NO-DEV
Ta komenda zainstaluje wszystkie dodatkowe biblioteki, od kt rych zależna jest nasza aplikacja
Możesz doda  dodatkowy parametr --optimize-autoloader by poprawi  szybko   działania
PHP ARTISAN MIGRATE --SEED
Ta komenda stworzy wszystkie tabele w bazie danych na bazie plik w migracji w Twoim projekcie
Parametr --seed uruchomi od razu wszystkie seedery zdefiniowane w DatabaseSeeder
Dobrą praktyką jest wrzucenie podstawowej konfiguracji, tabel słownikowych i użytkownika/admina wła nie przez seedery
        
 5. PHP ARTISAN KEY:GENERATE

Ta komenda wygeneruje unikatowy klucz aplikacji,
niezbędny do prawidłowego działania
Bez jej wykonania odwiedzenie jakiejkolwiek strony aplikacji będzie skutkowa  błędem

6. PHP ARTISAN STORAGE:LINK
Tę komendę uruchom wtedy, gdy w aplikacji umożliwiasz upload plik w, kt re p  niej mają by  dostępne publicznie (np. avatar użytkownika)
Powstawnie link symboliczny do folderu storage/public

7. UPEWNIJ SIĘ, ŻE APLIKACJA DZIAŁA POPRAWNIE To pierwsze uruchomienie aplikacji w nowym  rodowisku
Przeklinaj aplikację i upewnij się, że na pierwszy rzut oka działa poprawnie, po czym przejd  do kolejnych krok w

8. USTAW TRYB PRODUKCYJNY
Otw rz plik .env i ustaw parametry:
APP_ENV=production APP_DEBUG=false
Teraz aplikacja działa i można z niej bezpiecznie korzysta

9. CACHE (ZALECANE)
Ostatnim krokiem (opcjonalnym, cho  zalecanym) jest
stworzenie cache widok w, routingu i konfiguracji
Wykonaj takie trzy komendy:
php artisan config:cache php artisan route:cache php artisan view:cache


















