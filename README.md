1. Устанавливаем nodejs https://nodejs.org/en/download/
2. По инструкции устанавливаем https://yarnpkg.com/lang/en/
3. В терминале для Windows __yarn add global gulp__ и для Unix __sudo yarn add global gulp__
4. Клонируем git clone https://github.com/linedotwww/mockup.git
5. Переходим в папку, там командой yarn install устанавливаем все
6. Временное решение, в файле node_modules/gulp-css-url-adjuster/index.js нужно заменить строчку ```javascript if (url.indexOf('data:') === 0) {``` на ```javascriptif (url.indexOf('data:') === 0 || url.indexOf('http') === 0 || url.indexOf('font') === 0) {```
