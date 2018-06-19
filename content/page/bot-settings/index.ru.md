---
title: "Список доступных параметров"
date: 2018-03-14T20:00:00+02:00
draft: false

categories: []
tags: []

slug: "bot-settings"

---

Чтобы изменить значение параметра, используйте `dh!settings set <параметр> <значение>`
 
Вы можете просмотреть список изменённых параметров, написав `dh!settings modified`
 
Для установки значения параметра по умолчанию используйте `dh!settings reset <параметр>`

{{< table >}}
|Параметр|Тип значения|Значение по умолчанию|Описание|
|--- |--- |--- |--- |
|announce_level_up|boolean|True|Уведомлять/не уведомлять о повышении/понижении уровня|
|bang_lag|число с плавающей точкой|0.5|Устанавливает задержку между выстрелом и показом его последствий. Чтобы отключить, установите значение 0.|
|chance_to_kill_on_missed|целое число|5|Устанавливает вероятность попадания в кого-либо при промахе по утке в процентах.|
|clover_max_exp|целое число|10|Устанавливает максимальное количество очков опыта, которое может быть выдано за наличие клевера.|
|clover_min_exp|целое число|1|Устанавливает минимальное количество очков опыта, которое может быть выдано за наличие клевера.|
|delete_commands|boolean|False|Удалять/не удалять сообщения с командами после их выполнения.|
|disable_decoys_when_ducks_are_sleeping|boolean|True|Делать/не делать приманки безполезными, когда утки спят (см. sleeping_ducks_start и sleeping_ducks_stop)|
|duck_frighten_chance|целое число|5|Устанавливает вероятность того, что утка испугается и улетит, когда в неё стреляют в процентах.|
|ducks_per_day|целое число|48|Устанавливает количество уток, которые будут появляться в канале за день.|
|emoji_used|строка|:duck:|Устанавливает эмодзи, используемое ботом, если значение параметра emoji_ducks равно true.|
|exp_won_per_duck_killed|целое число|10|Устанавливает количество очков опыта, выдаваемое за одну убитую утку.|
|killed_mentions|boolean|True|Упоминать/не упоминать игроков, в которых кто-то попал. Может надоедать, можете его отключить.|
|language|строка|en_EN|Устанавливает язык, используемый ботом. Используйте формат 2-КОД-ЯЗЫКА-ИЗ-ДВУХ-БУКВ_КОД-СТРАНЫ-ИЗ-ДВУХ-БУКВ (fr_FR, hu_HU, en_US...). Если указанного языка не будет в базе, то будет автоматически выставлен английский.|
|mention_in_topscores|boolean|False|Упоминать/не упоминать игроков из топа. Это НЕ влияет на отправку оповещений. Может сломаться, если в топе есть игроки с длинными никами.|
|multiplier_miss_chance|число с плавающей точкой|1|Устанавливает шанс промаха. Чем больше значение данного параметра, тем больше шанс промаха.|
|pm_most_messages|boolean|False|Отправлять/не отправлять некоторые ответы посредством личных сообщений (о перезарядке, связанные с магазином и т. д.)|
|pm_stats|boolean|False|Отправлять/не отправлять ответ на команду dh!stats посредством личных сообщений|
|pm_top|boolean|False|Отправлять/не отправлять ответ на команду dh!top посредством личных сообщений|
|prefix|строка|!|Устанавливает префикс, который будет использовать бог. Если команды DuckHunt есть в других ботах, то вы можете изменить префикс. Не влияет на префикс dh!, он всегда будет работать.|
|randomize_mechanical_ducks|целое число|0|Доступны 3 значения. 0 — механические утки отличаются от обычных. 1 — некоторых уток можно отличить от обычных, некоторых нет. 2 — механические утки не отличаются от обычных.|
|show_super_ducks_life|boolean|False|Показывать/не показывать количество здоровья суперуток, пока они живы.|
|sleeping_ducks_start|целое число|0|Используется вместе с sleeping_ducks_stop для установки периода времени (в 24-часовом формате), во время которого утки не будут появляться. Параметр ducks_per_day НЕ перестаёт иметь силу.|
|sleeping_ducks_stop|целое число|0|См. параметр sleeping_ducks_start.|
|ducks_chance|целое число|100|Устанавливает вероятность того, что появившаяся утка будет обычной.|
|super_ducks_chance|integer|5|Probability that a duck that spawns will be a super duck|
|baby_ducks_chance|integer|2|Probability that a duck that spawns will be a baby duck|
|mother_of_all_ducks_chance|integer|1|Probability that a duck that spawns will be a mother of all ducks|
|super_ducks_exp_multiplier|float|1.1|To get experience earned when a hunter kill a superduck, we use the formula rounded_integer(exp_won_per_duck_killed * super_ducks_exp_multiplier * duck_life)|
|super_ducks_maxlife|integer|7|Maximum life of a super duck|
|super_ducks_minlife|integer|3|Minimum life of a super duck|
|tax_on_user_give|integer|5|Percentage of exp that will be taken as a tax when a player uses the send_exp command. This can be disabled by setting it to 0.|
|time_before_ducks_leave|integer|660|Time in seconds before a duck leaves of boredom if he isn't killed.|
|tts_ducks|bool|False|Try to speak when ducks appear. Experimental setting.|
|user_can_give_exp|bool|True|Allow users to send each other experience points with the send_exp command.|
|users_can_find_objects|bool|True|Allow users to find objects in bushes. Some objects are trash, some objects will benefit the hunter.|
{{< /table >}}
