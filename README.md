# redplace-uptime

[redplace.info](https://redplace.info) saytını oyaq saxlamaq üçün kiçik GitHub Actions cron-u.

Render free planı 15 dəqiqəlik hərəkətsizlikdən sonra servisi yatırır və servisin lokal
SQLite bazası sıfırlanır. Bu workflow hər 5 dəqiqədə sayta sorğu göndərir, beləcə servis
yatmir və sifarişlər/ayarlar qalır.

- `ping.yml` — əsas workflow (pulsuz, public repo üçün limitsiz Actions dəqiqəsi).
- `heartbeat.txt` — GitHub 60 gün repo fəaliyyətsizliyindən sonra cron-u söndürür;
  workflow hər ~20 gündə bu faylı yeniləyib aktivliyi saxlayır.

Bu repo heç bir sirr saxlamır.
