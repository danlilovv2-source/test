```html
<!DOCTYPE html>
<html lang="ru">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <link rel="stylesheet" href="css/styles.css">
</head>

<body class="boot">

    <!-- CRT эффекты -->
    <div class="scanlines"></div>
    <div class="flicker"></div>
    <div class="noise-overlay"></div>

    <!-- Основной терминал -->
    <main id="terminal" class="terminal">

        <!-- Экран -->
        <section id="bootScreen" class="boot-screen">
            <pre id="bootText"></pre>
            <div id="bootPrompt" class="boot-prompt"></div>
            <button id="startBtn" class="start-btn" style="display:none;"></button>
        </section>

        <!-- Контент -->
        <section id="content" class="content" style="display:none;"></section>

        <!-- Поле ввода -->
        <div id="inputLine" class="input-line" style="display:none;">
            <span class="prompt-symbol"></span>
            <span id="inputBuffer"></span>
            <span class="cursor"></span>
            <span id="autoComplete" class="autocomplete"></span>
        </div>

    </main>

    <!-- Аудио -->
    <audio id="sndHum" loop></audio>
    <audio id="sndBeep"></audio>
    <audio id="sndType"></audio>
    <audio id="sndGlitch"></audio>
    <audio id="sndCrash"></audio>
    <audio id="sndClick"></audio>

    <!-- Скрытый input -->
    <input id="hiddenInput" type="text" autocomplete="off" autocorrect="off" spellcheck="false">

    <script src="js/data.js"></script>
    <script src="js/sound.js"></script>
    <script src="js/script.js"></script>
</body>

</html>
```

Удалено:

* название страницы
* текст кнопки
* символ `>`
* символ курсора `█`
* все видимые надписи

Структура и эффекты терминала сохранены.
