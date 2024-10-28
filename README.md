#### Выполнил: Путинцев А.В.
***

Это мой получается 2 проект этого курса веб-разработки от сайта яндекс практикум . Проект предоставляет собой одностраничный сайт 
В первом проете я собирал первую часть , затронув вертстку позиционирование языка HTML .Во втором проекте были применены новые навыки с анимациями шрифтами 


В этот проект были вставлены два видео [два](https://www.youtube.com/watch?v=arj7oStGLkU) и [видео](https://www.youtube.com/watch?v=5MgBikgcWnY).

---
Планы по доработке проекта:

* подключить другие шрифты;
* добавить  образовательные видео;
* проверить код на кроссбраузерность и дописать все вендорные префиксы;
* задизайнить форму, через которую пользователи смогут отправить вам комментарий.

----
### Исходный код 


'''html

<!DOCTYPE html>
<html lang="ru">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./pages/index.css">
    <title>Научиться учиться</title>
  </head>
  <body class="page">
    <header class="header">
      <div class="logo logo_place_header"></div>
      <h1 class="header__title">Научиться учиться</h1>
      <p class="header__subtitle">
        Какие современные и эффективные подходы к обучению вы можете
        использовать в своей жизни?
        <a href="#" class="header__link" target="_blank">Узнать &rarr;</a>
      </p>
      <img
        src="./images/header-image.png"
        class="header__main-illustration"
        alt="Тут должна быть картинка"
      >
      <div class="header__square-pic rotation"></div>
    </header>
    <main class="content">
      <section class="description" aria-label="две колонки">
        <article class="two-columns">
          <h2 class="two-columns__brier">Главные проблемы в обучении</h2>
          <div class="two-columns__main-text">
            <p class="two-columns__paragraph">
              Ни в школе, ни в институте нас не учат тому, как правильно изучать
              материал. Мы готовимся к экзаменам и учим билеты. Мы тренируемся
              решать однообразные задачи, чтобы лучше сдать тест, но часто в
              итоге это не дает нам реального знания. Зубрежка быстро
              выветривается и не приносит пользы.
            </p>
            <p class="two-columns__paragraph">
              <span class="two-columns__span-accent">Вывод:</span> учиться тоже
              нужно уметь, но почему-то этому мало где учат. Что с этим делать?
            </p>
            <p class="two-columns__paragraph">
              Конкретные техники и упражнения помогают изменить подход к
              обучению, сделать его эффективным и захватывающим. Эти же техники
              применяются на примере обучения в Практикуме.
            </p>
          </div>
        </article>
      </section>
      <section class="techniques">
        <h2 class="section-title">Техники обучения</h2>
        <h3 class="section-subtitle">Пять практик от Барбары Оакли</h3>
        <ul class="cards">
          <li class="cards__item">
            <img
              class="cards__image"
              src="./images/cards-attention.png"
              alt="Тут должно быть изображение"
            >
            <h4 class="cards__title">Два вида внимания</h4>
            <p class="cards__description">
              Глубокие знания возникают, если чередовать сфокусированное и
              рассеянное мышление
            </p>
          </li>
          <li class="cards__item">
            <img
              class="cards__image"
              src="./images/cards-recall.png"
              alt="Тут должно быть изображение"
            >
            <h4 class="cards__title">Recall</h4>
            <p class="cards__description">
              Вспоминайте изученное - это позволит соединить разрозенные порции
              памяти
            </p>
          </li>
          <li class="cards__item">
            <img
              class="cards__image"
              src="./images/cards-interliving.png"
              alt="Тут должно быть изображение"
            >
            <h4 class="cards__title">Интерливинг</h4>
            <p class="cards__description">
              Изучайте несколько навыков одновременно, они обогащают друг друга.
            </p>
          </li>
          <li class="cards__item">
            <img
              class="cards__image"
              src="./images/cards-question.png"
              alt="Тут должно быть изображение"
            >
            <h4 class="cards__title">Вопросы</h4>
            <p class="cards__description">
              Слушая преподавателя, придумывайте хороший вопрос, который вас
              действительно волнует.
            </p>
          </li>
          <li class="cards__item">
            <img
              class="cards__image"
              src="./images/cards-competence.png"
              alt="Тут должно быть изображение"
            >
            <h4 class="cards__title">Иллюзия компетентности</h4>
            <p class="cards__description">
              Повторите про себя, запишите, расскажите другу: вам только
              кажется, что вы владеете новой темой.
            </p>
          </li>
        </ul>
      </section>
      <section class="video">
        <h2 class="section-title">Видео на TED</h2>
        <h3 class="section-subtitle">Для тех, кто любит прокрастинировать</h3>
        <div class="video__iframes">
          <iframe
            class="video__iframe"
            src="https://www.youtube.com/embed/5MgBikgcWnY"
            title="YouTube video player"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
          <iframe
            class="video__iframe"
            src="https://www.youtube.com/embed/arj7oStGLkU"
            title="YouTube video player"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </section>
      <section class="oakley" aria-label="две колонки">
        <article class="two-columns">
          <h2 class="two-columns__brier">
            История Барбары Оакли
          </h2>
          <div class="two-columns__main-text">
            <p class="two-columns__paragraph">
              С детства Барбаре не давалась математика. Она считала себя
              законченным гуманитарием, причём далеко не самым умным. В армии
              она изучала русский язык, чтобы получить надбавку, да так успешно,
              что её выдвинули в командиры. Но для продвижения по службе нужно
              было сдавать математику. И тогда Барбара придумала свой подход к
              точным наукам. Оказалось, если вам что-то «плохо даётся», ваши
              добытые трудом знания гораздо глубже, чем у тех, кому всё ясно с
              первого взгляда.
            </p>
          </div>
        </article>
      </section>
      <section class="feynman">
        <h2 class="feynman__title">Метод Фейнама</h2>
        <p class="feynman__subtitle">Выучить и не забыть</p>
        <a class="feynman__link" href="#" target="_blank">Подробнее &rarr;</a>
        <img
          src="./images/feynman.png"
          class="feynman__circle"
          alt="Тут должна быть картинка"
        >
      </section>
      <section class="digits">
        <h2 class="section-title">Цифры и факты</h2>
        <h3 class="section-subtitle">Про учёбу и мозг</h3>
        <ul class="table">
          <li class="table__cell">
            <h4 class="table__heading">86 миллиардов</h4>
            <p class="table__text">Число нейронов в мозге человека</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">2,1 миллиарда</h4>
            <p class="table__text">
              Число нуждающихся в повышении квалификации
            </p>
            <p class="table__text">Всемирный Банк, 2017</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">1000 терабайт</h4>
            <p class="table__text">Объем памяти человека</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">500 триллионов</h4>
            <p class="table__text">
              Число ответственных за обучение нервных синапсов у взрослого
            </p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">420 миллионов</h4>
            <p class="table__text">
              Число взрослых людей моложе 25 лет, не имеющих образования для
              трудоустройства
            </p>
            <p class="table__text">Всемирный Банк, 2017</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">17-20 лет</h4>
            <p class="table__text">Пик обучаемости</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">1885 год</h4>
            <p class="table__text">Открытие кривой забывания</p>
          </li>
          <li class="table__cell">
            <h4 class="table__heading">1889 год</h4>
            <p class="table__text">Открытие условного рефлекса</p>
          </li>
        </ul>
      </section>
      <section class="khan">
        <div class="khan__container">
          <p class="khan__author">Салман Хан</p>
          <h2 class="khan__title">Весь мир - школа</h2>
          <blockquote class="khan__quote">
            Страсть и новаторство Сала Хана меняют процесс обучения миллионов
            студентов по всему миру. Книгу «Весь мир — школа» нужно прочитать
            всем, кто занимается образованием — так учащиеся повсюду смогут
            получить навыки и знания, которые приносят успех в школе, карьере и
            жизни.
          </blockquote>
          <p class="khan__quote-autor">Джордж Лукас</p>
          <p class="khan__quote-autor-subline">Кинорежиссер, продюссер</p>
          <div class="khan__book-container">
            <img
              src="./images/khan-book.jpg"
              class="khan__book-pic"
              alt="Тут должна быть картинка книги"
            >
            <a class="khan__buy-link" href="#" target="_blank"
              >Купить книгу &rarr;</a
            >
          </div>
        </div>
      </section>
      <section class="kaufman">
        <h2 class="section-title section-title_theme_dark">
          Принципы обучения
        </h2>
        <h3 class="section-subtitle section-subtitle_theme_dark">
          от Джоша Кауфмана
        </h3>
        <ul class="table table_theme_dark">
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">1</h4>
            <p class="table__text table__text_theme_dark">
              Выберите привлекательный проект.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">2</h4>
            <p class="table__text table__text_theme_dark">
              Сосредоточьтесь на каком-то одном навыке.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">3</h4>
            <p class="table__text table__text_theme_dark">
              Определите целевой уровень мастерства.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">4</h4>
            <p class="table__text table__text_theme_dark">
              Разбейте навык на элементы.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">5</h4>
            <p class="table__text table__text_theme_dark">
              Приготовьте всё необходимое для занятий.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">6</h4>
            <p class="table__text table__text_theme_dark">
              Устраните препятствия для занятий.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">7</h4>
            <p class="table__text table__text_theme_dark">
              Выделите специальное время для занятий.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">8</h4>
            <p class="table__text table__text_theme_dark">
              Создайте быстрые петли обратной связи.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">9</h4>
            <p class="table__text table__text_theme_dark">
              Занимайтесь по расписанию, короткими интенсивными интервалами.
            </p>
          </li>
          <li class="table__cell table__cell_theme_dark">
            <h4 class="table__heading table__heading_theme_dark">10</h4>
            <p class="table__text table__text_theme_dark">
              Уделяйте внимание количеству и скорости.
            </p>
          </li>
        </ul>
        <div class="kaufman__triangle rotation"></div>
      </section>
      <section class="resources">
        <h2 class="section-title">Полезные ресурсы</h2>
        <h3 class="section-subtitle">
          Больше материалов о техниках и лайфхаках обучения
        </h3>
        <div class="resources__logo-zone">
          <a href="#" class="resources__link" target="_blank">
            <img
              src="./images/logo/resources-arzamas.svg"
              alt="Тут должен быть логотип"
              class="resources__logo"
            >
          </a>
          <a href="#" class="resources__link" target="_blank"
            ><img
              src="./images/logo/resources-n1.svg"
              alt="Тут должен быть логотип"
              class="resources__logo"
          ></a>
          <a href="#" class="resources__link" target="_blank"
            ><img
              src="./images/logo/resources-strelka.svg"
              alt="Тут должен быть логотип"
              class="resources__logo"
          ></a>
          <a href="#" class="resources__link" target="_blank"
            ><img
              src="./images/logo/resources-polka.svg"
              alt="Тут должен быть логотип"
              class="resources__logo"
          ></a>
        </div>
      </section>
    </main>
    <footer class="footer">
      <div class="footer__columns">
        <div class="footer__column footer__column_content_copyright">
          <a href="#" class="logo logo_place_footer" target="_blank"></a>
          <p class="footer__author">&copy; Виктор Абанькин</p>
        </div>
        <nav class="footer__column footer__column_content_info">
          <h2 class="footer__column-heading">О Практикуме</h2>
          <ul class="footer__column-links">
            <li>
              <a href="#" class="footer__column-link">Главные</a>
            </li>
            <li>
              <a href="#" class="footer__column-link">Концепция</a>
            </li>
            <li>
              <a href="#" class="footer__column-link">Наставники</a>
            </li>
          </ul>
        </nav>
        <nav class="footer__column footer__column_content_social">
          <h3 class="footer__column-heading">Соцсети</h3>
          <ul class="footer__column-links">
            <li>
              <a class="footer__column-link" href="#" target="_blank">
                <img
                  src="./images/youtube-icon.svg"
                  alt="Ютуб"
                  class="footer__social-icon"
                >YouTube
              </a>
            </li>
            <li>
              <a class="footer__column-link" href="#" target="_blank">
                <img
                  src="./images/vk_color_white.svg"
                  alt="Вконтакте"
                  class="footer__social-icon"
                >Вконтакте
              </a>
            </li>
            <li>
              <a class="footer__column-link" href="#" target="_blank">
                <img
                  src="./images/tiktok-icon.svg"
                  alt="ТикТок"
                  class="footer__social-icon"
                >TikTok
              </a>
            </li>
          </ul>
        </nav>
      </div>
    </footer>
  </body>
</html>