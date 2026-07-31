https://www.linkedin.com/in/alekseirozhkov/
https://github.com/arozhkovru

# Hardlink vs Symlink
- **Жесткая ссылка (Hardlink):** Это дополнительное имя для уже существующего файла. Она указывает напрямую на индексный дескриптор файла (`inode`), который содержит метаданные и указатели на физические блоки данных на диске. Оригинальный файл и жесткая ссылка абсолютно равноправны.
- **Символическая ссылка (Symlink):** Это отдельный, самостоятельный файл, который содержит в себе путь (текстовую строку) к целевому файлу или директории. У нее есть собственный, уникальный `inode`.

# Most usefull Linux.Filesystem commands
```
# Create directory with all nested directories
sudo mkdir -p /home/dir1/dir2
```