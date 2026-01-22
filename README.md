## Сборка прошивок Padavan на серверах GitHub

Для личного использования

Каталог [`configs.release`](configs.release) содержит конфигурации маршрутизаторов для сборки публичных релизов

Создание публичного релиза прошивок: [Actions](../../actions) → [Make firmware releases](../../actions/workflows/make_release.yml)

Создание публичного релиза toolchain: [Actions](../../actions) → [Make toolchain release](../../actions/workflows/make_toolchain_release.yml)

Каталог [`configs.build`](configs.build) содержит конфигурации маршрутизаторов для сборки прошивок в артефактах

Создание артефактов: [Actions](../../actions) → [Build firmware](../../actions/workflows/build.yml)

В файле [`variables`](variables) указывается репозиторий прошивки, ветка, конкретный тег или коммит, ссылка на заранее собранный toolchain для экономии времени компиляции прошивки.
Если ссылку на toolchain не указывать, то он будет скомпилирован перед сборкой прошивки.