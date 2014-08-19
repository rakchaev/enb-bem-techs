История изменений
=================

0.1.0
-----

Для версии `0.1.0` история изменений описана по отношению к пакету `enb@0.13.x`.

### Изменения, ломающие обратную совместимость

* Технологии `bemdecl-from-bemjson`, `bemdecl-from-deps-by-tech` и `bemdecl-merge` теперь предоставляют результат в `bemdecl` формате, вместо `deps` формата.
* Технологии `deps` и `deps-old` теперь ожидают от `bemdecl`-таргетов результаты в `bemdecl` формате.

### Крупные изменения

* Удалена вся логика, связанная с `BEViS` методологией.
* Технология `bemdecl-merge` переименована в `merge-bemdecl`.
* Технология `deps-merge` переименована в `merge-deps`.
* Технология `deps-subtract` переименована в `subtract-deps`.
* Технология `bemdecl-provider` переименована в `provide-bemdecl`.
* Технология `deps-provider` переименована в `provide-deps`.
* Опции `sourceTarget` и `destTarget` из `bemdecl-from-bemjson` технологии объявлены как **deprecated**, вместо них следует использовать `source` и `target` соответственно.
* Опции `bemdeclSources` и `bemdeclTarget` из `merge-bemdecl` технологии объявлены как **deprecated**, вместо них следует использовать `sources` и `target` соответственно.
* Опции `sourceNodePath`, `sourceTarget` и `bemdeclTarget` из `provide-bemdecl` технологии объявлены как **deprecated**, вместо них следует использовать `node`, `source` и `target` соответственно.
* Опции `bemdeclTarget` и `depsTarget` из `deps` технологии объявлены как **deprecated**, вместо них следует использовать `sourceDepsFile` и `target` соответственно.
* Опции `depsSources` и `depsTarget` из `merge-deps` технологии объявлены как **deprecated**, вместо них следует использовать `sources` и `target` соответственно.
* Опции `bemdeclTarget` и `depsTarget` из `deps-old` технологии объявлены как **deprecated**, вместо них следует использовать `sourceDepsFile` и `target` соответственно.
* Опции `sourceNodePath`, `sourceTarget` и `depsTarget` из `provide-deps` технологии объявлены как **deprecated**, вместо них следует использовать `node`, `source` и `target` соответственно.
* Опции `subtractFromTarget`, `subtractWhatTarget` и `depsTarget` из `subtract-deps` технологии объявлены как **deprecated**, вместо них следует использовать `from`, `what` и `target` соответственно.
* Опция `depsTarget` из `files` технологии объявлена как **deprecated**, вместо неё следует использовать `depsFile`.
* Опция `sublevelDirectories` из `levels` технологии объявлена как **deprecated**.
* Добавлена опция `format` для `deps` и `deps-old` технологий.

### Также в релиз вошли следующие изменения

* Исправлена ошибка в `deps` и `deps-old` технологиях, из-за которой было невозможно выразить булевый модификатор со значением `true` в `deps` формате.
* Модуль `vow` обновлён до версии `0.4.5`.
* Модуль `inherit` обновлён до версии `2.2.2`.
* Модуль `js-yaml` обновлён до версии `3.1.0`.