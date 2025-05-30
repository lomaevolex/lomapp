# lomapp

macOS-приложение на **SwiftUI** для встраивания цифрового отпечатка в файл и проверки его целостности.

## 🧩 Возможности

- **Загрузка контейнера**: выбирайте любой файл для обработки.  
- **Методы отпечатка**:  
  - **SHA-256** (хеш-функция)  
  - **HMAC-SHA256** (аутентификация с ключом)  
  - **Модификация структуры файла**  
  - **Встраивание в ресурсы/код**  
- **Вставить и сохранить**: встраивает отпечаток и сохраняет новый файл.  
- **Проверить**: проверяет корректность отпечатка.  
- **Логи**: отображение истории действий с возможностью очистки.  
- **Настройки**:  
  - 🌙 **Dark Mode**  
  - 🎨 **Accent Color**  

## 🛠️ Технологии

- **Язык:** Swift 5  
- **UI:** SwiftUI, AppKit (NSOpenPanel, NSSavePanel)  
- **Крипто:** CryptoKit (SHA-256, HMAC)  
- **Хранилище ключей:** Keychain API  
- **Логирование:** FileManager, Swift `Logger`  
- **Тестирование:** XCTest (Unit & UI)  

## ⚙️ Использование

1. Нажмите **Загрузить контейнер** и выберите файл `.data` или любой бинарный.  
2. В выпадающем меню **Алгоритм** выберите нужный метод вставки отпечатка:  
   - SHA-256  
   - HMAC  
   - Модификация структуры  
   - Встраивание в ресурсы/код  
3. Нажмите **Вставить и сохранить** (или используйте сочетание клавиш ⌘S), чтобы встроить отпечаток и сохранить новый файл.  
4. Нажмите **Проверить** (или ⌘T), чтобы проверить корректность отпечатка.  
5. Результат проверки отобразится под кнопками в виде зелёной галочки (✔) или красного креста (✘).  
6. Панель **Логи** отображает историю всех операций.  
7. Кнопка **Очистить** сбрасывает содержимое логов.  
8. В меню **Настройки** можно:  
   - включить/отключить тёмный режим  
   - выбрать цвет акцентов интерфейса
