# Binance Motion Pack

В папке [`video/`](video/) лежат 41 готовый ролик MP4 H.264, 1920×1080, 30 FPS. Эти MP4 хранятся в Git как обычные файлы: скачивайте отдельные ролики через **Download** или получите их вместе через **Code → Download ZIP**.

В `video/` также находятся монтажные маски MP4 и прозрачные слои MOV ProRes 4444. Файлы MOV предназначены для видеомонтажа и наложения альфа-канала; стандартный проигрыватель Windows может не воспроизводить ProRes. Они хранятся через Git LFS.

Для скачивания содержимого LFS-роликов используйте Git LFS:

```sh
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/murdegun/Video-gener.git
cd Video-gener
git lfs pull --include="video/**/*.mov" --exclude=""
```

[Папка с видео на GitHub](https://github.com/murdegun/Video-gener/tree/main/video). Полный исходный архив проекта также оставлен в корне репозитория; его SHA-256: `0de7c9f49d5405d6bc608b3be82856e3cac3770f0144ec26a351954a03434de8`.
