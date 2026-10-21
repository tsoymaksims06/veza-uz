ВЕЗА Узбекистан — сайт (RU / UZ / EN)

Состав:
  index.html      — страница сайта
  data.json       — каталог и решения (русский)
  data_uz.json    — каталог и решения (узбекский)
  data_en.json    — каталог и решения (английский)
  ph/             — все фотографии
  favicon.svg     — иконка вкладки

Сборка не нужна: это статичный сайт.

Публикация на Vercel:
  1. Создайте репозиторий на github.com (New repository) и загрузите
     в него содержимое этой папки (Add file → Upload files), без самой
     папки-обёртки: index.html должен лежать в корне репозитория.
  2. На vercel.com: Add New → Project → Import этот репозиторий.
     Framework Preset: Other. Ничего не меняйте, нажмите Deploy.
  3. Свой домен: Project → Settings → Domains → Add, затем пропишите
     у регистратора домена DNS-записи, которые покажет Vercel.

Проверить локально (нужен Python):
  python3 -m http.server 8000   →   http://localhost:8000
  (index.html двойным кликом не откроется полностью: каталог
   подгружается из json-файлов, браузеры блокируют это для file://)
