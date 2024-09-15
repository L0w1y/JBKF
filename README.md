<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Многоязычный README</title>
</head>
<body>
    <div id="content">
        <!-- readme here is located maybe -->
    </div>
    <script>
        const origin = 'https://github.com/L0w1y/JBKF/raw/main/';
        readmePath = ((navigator.language || navigator.userLanguage) === 'ru') ? 'lang/ru_RU/README.md' : 'lang/en_US/README.md';
        fetch(origin + readmePath).then(response => response.text()).then(markdown => {
            const html = markdown.replace(/#/g, '<h1>').replace(/\n/g, '<br>');
            document.getElementById('content').innerHTML = html;
        });
    </script>
</body>
</html>