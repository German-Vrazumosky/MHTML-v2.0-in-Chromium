# MHTML-v2.0-in-Chromium
En:
Realization MHTML v2.0 for Chromium web browser based on Chromium MHTML v1.0 (1999) (RFC 2557) module.

Who owns the MHTML (MIME HTML) markup language, and why isn't anyone developing it? It hasn't been updated since 1999, when its standard was proposed in RFC 2557. This is a very important and necessary thing. I wanted to update it and propose my changes. They are simple:
- Add Unicode so that non-English content text isn't encoded, but left as is;
- Remove the 80-character (76 actual) line limit;
- Remove the line limit, line break, and line break with the "=" character;
- Make the EOL (line break) in Unix style - "\n" instead of the Windows style - "\r\n".

The changes are simple, but very important, because they improve the readability of the document code and reduce its size, which is very important.

For this purpose, I edited the `mhtml_archive.cc` file:
third_party/blink/renderer/platform/mhtml/mhtml_archive.cc
https://source.chromium.org/chromium/chromium/src/+/main:third_party/blink/renderer/platform/mhtml/mhtml_archive.cc

I would like to see MHTML v2.0 support added to Chromium and Google Chrome.

## Links
- [MHTML](https://en.wikipedia.org/wiki/MHTML)

---

Ru:
Реализация MHTML v2.0 для веб-браузера Chromium на основе модуля Chromium MHTML v1.0 (1999) (RFC 2557).

Кому принадлежит язык разметки MHTML (MIME HTML) и почему его никто не развивает? Никто его не обновлял с 1999 года, когда его стандарт предложили в RFC 2557. Это же очень важная и нужная вещь. Я хотел его обновить и предложить свои правки. Они простые:
- добавить Unicode, чтобы текст контента на отличном от английского языке не кодировался, а оставался как есть;
- убрать ограничение строки в 80 (76 реальных) симвлов;
- убрать лимит строки, разрыв и перенос строки символом "=";
- EOL (перенос строки) сделать в Unix стиле - "\n", вместо стиля Windows - "\r\n".

Изменения простые, но очень важные, потому что улучшат читаемость кода документа и уменьшат его размер, что очень важно.

Для этого мной был отредактирован файл `mhtml_archive.cc`:
third_party/blink/renderer/platform/mhtml/mhtml_archive.cc
https://source.chromium.org/chromium/chromium/src/+/main:third_party/blink/renderer/platform/mhtml/mhtml_archive.cc

Хотелось бы, чтобы поддержку MHTML v2.0 добавили в Chromium и Google Chrome.

## Ссылки
- [MHTML](https://ru.wikipedia.org/wiki/MHTML)
