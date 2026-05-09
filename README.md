# NR BAZAR (Render Disk)

Одна страница: **ПОКУПАЮ / ПРОДАЮ** → форма → данные в **CSV** + фото (только для "ПРОДАЮ") в папку **uploads** на Render Persistent Disk.

## Render Disk
Render → Settings → Disks → Add Disk:
- Mount path: `/var/data`

Env vars:
- `DATA_DIR=/var/data/data`
- `UPLOADS_DIR=/var/data/uploads`
- `SECRET_KEY=...`
- (опционально) `ADMIN_KEY=...` для админки

## Где данные
- CSV: `DATA_DIR/submissions.csv`
- Фото (только ПРОДАЮ): `UPLOADS_DIR/<ID>/...`

## Поля формы
- **Название**
- **Стоимость**
- **Ваш контакт**
- **Описание**
- **Фото** (только для ПРОДАЮ, до 5)
