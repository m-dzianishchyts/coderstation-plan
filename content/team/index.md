---
title: Команда
---

На этой странице описаны структура команды проекта, Совет Проекта и ключевые участники.

## Иерархия команды

Следующая диаграмма отражает иерархию команды и ее разделение на основные направления: разработка, администрация, работа с сообществом и Wiki.

```mermaid
---
config:
  class:
    hideEmptyMembersBox: true
---
classDiagram

  %% Совет %%

  class Council["Совет Проекта"]
  click Council href "/team/council"

  Council <.. HeadDeveloper
  Council <.. HeadAdministrator
  Council <.. HeadCommunityManager
  Council <.. HeadWikiEditor
  Council <.. HeadLorekeeper

  %% Разработка %%

  class HeadDeveloper["Старший Разработчик"]
  click HeadDeveloper href "/team/dev#старший-разработчик"
  class DeputyHeadDeveloper["Зам. Старшего Разработчика"]
  click DeputyHeadDeveloper href "/team/dev#заместитель-старшего-разработчика"
  class DiscordDeveloper["Discord Разработчик"]
  click DiscordDeveloper href "/team/dev#discord-разработчик"
  class Maintainer["Мейнтейнер"]
  click Maintainer href "/team/dev#мейнтейнер"
  class Coder["Программист"]
  click Coder href "/team/dev#программист"
  class Mapper["Маппер"]
  click Mapper href "/team/dev#маппер"
  class Spriter["Спрайтер"]
  click Spriter href "/team/dev#спрайтер"

  HeadDeveloper <|-- DeputyHeadDeveloper
  DeputyHeadDeveloper <.. DiscordDeveloper
  DeputyHeadDeveloper <.. Maintainer
  Maintainer <.. Coder
  Maintainer <.. Mapper
  Maintainer <.. Spriter

  %% Администрация %%

  class HeadAdministrator["Старший Администратор"]
  click HeadAdministrator href "/team/admin#старший-администратор"
  class DeputyHeadAdministrator["Зам. Старшего Администратора"]
  click DeputyHeadAdministrator href "/team/admin#заместитель-старшего-администратора"
  class Administrator["Администратор"]
  click Administrator href "/team/admin#администратор"

  HeadAdministrator <|-- DeputyHeadAdministrator
  DeputyHeadAdministrator <.. Administrator

  %% Работа с сообществом %%

  class HeadCommunityManager["Главный Менеджер Сообщества"]
  click HeadCommunityManager href "/team/community#главный-менеджер-сообщества"
  class CommunityManager["Менеджер Сообщества"]
  click CommunityManager href "/team/community#менеджер-сообщества"
  class Mentor["Ментор"]
  click Mentor href "/team/community#ментор"

  HeadCommunityManager <.. CommunityManager
  CommunityManager <.. Mentor

  %% Wiki %%

  class HeadWikiEditor["Главный Редактор Wiki"]
  click HeadWikiEditor href "/team/wiki#главный-редактор-wiki"
  class WikiEditor["Редактор Wiki"]
  click WikiEditor href "/team/wiki#редактор-wiki"

  HeadWikiEditor <.. WikiEditor

  %% Лор %%

  class HeadLorekeeper["Главный лоровед"]
  click HeadLorekeeper href "/team/lore#главный-лоровед"
  class Lorekeeper["Лоровед"]
  click Lorekeeper href "/team/lore#лоровед"

  HeadLorekeeper <.. Lorekeeper
```

## Совет Проекта

Совет проекта координирует основные направления и принимает решения, влияющие на развитие и стабильность проекта.

[Совет Проекта](/team/council)

## Направления

- [Разработчики](/team/dev)
- [Администрация](/team/admin)
- [Связь с Сообществом](/team/community)
- [Wiki](/team/wiki)
- [Лор](/team/lore)

## Текущие кандидатуры

- [Старший Разработчик](/team/dev#старший-разработчик)
  - Furior
- [Зам. Старшего Разработчика](/team/dev#заместитель-старшего-разработчика)
  - Maxiemar
- [Старший Администратор](/team/admin#старший-администратор)
  - VentelR
- [Зам. Старшего Администратора](/team/admin#заместитель-старшего-администратора)
  - Нет кандидатов
- [Главный Менеджер Сообщества](/team/community#главный-менеджер-сообщества)
  - Нет кандидатов
- [Главный Редактор Wiki](/team/wiki#главный-редактор-wiki)
  - Нет кандидатов
- [Главный лоровед](/team/lore#главный-лоровед)
  - Нет кандидатов
