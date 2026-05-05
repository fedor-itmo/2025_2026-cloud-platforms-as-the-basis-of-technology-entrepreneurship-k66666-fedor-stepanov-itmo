University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2025/2026  
Group: K66666  
Author: Stepanov Fedor  
Lab: Lab3  
Date of create: 05.05.2026  
Date of finished: 05.05.2026

# Лабораторная работа №3
## Исследование Cloud Storage

## Цель работы
Изучить создание и настройку бакета, работу с объектами, перемещение файлов в «папку», публикацию и удаление ресурсов.

## Ход работы
1. Создан бакет `fstepanov-lab3-bucket` в Cloud Storage.
2. В бакет загружены изображения `111.jpg`, `222.jpg`, `333.jpg`.
3. Создана папка (префикс) `lsllslslsl/` и файлы перемещены внутрь нее.
4. Для бакета снято ограничение public access prevention и добавлен доступ `allUsers`.
5. Через контекстное меню получены публичные URL файлов.
6. После проверки доступности и структуры хранения бакет удален.

## Скриншоты
### Создание и начальное состояние бакета
![Create bucket wizard](../images/img21.png)
![Bucket created and empty](../images/img22.png)

### Работа с файлами и папкой
![Objects uploaded](../images/img23.png)
![Create folder dialog](../images/img24.png)
![Folder and files in resource hierarchy](../images/img25.png)
![Move operation in context menu](../images/img26.png)
![Folder appears in objects list](../images/img27.png)
![Files moved into folder](../images/img28.png)
![Local preview of uploaded files](../images/img29.png)

### Публичный доступ
![Copy public URL option](../images/img30.png)
![Disable public access prevention](../images/img31.png)
![Grant allUsers role](../images/img32.png)
![Access granted to public principals](../images/img33.png)

### Удаление ресурсов
![Delete bucket confirmation](../images/img34.png)

## Выводы
- В Cloud Storage «папки» реализуются через префиксы имен объектов, а не через отдельную файловую иерархию.
- Для публикации контента нужно корректно настроить как ограничение public access prevention, так и IAM-доступ `allUsers`.
- После выполнения лабораторной важно удалять бакет и связанные ресурсы для контроля затрат и безопасности.
