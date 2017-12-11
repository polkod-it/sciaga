## Zmiana kontekstu rekursywnie w całym folderze
```
chcon -Rv --type=httpd_sys_rw_content_t /var/www
```
## Odtworzenie kontekstu 
```
restorecon -v /var/www/*
```
## Ustawienie wartości zmiennej
```
setsebool -P httpd_read_user_content 1
```
