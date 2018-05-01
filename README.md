1. Устанавливаем nodejs https://nodejs.org/en/download/
2. По инструкции устанавливаем https://yarnpkg.com/lang/en/
3. В терминале для Windows __yarn add global gulp__ и для Unix __sudo yarn add global gulp__
4. Клонируем git clone https://github.com/linedotwww/mockup.git
5. Переходим в папку, там командой yarn install устанавливаем все
6. Временное решение, в файле node_modules/gulp-css-url-adjuster/index.js нужно заменить строчку ```javascript if (url.indexOf('data:') === 0) {``` на ```javascriptif (url.indexOf('data:') === 0 || url.indexOf('http') === 0 || url.indexOf('font') === 0) {```
7. Теперь подключать файлы в templates/main/source/styles/style.scss не нужно, все подключается автоматом
8. Пользовательские стили могут лежать тут templates/main/source/styles/users либо в компонентах
9. В компонентах можно создавать json файлы, пример лежит в меню и потом работать с данными в шаблоне
10. В стилях путь к картинкам не прописываем, только название файла, пути в html файлах можем прописывать как ```html <img src="{{src}}logo.png" alt="" class="logo__pic">```
10. Две команды есть, gulp и gulp build
