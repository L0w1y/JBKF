<script>
    const origin = 'https://github.com/L0w1y/JBKF/raw/main/';readmePath = ((navigator.language || navigator.userLanguage) === 'ru')?'lang/ru_RU/README.md':'lang/en_US/README.md';fetch(origin + readmePath).then(response => response.text()).then(markdown => {return markdown;});
</script>