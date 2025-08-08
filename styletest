<script>
(function () {
  'use strict';

  // --- НАСТРОЙКИ ТЕСТА ---
  const testConfig = {
    title: "Ваш стилевой вектор",
    numberOfQuestions: 7,
    categories: {
      a: { title: "Поэтичный стиль", description: `<p><strong>Поэтичный стиль</strong></p><p>Вы — мечтательница, ищущая красоту в деталях. Ваша душа откликается на сказки, выразительные формы и цвета. Вы не просто носите одежду, вы проживаете в ней эмоции. Вам важны легкость, романтика, прикосновение к чуду. Стиль — это ваша история, рассказанная цветом, шелестом ткани и изгибом силуэта.</p><p><strong>Детали:</strong> акварельные оттенки, ягодные оттенки, воздушные платья, воланы, легкие ткани, немного винтажной магии, немного театральности.</p><p><strong>Цвета:</strong></p><p>Пастельные, приглушённые, акварельные, ягодные, винтажные. Лавандовый, дымчато-розовый, небесный, молочный, светлый серо-бежевый, клубничный, черничный, малиновый, горчичный, цвет корицы, цвет морской волны, одуванчиковый, васильковый.</p><p><strong>Материалы:</strong></p><p>Шифон, органза, батист, кружево, шитье, лёгкий хлопок, тонкая шерсть с мохером, бархат.</p><p><strong>Ключевые образы для вдохновения:</strong></p><ul><li>Героиня осеннего фильма в твидовой юбке и вязаной жилетке с контрастной окантовкой</li><li>Студентка на выставке в розовой блузе с воланами и пальто цвета хаки с вышивкой на спине</li><li>Девушка в прозрачной блузе с бантом и длинной юбке в приглушенных тонах</li><li>Художница с легким шарфом и блокнотом для зарисовок</li><li>Героиня французского артхауса в пальто из альпаки и беретке</li><li>Читательница стихов на подоконнике в платье с оборками</li><li>Танцующая на рассвете девушка в платье-комбинации и с распущенными волосами</li></ul><p><strong>Героини кино:</strong></p><p>Ваш образ раскрывается через мечты, атмосферу, деликатность.</p><p><strong>Герои:</strong></p><ul><li>Алиса «Алиса в стране чудес»</li><li>Сьюзи «Королевство полной луны»</li><li>Эмили «Эмили в Париже»</li><li>Белль «Красавица и чудовище»</li><li>Амели Пулен «Амели»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Платья с завышенной талией</li><li>Рукава-фонарики</li><li>Юбки миди с мягкой драпировкой</li><li>Цветочные и ритмические принты</li><li>Винтажные блузки</li><li>Пальто-кокон</li><li>Обувь с ремешками (мери-джейн)</li><li>Сумка с фигурной пряжкой</li></ul><p><strong>Ваша формула:</strong> «Мягкость + Чудо + Внутреннее я»</p>` },
      b: { title: "Интеллектуальный стиль", description: `<p><strong>Интеллектуальный стиль</strong></p><p>Вы выражаете себя через идеи, вам важно показать, что внутреннее важнее внешнего. В вас сочетается наблюдательность, глубина и тонкий вкус к деталям. Вам важна форма, история и внутренний смысл. Одежда — это часть вашего языка. Вещи должны быть со структурой, с индивидуальностью, с подтекстом.</p><p><strong>Детали:</strong> костюмы с изюминкой, винтаж, редкие украшения, художественные цитаты в образе, фактурные ткани, приглушенные и сложные цвета</p><p><strong>Цвета:</strong></p><p>Глубокие и сложные. Серо-синий, бордовый, охра, бутылочный, графитовый, сине-зелёный, кирпичный, глубокий синий, горчичный, болотный, шоколад.</p><p><strong>Материалы:</strong></p><p>Твид, шерсть, мягкий деним, кашемир, шёлк с матовым блеском, вельвет, вискоза.</p><p><strong>Ключевые образы:</strong></p><ul><li>Французская писательница в пальто мужского кроя и очках</li><li>Героиня артхаусного кино в сером кашемировом свитере</li><li>Лектор в университете в рубашке с отложным воротником и винтажной броши</li><li>Архитектор в минималистичном платье с кожаной сумкой, презентующая свой проект</li><li>Куратор музея в льняном костюме и мягких слипонах</li><li>Героиня романа в хлопковой рубашке и брюках с защипами</li><li>Девушка, читающая книгу в кафе в длинном пальто и мужских ботинках</li><li>Преподавательница философии в твидовом пиджаке и винтажных часах</li></ul><p><strong>Героини кино</strong></p><p>Ваш образ раскрывается через идеи, глубину и наблюдение.</p><p><strong>Герои:</strong></p><ul><li>Бет Хармон «Ход королевы»</li><li>Элизабет Беннет «Гордость и предубеждение» 2005</li><li>Джо Марч «Маленькие женщины» 2020</li><li>Мерфи Купер «Интерстеллар»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Блузы с необычными воротниками, крупными, асимметричными, аскот</li><li>Структурные жакеты</li><li>Брюки со стрелками</li><li>Юбки-миди с архитектурным кроем</li><li>Очки в тяжёлой оправе</li><li>Лоферы, оксфорды</li><li>Структурные сумки</li><li>Акцентные пуговицы с гербами</li><li>Элементы мужского гардероба</li></ul><p><strong>Ваша формула:</strong> «Смысл + Форма + Уникальность»</p>` },
      c: { title: "Драматичный стиль", description: `<p><strong>Драматичный стиль</strong></p><p>Вы — магнетичная, выразительная, не боитесь быть в центре внимания. Ваша энергия не мягкая, а будоражущая. Ваш стиль — не защита, а заявление. Вы можете быть резкой, можете быть пленительной, но никогда — пустой или незаметной. Для вас важно, чтобы одежда выражала характер и эмоцию, ваш стиль никогда не будет сдержанным и правильным, он будет заставлять других оборачиваться вам в след.</p><p><strong>Детали:</strong> Выразительный силуэт, контраст цвета или фактуры, неожиданный акцентный элемент (украшение, вырез, асимметрия, принт), яркая помада</p><p><strong>Цвета:</strong></p><p>Контрастные, выразительные. Чёрный, белый, красный, изумрудный, сапфировый, фуксия.</p><p><strong>Материалы:</strong></p><p>Гладкий атлас, кожа, глянец, лак, структурированный плотный трикотаж, костюмная ткань с блеском.</p><p><strong>Ключевые образы:</strong></p><ul><li>Героиня нуара в длинном пальто и красной помаде</li><li>Современная ведьма в черном асимметричном платье и кольцах с камнями</li><li>Рок-дива в коже и шелке</li><li>Модная редакторка в объемном жакете с острыми плечами</li><li>Арт-муза в струящейся ткани с ярким макияжем и драматичным взглядом</li><li>Актриса новой волны в платье с провокационным вырезом</li></ul><p><strong>Героини кино</strong></p><p>Ваш образ раскрывается через силу, контраст, эффект.</p><p><strong>Герои:</strong></p><ul><li>Миранда Пристли «Дьявол носит Prada»</li><li>Кэрол «Кэрол»</li><li>Рита Скитер «Гарри Поттер»</li><li>Одри «Твин Пикс»</li><li>Джиллиан Оуэнс «Практическая магия»</li><li>Вилланель «Убивая Еве»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Монолук в одном цвете: черный или наоборот яркий</li><li>Пальто в пол с акцентной линией плеч</li><li>Силуэт с выраженной талией и барочной линией бедер</li><li>Чёрные солнцезащитные очки</li><li>Туфли с острым носом</li><li>Минимализим и архитектура в образе</li><li>Сложные необычные украшения</li><li>Большое количество аксессуаров</li><li>Крупный масштаб</li><li>Декольте или наоборот полностью закрытый силуэт</li><li>Подчеркнутая фигура или наоборот выраженный оверсайз</li></ul><p><strong>Ваша формула:</strong> «Выразительность + Архитектура + Сила»</p>` },
      d: { title: "Натуральный стиль", description: `<p><strong>Натуральный стиль</strong></p><p>Вам близка простота, честность, заземленность. Одежда для вас – это не способ производить впечатление, а способ быть собой, свобода, комфорт, ощущение спокойствия. Вы как глоток воздуха, как «возвращение домой».</p><p><strong>Детали:</strong> льняные рубашки, оверсайз, натуральные ткани, природная палитра, свободные платья, немного народных мотивов, природные материалы в аксессуарах.</p><p><strong>Цвета:</strong></p><p>Натуральная палитра. Песочный, хаки, глина, беж, охра, оливковый, выцветший деним.</p><p><strong>Материалы:</strong></p><p>Лён, хлопок, плотный трикотаж, грубая шерсть, замша, деним без стрейча, необработанные края.</p><p><strong>Ключевые образы:</strong></p><ul><li>Девушка в вязаном свитере, джинсах и замшевых ботинках</li><li>Хозяйка сада в платье из хлопка с фартуком</li><li>Муза деревенского дома в платье-рубашке и мягком кардигане</li><li>Девушка, которая варит кофе на открытой веранде</li><li>Актриса на пикнике в легком платье с шитьем</li><li>Мечтательница в поле в джинсах и футболке с рисунком</li><li>Молодая мама в джинсовом комбинезоне и больших серёжках</li><li>Путешественница в вельветовых брюках и вязанном шарфе на привале, наблюдающая за природой</li><li>Пекарь в льняном платье, фартуке и с запахом корицы</li><li>Героиня slow life с чашкой травяного чая в руках</li></ul><p><strong>Героини кино</strong></p><p>Ваш образ раскрывается через про свободу, природу, честность.</p><p><strong>Герои:</strong></p><ul><li>Грейс Стампер «Армагеддон»</li><li>Ребекка Пирсон «Это мы»</li><li>Френни «Однажды в Нью-Йорке»</li><li>Элис Флетчер «Годлесс»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Оверсайз рубашки</li><li>Свободные платья из льна</li><li>Джинсовые куртки</li><li>Мешковатые брюки</li><li>Плетёные аксессуары</li><li>Простая обувь без каблука</li><li>Резиновые сапоги и высокие носки</li><li>Украшения из натуральных материалов</li><li>Мягкие кардиганы</li><li>Вязанные летние платья</li><li>Платья из хлопка природных оттенков или в мелкий цветочек</li></ul><p><strong>Ваша формула:</strong> «Открытость + Природа + Спокойствие»</p>` },
      e: { title: "Романтичный стиль", description: `<p><strong>Романтичный стиль</strong></p><p>Вы — нежность и тепло. Вам важно чувствовать себя красивой, ухоженной, эстетичной. Вы умеете украшать повседневность и ценить мягкость, уют. Вы выражаете любовь к себе через красоту.</p><p><strong>Детали:</strong> женственные платья, мягкие текстуры, благородные пастельные оттенки, аксессуары с сердцами и цветами.</p><p><strong>Ключевые образы:</strong></p><ul><li>Девушка в платье с цветочным принтом и распущенными локонами</li><li>Героиня кино в лёгком пальто, летящем платье и балетках</li><li>Девушка с идеальной укладкой и «Vogue» в сумке</li><li>Красавица в кофейне с видом на Эйфелеву башню, завтракающая круассаном и кофе</li><li>Девушка в шелковом платке и кремовом тренче</li><li>Греческая богиня на балконе в белом платье и золотых серёжках</li><li>Современная принцесса</li></ul><p><strong>Героини кино</strong></p><p>Ваш образ раскрывается через красоту, ухоженность, нежность.</p><p><strong>Герои:</strong></p><ul><li>Шарлотта «Секс в большом городе»</li><li>Холли Голайтли «Завтрак у Тиффани»</li><li>Джейн Беннет «Гордость и предубеждение», 2005</li><li>Жизель «Зачарованная»</li></ul><p><strong>Цвета:</strong></p><p>Нежные, тёплые, женственные. Розовый, персиковый, кремовый, карамель, пудровый, молочный шоколад, нежно-голубой, светло-зеленый.</p><p><strong>Материалы:</strong></p><p>Шёлк, вискоза, кружево, мягкий трикотаж, ангоровая шерсть, тонкий кашемир, все дышащее и полупрозрачное.</p><p><strong>Примеры одежды:</strong></p><ul><li>Струящиеся платья</li><li>Юбки с цветочными принтами</li><li>Складки и воланы</li><li>Юбки солнце</li><li>Блузы с рюшами</li><li>Банты на груди и поясе</li><li>Мягкие кардиганы</li><li>Балетки</li><li>Сумки с округлыми формами</li><li>Броши на воротнике</li><li>Жемчуг</li></ul><p><strong>Ваша формула:</strong> «Нежность + Уход + Утончённость»</p>` },
      f: { title: "Бунтарский стиль", description: `<p><strong>Бунтарский стиль</strong></p><p>Ваш стиль – это не «вписаться», а «сказать по-своему». Это способ транслировать свободу, эмоцию, свое мнение и даже протест. В образах вы цените неожиданность, индивидуальность. Для вас стиль — это не просто одежда, а визуальное высказывание, творческий акт, внутренняя свобода. Вы не боитесь странного, вы им гордитесь.</p><p>Бунтарский стиль – это эстетика уличного искусства, независимых кинофестивалей, лоу-фай музыки и образов, созданных по наитию, а не по инструкции. В нем нет агрессии, но есть вызов.</p><p>Вы можете смешивать несовместимое, сочетать винтаж и спорт, кожу и кружево, графику и хаос.</p><p>Вы любите вещи с историей, с характером, которые отражают вас.</p><p>Ваши образы могут казаться небрежными, но именно в этом и есть их энергия и творческий дух.</p><p><strong>Детали:</strong> принты, нестандартные силуэты, мрачные/яркие акценты, смесь эпох и жанров, блестки, необычный макияж, грубые ботинки, панк, гранж, глэм-рок.</p><p><strong>Цвета:</strong></p><p>Глубокие, насыщенные, неоновые, сложные. Чёрный, индиго, фуксия, ултрафиолет, металлик, ярко-желтый, ярко-розовый, графит, желто-зеленый.</p><p><strong>Материалы:</strong></p><p>Кожа, деним, сетка, металлизированные ткани, плащёвка, глянец рваные ткани (джинс, трикотаж со спущенными петлями).</p><p><strong>Ключевые образы:</strong></p><ul><li>Девушка в кожаной куртке и ботинках на шнуровке</li><li>Современная муза с пирсингом, шапкой-бини и графичным мейкапом</li><li>Арт-героиня в асимметричном крое и чёрных очках</li><li>Девушка на мотоцикле в потертых джинсах и топе-сетке</li><li>Художница в окрашенном вручную пальто</li><li>Девушка в кожаном пиджаке, майке и черном чокере</li><li>Муза андеграунда в  оверайз жакете и футболке с портретом любимого режиссёра</li><li>Рокерша в платье-сорочке и ботинках на огромной платформе</li><li>Девушка, превращающая бабушкин свитер в арт-объект</li></ul><p><strong>Героини кино</strong></p><p>Ваш образ раскрывается через вызов, эксперимент, острое самовыражение.</p><p><strong>Герои:</strong></p><ul><li>Джулс Вон «Euphoria»</li><li>Лисбет Саландер «Девушка с татуировкой дракона»</li><li>Харли Квинн «Отряд самоубийц»</li><li>Фиби «Флибаг»</li><li>Драса «Ущелье»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Кожаные куртки</li><li>Рваные джинсы</li><li>Неоновые вставки</li><li>Маскулинные жакеты</li><li>Свитера со спущенными петлями</li><li>Корсеты</li><li>Грубые ботинки</li><li>Графические принты, надписи</li><li>Цепи</li><li>Пирсинг (на одежде и аксессуарах он тоже может быть)</li><li>Прозрачные синтетические ткани</li><li>Кастомизированные вещи</li><li>Деконструктивизм, апсайклинг</li></ul><p><strong>Ваша формула:</strong> «творчество + искренность + ирония»</p>` },
      g: { title: "Динамический стиль", description: `<p><strong>Динамический стиль</strong></p><p>Вы живёте телом. Вы ощущаете себя через движение, активность, ясность. Вам важно, чтобы одежда работала с вами, а не против. Вы цените комфорт, функциональность и свежесть. Стиль — это часть вашего ритма жизни. Вам важно быть в моменте, быть живой, быть настоящей.</p><p><strong>Детали:</strong> лаконичные формы, спортивные элементы, дышащие ткани, светлые и яркие цвета, минимализм, яркие вставки, подчеркнутая фигура.</p><p><strong>Цвета:</strong></p><p>Свежие, чистые, спортивные. Белый, светло-серый, лайм, бирюзовый, неоновый акцент на фоне нейтрального.</p><p><strong>Материалы:</strong></p><p>Трикотаж, спандекс, спортивный нейлон, микрофибра, гладкий хлопок, мембранные ткани, тех-материалы.</p><p><strong>Ключевые образы:</strong></p><ul><li>Девушка в спортивных леггинсах, кроссовках и яркой куртке</li><li>Скейтбордистка в шортах-карго и майке с открытой спиной</li><li>Героиня кино в капюшоне, с рюкзаком и наушниками</li><li>Любительница хайкинга в ветровке и удобных брюках</li><li>Тренерка в спортивной форме с элементами стритстайла</li><li>Девушка после пилатеса в монохромном костюме</li><li>ЗОЖ-энтузиастка в бейсболке, с бутылкой воды и поясной сумкой</li><li>Девушка в уютном флисовом костюме</li></ul><p><strong>Героини кино</strong></p><p>Вы — про энергию, свежесть, телесность.</p><p><strong>Герои:</strong></p><ul><li>Лара Крофт «Tomb Raider»</li><li>Джулетта Николс «Укрытие»</li><li>Шерил Стрейд «Дикая»</li><li>Аня Смолина «Поехавшая»</li></ul><p><strong>Примеры одежды:</strong></p><ul><li>Спортивные костюмы из футера</li><li>Облегающие монохромные костюмы</li><li>Кроссовки</li><li>Комбинезоны с карманами</li><li>Облегающие комбинезоны</li><li>Топы и спортивные бра</li><li>Ветровки, жилеты с сеткой</li><li>Бейсболки</li></ul><p><strong>Ваша формула:</strong> «Свежесть + Здоровье + Движение»</p>` }
    },
    resultImages: {
      a: "https://static.tildacdn.com/tild6334-3837-4938-a435-616264306535/photo.jpg",
      b: "https://static.tildacdn.com/tild6433-3136-4435-a533-663939376562/photo.jpg",
      c: "https://static.tildacdn.com/tild6332-6435-4539-b362-326431626335/photo.jpg",
      d: "https://static.tildacdn.com/tild6532-6435-4630-a533-373932336232/photo.jpg",
      e: "https://static.tildacdn.com/tild3833-6633-4133-b032-353865613964/photo.jpg",
      f: "https://static.tildacdn.com/tild6236-3863-4638-a362-633563386537/photo.jpg",
      g: "https://static.tildacdn.com/tild6533-3937-4065-b430-646563363536/photo.jpg"
    },
    questions: [
      { text: "Какой интерьер вам ближе всего?", options: [
        { text: "Воздушный, с кружевом, цветами, пастель", category: "a" },
        { text: "Минималистичный, с книгами и винтажом", category: "b" },
        { text: "Чёрно-белый, с акцентами, глянец и металл", category: "c" },
        { text: "Скандинавский, природные материалы, дерево", category: "d" },
        { text: "Мягкий, уютный, как кукольный домик", category: "e" },
        { text: "Неоновый, тёмный, постеры, арт", category: "f" },
        { text: "Светлый, свежий, много воздуха, натуральные ткани, минимум декора", category: "g" }
      ]},
      { text: "Какой фильм вызывает у вас эстетическое восхищение?", options: [
        { text: "«Амели», «Отель \"Гранд Будапешт\"»", category: "a" },
        { text: "«Авиатор», «Игры разума»", category: "b" },
        { text: "«Под покровом ночи», «Черный лебедь»", category: "c" },
        { text: "«Маленькая мисс Счастье», «Мой парень - псих»", category: "d" },
        { text: "«Гордость и предубеждение», «Сладкий ноябрь»", category: "e" },
        { text: "«Вечное сияние чистого разума», «Скотт Пилигрим»", category: "f" },
        { text: "«Дикая», «Аватар», «Под солнцем Тосканы»", category: "g" }
      ]},
      { text: "Какие ткани вам особенно нравятся?", options: [
        { text: "Шифон, органза, тонкий батист", category: "a" },
        { text: "Лён, шерсть, фактурный хлопок", category: "b" },
        { text: "Кожа, сатин, деним", category: "c" },
        { text: "Хлопок, флис, твид", category: "d" },
        { text: "Атлас, трикотаж, тонкая шерсть", category: "e" },
        { text: "Сетка, нейлон, бархат, блестки", category: "f" },
        { text: "Джерси, лайкра, дышащие и эластичные материалы", category: "g" }
      ]},
      { text: "Что вас вдохновляет из детства?", options: [
        { text: "Сказки, книжки с картинками", category: "a" },
        { text: "Коллекции, запах книг, музеи", category: "b" },
        { text: "Танцы, сцена, шоу, конкурсы", category: "c" },
        { text: "Игры в лесу, походы, семья", category: "d" },
        { text: "Наряды принцесс, рисование, куклы", category: "e" },
        { text: "Субкультуры, музыка, эмо-период, странные аксессуары", category: "f" },
        { text: "Двор с друзьями, подвижные игры, спортивные кружки", category: "g" }
      ]},
      { text: "В какой одежде вы чувствуете себя собой?", options: [
        { text: "Яркое платье, туфли мэри джейн и сумка с принтом", category: "a" },
        { text: "Винтажная рубашка, прямые брюки, лоферы", category: "b" },
        { text: "Чёрный total look, деконструктивизм в кроем", category: "c" },
        { text: "Свитер oversize, джинсы, кеды", category: "d" },
        { text: "Легкое платье, мягкий кардиган", category: "e" },
        { text: "Свитер со спущенными петлями, грубые ботинки, яркие аксессуары", category: "f" },
        { text: "Лаконичный крой, спортивный силуэт, кроссовки, лосины", category: "g" }
      ]},
      { text: "Какой подарок вам приятнее всего получить?", options: [
        { text: "Альбом с репродукциями любимого художника или волшебная брошь", category: "a" },
        { text: "Научно-популярная книга или коллекция фоторабот", category: "b" },
        { text: "Поход в караоке или фотосессия", category: "c" },
        { text: "Плед, аромасвечи, корзина с мёдом", category: "d" },
        { text: "Блокнот с милым рисунком или браслет из камней по дате рождения", category: "e" },
        { text: "Арт-постер или дикое безумное украшение", category: "f" },
        { text: "Спортивный аксессуар, абонемент на танцы/йогу, массаж или трекер активности", category: "g" }
      ]},
      { text: "Какие цвета вам сейчас ближе?", options: [
        { text: "Бирюзовый, пыльная роза, коралловый", category: "a" },
        { text: "Горчичный, бордо, серый", category: "b" },
        { text: "Чёрный, белый, вишнёвый", category: "c" },
        { text: "Песочный, оливковый, кремовый", category: "d" },
        { text: "Персиковый, лавандовый", category: "e" },
        { text: "Неон, ярко-фиолетовый, серо-зелёный", category: "f" },
        { text: "Лаймовый, оранжевый, светло-серый, белый, небесно-голубой", category: "g" }
      ]}
    ]
  };
  // --- КОНЕЦ НАСТРОЕК ---

  function initConstructorTest() {
    const container = document.getElementById('constructor-test-container');
    if (!container) return;
    if (container.dataset.inited === '1' || container.shadowRoot) return; // защита от повторной инициализации
    container.dataset.inited = '1';

    const shadow = container.attachShadow({ mode: 'open' });

    // --- Генерация HTML ---
    let questionsHTML = '';
    for (let i = 0; i < testConfig.numberOfQuestions; i++) {
      const q = testConfig.questions[i];
      let optionsHTML = '';
      for (let j = 0; j < q.options.length; j++) {
        optionsHTML += `
          <li class="answer-option"><label><input type="radio" name="q${i+1}" value="${q.options[j].category}"> ${q.options[j].text}</label></li>
        `;
      }
      let navButtons = '';
      if (i === 0) {
        navButtons = `<button id="next-btn-1" class="material-button next-full-width">Далее</button>`;
      } else if (i === testConfig.numberOfQuestions - 1) {
        navButtons = `<div class="nav-buttons-wrapper"><button class="prev-btn material-button arrow-button" data-question="${i+1}">Назад</button><button id="show-result-btn" class="material-button next-full-width">Показать результат</button></div>`;
      } else {
        navButtons = `<div class="nav-buttons-wrapper"><button class="prev-btn material-button arrow-button" data-question="${i+1}">Назад</button><button class="next-btn material-button next-full-width" data-question="${i+1}">Далее</button></div>`;
      }
      questionsHTML += `
        <div class="question-container ${i===0 ? 'active' : ''}" id="q${i+1}">
          <div class="question-number">Вопрос ${i+1}</div>
          <div class="question-text">${q.text}</div>
          <ul class="answer-options">
            ${optionsHTML}
          </ul>
          <div class="navigation">
            ${navButtons}
          </div>
        </div>
      `;
    }

    const testHTML = `
      <div class="test-container">
        <h1>${testConfig.title}</h1>
        <div class="progress-text">Вопрос <span id="current-question">1</span> из ${testConfig.numberOfQuestions}</div>
        <div class="progress-bar-container"><div class="progress-bar" id="progress-bar"></div></div>
        ${questionsHTML}
        <div class="result-container" id="result-container">
          <h2 class="result-title" id="result-title">Ваш результат</h2>
          <img src="" alt="Результат" class="result-image" id="result-image">
          <div class="result-description" id="result-description"></div>
          <div class="buttons-container">
            <button id="save-result-btn" class="material-button">Сохранить результат</button>
            <button id="restart-btn" class="material-button">Пройти повторно</button>
          </div>
        </div>
      </div>
    `;

    // --- CSS ---
    const testCSS = `
      :host { display: block; width: 100%; }
      * { box-sizing: border-box; }
      body { font-family: 'Roboto','Helvetica Neue',Arial,sans-serif; line-height: 1.6; color: #212121; background-color: #f5f5f5; margin: 0; padding: 10px; box-sizing: border-box; }
      .test-container { font-family: 'Roboto','Helvetica Neue',Arial,sans-serif; max-width: 1000px; margin: 0 auto; background-color: #fff; border-radius: 50px; box-shadow: 0 2px 4px rgba(0,0,0,0.1), 0 4px 8px rgba(0,0,0,0.05); padding: 25px; position: relative; overflow: hidden; transition: box-shadow 0.3s ease; }
      .test-container:hover { box-shadow: 0 4px 8px rgba(0,0,0,0.15), 0 8px 16px rgba(0,0,0,0.1); }
      .test-container::before { content: ""; position: absolute; top: 0; left: 0; right: 0; height: 6px; background: linear-gradient(90deg,#fc6767,#ff9b9b); border-radius: 50px 50px 0 0; }
      h1 { text-align: center; color:#212121; margin-bottom:25px; font-weight:500; }
      .question-container { display:none; border-radius:50px; padding:20px; background-color:#fafafa; margin-bottom:20px; }
      .question-container.active { display:block; animation: fadeIn 0.5s ease-out; }
      @keyframes fadeIn { from {opacity:0; transform: translateY(10px);} to {opacity:1; transform: translateY(0);} }
      .question-number { font-weight:500; color:#616161; margin-bottom:12px; font-size:0.95em; }
      .question-text { font-size:1.15em; margin-bottom:25px; font-weight:400; color:#424242; }
      .answer-options { list-style:none; max-width:600px; margin-inline:auto; margin-top:0; margin-bottom:25px; padding:0; border-radius:50px; background:#fff; box-shadow:0 1px 2px rgba(0,0,0,0.05); padding-left:10px; padding-right:10px; width:100%; box-sizing:border-box; }
      .answer-option { margin-bottom:12px; }
      .answer-option label { display:flex; align-items:center; min-height:56px; cursor:pointer; padding:12px 20px; border:1px solid #e0e0e0; border-radius:50px; transition: all .2s ease, box-shadow .2s ease, transform .1s ease; font-size:1em; background:#fff; position:relative; overflow:hidden; word-break:break-word; }
      .answer-option label:hover { background:#f5f5f5; border-color:#bdbdbd; box-shadow:0 1px 3px rgba(0,0,0,0.1); transform: translateY(-1px); }
      .answer-option label:active { transform: translateY(0); box-shadow:0 1px 2px rgba(0,0,0,0.1); }
      .answer-option input[type="radio"] { margin-top:0; margin-right:16px; flex-shrink:0; cursor:pointer; width:18px; height:18px; accent-color:#fc6767; }
      .answer-option input[type="radio"]:focus + label, .answer-option label:focus-within { outline:2px solid #fc6767; outline-offset:2px; border-color:#fc6767; }
      .navigation { display:flex; justify-content:space-between; margin-top:25px; flex-wrap:wrap; gap:12px; box-sizing:border-box; align-items:center; }
      .nav-buttons-wrapper { display:flex; width:100%; align-items:center; gap:12px; }
      .material-button { padding:0; border:none; border-radius:50px; cursor:pointer; font-size:1em; font-weight:500; transition: background-color .3s ease, box-shadow .3s ease, transform .1s ease; text-transform:none; letter-spacing:.05em; box-shadow:0 1px 3px rgba(0,0,0,0.1); position:relative; overflow:hidden; outline:none; display:flex; justify-content:center; align-items:center; width:150px; height:56px; min-width:150px; min-height:56px; }
      .material-button:hover { box-shadow:0 2px 6px rgba(0,0,0,0.15); transform: translateY(-1px); }
      .material-button:active { transform: translateY(0); box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24); }
      .material-button:focus { outline:2px solid #fc6767; outline-offset:2px; }
      .next-full-width, #show-result-btn, #save-result-btn { background-color:#fc6767; color:#fff; flex:1; min-width:150px; min-height:56px; margin:0; }
      .next-full-width:hover, #show-result-btn:hover, #save-result-btn:hover { background-color:#fb4f4f; }
      .next-full-width:active, #show-result-btn:active, #save-result-btn:active { background-color:#e55c5c; }
      #restart-btn, .prev-btn { background:#f5f5f5; color:#424242; border:1px solid #e0e0e0; width:150px; height:56px; min-width:150px; min-height:56px; padding:0; flex:0 0 auto; }
      #restart-btn:hover, .prev-btn:hover { background:#eee; border-color:#bdbdbd; }
      #restart-btn:active, .prev-btn:active { background:#e0e0e0; }
      .arrow-button { font-size:1em; font-weight:500; width:150px; height:56px; min-width:150px; min-height:56px; }
      .result-container { display:none; text-align:center; animation: fadeIn .8s ease-out; border-radius:50px; padding:30px; background:#fff; box-shadow:0 2px 4px rgba(0,0,0,0.05); margin-top:20px; }
      .result-image { width:100%; height:auto; border-radius:25px; margin:25px auto; box-shadow:0 2px 4px rgba(0,0,0,0.1), 0 4px 8px rgba(0,0,0,0.05); }
      .result-title { font-size:1.7em; margin-bottom:20px; color:#212121; font-weight:500; }
      .result-description { text-align:left; max-width:700px; margin:25px auto; padding:20px; background:#fafafa; border-radius:50px; box-shadow:0 1px 3px rgba(0,0,0,0.05); font-size:1em; line-height:1.7; }
      .result-description li { margin-bottom:.6em; }
      .progress-bar-container { width:100%; background:#eee; border-radius:50px; margin-bottom:25px; overflow:hidden; height:12px; box-shadow: inset 0 1px 2px rgba(0,0,0,0.05); }
      .progress-bar { height:100%; background: linear-gradient(90deg,#fc6767,#ff9b9b); width:0%; transition: width .5s cubic-bezier(.4,0,.2,1); border-radius:50px; }
      .progress-text { text-align:right; font-size:.95em; color:#616161; margin-bottom:8px; font-weight:400; }
      .buttons-container { display:flex; justify-content:space-between; align-items:center; margin-top:20px; gap:20px; }
      #save-result-btn, #restart-btn { display:inline-block; width:200px; height:56px; margin:10px 10px 0 0; text-align:center; font-size:1em; font-weight:500; letter-spacing:.05em; border-radius:50px; transition: background-color .3s ease, box-shadow .3s ease, transform .1s ease; }
      @media (max-width:768px) {
        .test-container { padding:20px; border-radius:50px; }
        h1 { font-size:1.5em; margin-bottom:20px; }
        .question-number { font-size:.9em; margin-bottom:10px; }
        .question-text { font-size:1.1em; margin-bottom:20px; }
        .answer-options { margin-bottom:20px; border-radius:50px; }
        .answer-option { margin-bottom:10px; }
        .answer-option label { min-height:50px; padding:10px 15px; font-size:.95em; border-radius:50px; }
        .answer-option input[type="radio"] { width:16px; height:16px; margin-right:12px; }
        .navigation { margin-top:20px; gap:10px; }
        .nav-buttons-wrapper { gap:10px; }
        .material-button { width:150px; height:56px; min-width:150px; min-height:56px; font-size:.95em; border-radius:50px; }
        .next-full-width, #show-result-btn, #save-result-btn { min-width:150px; min-height:56px; }
        #restart-btn, .prev-btn { width:150px; height:56px; min-width:150px; min-height:56px; }
        .arrow-button { font-size:1em; width:150px; height:56px; min-width:150px; min-height:56px; }
        .result-title { font-size:1.5em; margin-bottom:15px; }
        .result-description { padding:15px; font-size:.95em; border-radius:50px; margin:20px auto; }
        .progress-bar-container { height:10px; border-radius:50px; margin-bottom:20px; }
        .progress-bar { border-radius:50px; }
        .progress-text { font-size:.9em; margin-bottom:6px; }
        .buttons-container { flex-direction:column; align-items:center; gap:15px; }
        #save-result-btn, #restart-btn { width:100%; max-width:250px; }
      }
      @media (max-width:480px) {
        .test-container { padding:15px; border-radius:50px; }
        h1 { font-size:1.3em; }
        .question-text { font-size:1em; }
        .answer-option label { min-height:45px; padding:8px 12px; font-size:.9em; border-radius:50px; }
        .answer-option input[type="radio"] { width:14px; height:14px; margin-right:10px; }
        .material-button { width:150px; height:56px; min-width:150px; min-height:56px; font-size:.9em; border-radius:50px; }
        #restart-btn, .prev-btn { width:150px; height:56px; min-width:150px; min-height:56px; }
        .arrow-button { font-size:1em; width:150px; height:56px; min-width:150px; min-height:56px; }
        .result-title { font-size:1.3em; }
        .result-description { padding:12px; font-size:.9em; border-radius:50px; }
        .progress-text { font-size:.85em; }
        .buttons-container { gap:12px; }
        #save-result-btn, #restart-btn { width:100%; max-width:220px; margin:0; }
      }
    `;

    const style = document.createElement('style');
    style.textContent = testCSS;
    const wrapper = document.createElement('div');
    wrapper.innerHTML = testHTML;
    shadow.appendChild(style);
    shadow.appendChild(wrapper);

    // --- ЛОГИКА ТЕСТА ---
    let currentQuestionIndex = 0;
    const totalQuestions = testConfig.numberOfQuestions;
    const scores = {};
    for (const cat in testConfig.categories) scores[cat] = 0;
    let finalResultCategory = null;

    function findEl(selector) { return shadow.querySelector(selector); }

    function updateProgressBar() {
      const progressPercent = ((currentQuestionIndex + 1) / totalQuestions) * 100;
      findEl('#progress-bar').style.width = `${progressPercent}%`;
      findEl('#current-question').textContent = currentQuestionIndex + 1;
    }

    function nextQuestion(questionNumber) {
      const selectedOption = findEl(`input[name="q${questionNumber}"]:checked`);
      if (!selectedOption) { alert("Пожалуйста, выберите один из вариантов ответа."); return; }
      const category = selectedOption.value;
      scores[category]++;
      if (questionNumber < totalQuestions) {
        findEl(`#q${questionNumber}`).classList.remove('active');
        currentQuestionIndex++;
        if (currentQuestionIndex < totalQuestions) {
          findEl(`#q${questionNumber + 1}`).classList.add('active');
          updateProgressBar();
        }
      }
    }

    function prevQuestion(questionNumber) {
      if (questionNumber > 1) {
        const prevQuestionNum = questionNumber - 1;
        const prevSelectedOption = findEl(`input[name="q${prevQuestionNum}"]:checked`);
        if (prevSelectedOption) {
          const prevCategory = prevSelectedOption.value;
          scores[prevCategory]--;
        }
        findEl(`#q${questionNumber}`).classList.remove('active');
        currentQuestionIndex--;
        findEl(`#q${questionNumber - 1}`).classList.add('active');
        updateProgressBar();
      }
    }

    function showResult() {
      const selectedOption = findEl(`input[name="q${totalQuestions}"]:checked`);
      if (!selectedOption) { alert("Пожалуйста, выберите один из вариантов ответа."); return; }
      const category = selectedOption.value;
      scores[category]++;

      let maxScore = -1;
      let winningCategories = [];
      for (const cat in scores) {
        if (scores[cat] > maxScore) { maxScore = scores[cat]; winningCategories = [cat]; }
        else if (scores[cat] === maxScore) { winningCategories.push(cat); }
      }
      let finalCategory = winningCategories.length > 1
        ? winningCategories[Math.floor(Math.random() * winningCategories.length)]
        : winningCategories[0];

      finalResultCategory = finalCategory;
      findEl('#q' + totalQuestions).classList.remove('active');
      findEl('#result-container').style.display = 'block';
      findEl('#result-title').textContent = testConfig.categories[finalCategory].title;
      findEl('#result-image').src = testConfig.resultImages[finalCategory] || '';
      findEl('#result-description').innerHTML = testConfig.categories[finalCategory].description;
    }

    async function loadImageAsDataURL(imageUrl) {
      return new Promise(async (resolve, reject) => {
        try {
          const response = await fetch(imageUrl);
          if (!response.ok) throw new Error(`Ошибка сети при загрузке изображения: ${response.status} ${response.statusText}`);
          const blob = await response.blob();
          const reader = new FileReader();
          reader.onloadend = () => resolve(reader.result);
          reader.onerror = () => reject(new Error('Ошибка при чтении данных изображения.'));
          reader.readAsDataURL(blob);
        } catch (e) {
          reject(new Error(`Не удалось загрузить изображение: ${e.message}`));
        }
      });
    }

    async function saveResult() {
      if (!finalResultCategory) { alert("Результат не определен."); return; }
      try {
        const title = testConfig.categories[finalResultCategory].title;
        const descriptionHTML = findEl('#result-description').innerHTML;
        const imageUrl = findEl('#result-image').src;
        const imageDataUrl = await loadImageAsDataURL(imageUrl);
        const htmlContent = `<!DOCTYPE html>
<html lang="ru"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1.0"><title>${title}</title>
<style>
body{font-family:'Roboto','Helvetica Neue',Arial,sans-serif;line-height:1.6;color:#212121;max-width:1000px;margin:0 auto;padding:25px;background-color:#f5f5f5}
.result-container{background:#fff;border-radius:50px;box-shadow:0 2px 4px rgba(0,0,0,.1),0 4px 8px rgba(0,0,0,.05);padding:35px}
.result-title{text-align:center;color:#212121;margin-bottom:25px;font-weight:500}
.result-image{width:100%;height:auto;border-radius:25px;margin:25px 0;box-shadow:0 2px 4px rgba(0,0,0,.1),0 4px 8px rgba(0,0,0,.05)}
.result-description{text-align:left;padding:20px;background:#fafafa;border-radius:50px;box-shadow:0 1px 3px rgba(0,0,0,.05);line-height:1.7}
.result-description li{margin-bottom:.6em}
</style></head>
<body><div class="result-container"><h1 class="result-title">${title}</h1><img src="${imageDataUrl}" alt="Результат: ${title}" class="result-image"><div class="result-description">${descriptionHTML}</div></div></body></html>`;
        const blob = new Blob([htmlContent], { type: 'text/html;charset=utf-8' });
        const url = URL.createObjectURL(blob);
        const a = document.createElement('a');
        a.href = url;
        a.download = `результат_${finalResultCategory}.html`;
        document.body.appendChild(a);
        a.click();
        setTimeout(() => {
          document.body.removeChild(a);
          URL.revokeObjectURL(url);
        }, 100);
      } catch (error) {
        console.error("Ошибка при сохранении результата:", error);
        alert(`Не удалось сохранить результат: ${error.message || 'Произошла ошибка.'}`);
      }
    }
    function restartTest() {
  currentQuestionIndex = 0;
  finalResultCategory = null;
  for (let cat in scores) scores[cat] = 0;
  findEl('#result-container').style.display = 'none';
  shadow.querySelectorAll('.question-container').forEach(q => q.classList.remove('active'));
  findEl('#q1').classList.add('active');
  shadow.querySelectorAll('input[type="radio"]').forEach(radio => radio.checked = false);
  updateProgressBar();
}

shadow.addEventListener('click', (event) => {
  const target = event.target;
  if (target.classList.contains('material-button')) {
    target.style.transform = 'translateY(0)';
    target.style.boxShadow = '0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24)';
    setTimeout(() => {
      if (target.isConnected) { target.style.transform = ''; target.style.boxShadow = ''; }
    }, 150);
  }
  if (target.id === 'next-btn-1') {
    nextQuestion(1);
  } else if (target.classList.contains('next-btn')) {
    const questionNum = parseInt(target.dataset.question);
    if (!isNaN(questionNum)) nextQuestion(questionNum);
  } else if (target.classList.contains('prev-btn')) {
    const questionNum = parseInt(target.dataset.question);
    if (!isNaN(questionNum)) prevQuestion(questionNum);
  } else if (target.id === 'show-result-btn') {
    showResult();
  } else if (target.id === 'save-result-btn') {
    saveResult();
  } else if (target.id === 'restart-btn') {
    restartTest();
  }
});

updateProgressBar();

}


// --- ИНИЦИАЛИЗАЦИЯ ДЛЯ ЛК (контент подгружается асинхронно) ---
function tryInit() {
const el = document.getElementById('constructor-test-container');
if (el && !el.dataset.inited) {
initConstructorTest();
return true;
}
return !!(el && el.dataset.inited);
}


if (!tryInit()) {
const obs = new MutationObserver(() => {
if (tryInit()) obs.disconnect();
});
obs.observe(document.documentElement, { childList: true, subtree: true });
}
})();
</script>
