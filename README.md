# Введение в компьютерную безопасность

## Описание курса

Программа и материалы курса «Введение в компьютерную безопасность»
образовательной программы по направлению подготовки (специальности)
10.05.01 «Компьютерная безопасность», преподаваемого в [Национальном исследовательском Томском государственном университете](http://www.tsu.ru) на [кафедре защиты информации и киптографии](http://isc.tsu.ru)

## Вопросы

1. Введение в предмет компьютерной безопасности
    * подходы к определению безопасности
    * базовое определение защищенной информационной системы (ИС)
    * направления в компьютерной безопасности
    * профессии в компьютерной безопасности
    * соотношение информационной, кибер и компьютерной безопасности
    * роль криптографии в компьютерной безопасности
    * мифы компьютерной безопасности
    * [классические принципы защищенности Зальцера и Шредера](http://www.cs.virginia.edu/~evans/cs551/saltzer/)
1. Основные термины компьютерной безопасности
    * угроза
    * недостаток
    * уязвимость
    * атака
    * безопасность
    * защищенность
    * политика безопасности
1. Уязвимости
    * формальное определение уязвимости
    * [модель Engle-Whalen-Bishop] (http://nob.cs.ucdavis.edu/bishop/notes/2008-cse-14/2008-cse-14.pdf)
    * классификация уязвимостей
    * каталоги [CWE] (http://cwe.mitre.org/), [CVE] (http://cve.mitre.org/) и [CAPEC] (http://capec.mitre.org/) 
1. Политика безопасности и механизмы защиты
    * Превентивные (preventive), смягчающие (mitigative), детективные (detective) и коррективные (corrective) механизмы
    * Многоуровневая защита
    * Безопасность через сокрытие 
    * Безопасность систем с открытым и закрытым исходным кодом
1. Основные этапы разработки защищенных ИС 
1. Моделирование угроз
    * Основные модели угроз 
        * модель [CIA] (http://en.wikipedia.org/wiki/Information_security)
        * модель [STRIDE] (http://msdn.microsoft.com/en-us/library/ee823899(v=cs.20).aspx)
        * модель МакКамбера
        * модель Паркера
   * Риск-ориентированный подход к компьютерной безопасности
        * модель [DREAD] (http://msdn.microsoft.com/en-us/library/ff648644.aspx)
        * модель [CVSS] (http://nvd.nist.gov/cvss.cfm?calculator&version=2)
   * Построение модели угроз в виде диаграммы потока данных
1. Управление доступом
   * Идентификация, аутентификация и авторизация
   * Аутентификация
       * парольная аутентификация
       * [gesture-based аутентификация] (http://en.wikipedia.org/wiki/Draw_a_Secret)
       * биометрическая аутентификация
       * двухфакторная аутентификация
       * технологии AAA и SSO
   * Политики управление доступом и информационными потоками
       * дискреционное управление доступом (DAC)
       * мандатное управление доступом ([LBAC] (http://en.wikipedia.org/wiki/Lattice-based_access_control), [MLS] (http://en.wikipedia.org/wiki/Multilevel_security), [TE] (http://en.wikipedia.org/wiki/Type_enforcement))
       * ролевое управление доступом (RBAC)
       * атрибутное управление доступом (ABAC)
       * элементы формального моделирования
   * Классические модели безопасности
       * модель Харрисона-Руззо-Ульмана
       * модель Take-Grant
       * модель [Белла-ЛаПадулы] (http://en.wikipedia.org/wiki/Bell%E2%80%93LaPadula_model)
   * Скрытые каналы
       * определение, назначание и виды скрытых каналов
       * общая схема функционирования скрытых каналов
       * примеры скрытых каналов по памяти и по времени
1. Защищенность сетей
   * Основные принципы функционирования компьютерных сетей
   * [Одна секунда из жизни пакета](http://habrahabr.ru/post/191954/)
   * Классические сетевые атаки
       * TCP-hijacking
       * [DoS-](http://en.wikipedia.org/wiki/Denial-of-service_attack), [DDoS-](http://www.cisco.com/web/about/security/intelligence/guide_ddos_defense.html), [DRDoS-](http://blog.cloudflare.com/deep-inside-a-dns-amplification-ddos-attack/)атаки
       * ARP-spoofing
   * Классические сетевые механизмы защиты 
       * Межсетевые экраны
       * Системы обнаружения вторжений
       * Виртуальные частные сети (VPN)
1. Элементы криптографических протоколов
   * Виды протоколов 
   * Протоколы SSL/TLS
   * PKI
1. Анализ защищенности
   * тестирование
   * технологии [SAST](http://sgordey.blogspot.ru/2013/08/blog-post_13.html), [DAST] (http://sgordey.blogspot.ru/2013/08/0day-11.html) и [IAST](http://www.youtube.com/watch?v=sUNsPBb6NPA)
   * [тестирование на проникновение](http://www.youtube.com/watch?v=X0ilODBepU8&feature=youtu.be)
1. Практические аспекты
   * ответственное разглашение и программы Bug Bounty
   * соревнования по защите информации CTF
1. Дружелюбная безопасность (Usable security)
   * Модели взаимодействия
   * [NEAT](http://blogs.msdn.com/b/sdl/archive/2011/05/04/adding-usable-security-to-the-sdl.aspx)
   
## Задания
1. Алиса и Боб - сотрудники Банка. Алиса работает бухгалтером и каждый вечер, после завершения работы Банка с клиентами, должна отправить секретный дневной отчет в Центробанк. Затем этот отчет сохраняется в архиве на жестком диске. Для шифрования каналов передачи данных используется специальное программно-аппаратное обеспечение, реализующее алгоритм ГОСТ 28147-89. Боб работает в службе безопасности. Для обеспечения доверенной загрузки ОС на компьютере установлен специальный аппаратный модуль, осуществляющий аутентификацию пользователя до загрузки этой ОС по аппаратному ключу, который хранится у Боба. Для аутентификации в ОС необходимо также знать пароль, который хранится у Алисы. Пароль должен иметь длинну не менее 16 символов и содержать цифры, большие и маленькие буквы и спецсимволы. Ни Боб, ни Алиса самостоятельно не могут загрузить ОС. Компьютер находится на рабочем месте Алисы. Каждое утро Боб приходит к Алисе, и они вместе загружают ОС на компьютере, после чего Алиса начинает свою работу. Некто Мэлори поставил перед собой цель раскрыть перед обществом финансовые показатели Банка и хочет получить доступ как можно к большему количеству секретных отчетов. Необходимо построить [дерево атак] (https://en.wikipedia.org/wiki/Attack_tree), описывающее как Мэлори можно получить хотя бы один.
2. Построить модель угроз в виде DFD для простейшего веб-приложения, используя Microsoft Threat Modeling Tool.
3. Самостоятельно вычислить оценку для 3-х наиболее известных уязвимостей, обнаруженных за последний год, используя методики [DREAD](https://msdn.microsoft.com/en-us/library/aa302419.aspx) и [CVSSv2](https://nvd.nist.gov/CVSS-v2-Calculator).
4. Проанализировать следующий код веб-приложения и найти в нем недостатки и уязвимости, если таковые имеются:

   ```
<?php
    if (isset($_GET['redirect'])) {
        header('Location: '.$_GET['redirect']);
    }
    header('Set-Cookie: _afUserId='. $_GET['userId']);
    header('Set-Cookie: _afGroupId='. $_GET['groupId']);
?>
<html>
    <head>
        <meta http-equiv="refresh" content="5;url=<?=$_GET['url']?>"></meta>
    </head>
    <body>
          <?php
              $roleId = explode(":", base64_decode($_COOKIE['roleId']))[0];
              if ($roleId == 'admin') {
                  include 'admin_interface.php';
              }
              elseif ($roleId == 'user') {
                  include 'user_interface.php'
              }
              else {
                  echo '<h2>Unknown role '.$roleId.'\n</h2>';
              }
          ?>

    </body>
</html>
   ```

5. Написать приложение, содержащее какую-либо уязвимость, необнаруживаемую сканером безопасности (false negative), а также приводящее к генерации сканером сообщения о наличии уязвимости, отсутствующей на самом деле (false positive). Пример: веб-приложение содержащее [недостатки предварительной обработки данных в SQL-запросах](http://cwe.mitre.org/data/definitions/89.html), приводящих к возниконовению уязвимости к атаке [SQL-injection] (https://capec.mitre.org/data/definitions/66.html), необнаруживаемой сканером [Sqlmap](http://sqlmap.org/) и не содержащее [недостатки предварительной обработки данных, выводящихся пользователю](http://cwe.mitre.org/data/definitions/79.html), но ошибочно считаемое уязвимым к атаке [XSS] (https://capec.mitre.org/data/definitions/18.html) сканером [ZAP](https://code.google.com/p/zaproxy/).
6. Устранить, выбранный класс уязвимостей в приложении [Gruyere](https://google-gruyere.appspot.com/) или [DVWA](http://www.dvwa.co.uk/) путем изменения исходного кода приложения.
7. На произвольном языке программирования написать код для клиента и сервера, реализующих [скрытый канал](https://en.wikipedia.org/wiki/Covert_channel) по времени с использованием любого механизма операционной системы, например:
    * создание сокета
    * доступ к файлу
    * жесткие ссылки
    * символические ссылки
    * файловая система /proc
    * загрузка процессора
    * наличие установленного сетевого соединения
8. Проанализировать и сравнить защищенность конфигураций SSL/TLS любых 10 популярных веб-ресурсов с помощью [сканера ssllabs.com](http://www.ssllabs.com)

## Материалы

### Обязательные
* [Matt Bishop. Introduction to Computer Security.](http://nob.cs.ucdavis.edu/book/book-intro/) Chapter 1 
* [Подкаст Noise Security Bit. Об образовании в области ИБ](http://noisebit.podster.fm/6)
* [Подкаст Noise Security Bit. О практической безопасности](http://noisebit.podster.fm/3)
* [А. Карпов. Краткая история хакерства] (http://habrahabr.ru/company/yandex/blog/244559/)
* [В. Кочетков. Как разработать защищенное веб-приложение и не сойти при этом с ума](http://my.webinar.ru/record/140584/)
* [В. Кочетков. Информационная угрозология, уязвимоведение и рисководство](http://habrahabr.ru/post/129386/)
* [А. Масалович. Конкурентная разведка в Интернет](http://www.youtube.com/watch?v=HcwASJCk16k)
* [Н.А. Гайдамакин. Теоретические основы компьютерной безопасности.](http://elar.urfu.ru/bitstream/10995/1778/5/1335332_schoolbook.pdf) Глава 1.
* [А. Гостев. Особенности национальной охоты](https://www.youtube.com/watch?v=Canud1V4Fww)
* [В. Дубровин. Ошибки использования безопасных протоколов и их эксплуатация](http://live.digitaloctober.ru/embed/2996#time1400752650)
* [А. Петухов. Обзор ограничений современных технологий в области ИБ] (https://events.yandex.ru/lib/talks/2692/)

### Рекомендуемые
* П.Н. Девянин. Модели безопасности компьютерных систем. Управление доступом и информационными потоками. 2-е изд.
* С.П. Расторгуев. Информационная война. Проблемы и модели. Экзистенциальная математика
* К. Касперски. Техника сетевых атак

### Справочные
* [Matt Bishop. Computer Security: Art and Sciense](http://nob.cs.ucdavis.edu/book/book-aands/)
* [А.В. Лукацкий. Моделирование угроз](http://www.slideshare.net/lukatsky/ss-13257562)

## Оценка уровня знаний по компьютерной безопасности
* [Information Security Interview Questions](http://danielmiessler.com/study/infosec_interview_questions/)
* [Security Related Interview Questions for all Engineers](https://www.netmeister.org/blog/security-questions.html)
* [Application security related questions for developers](https://teamquiz.aspectsecurity.com)
* [XSS Game](https://xss-game.appspot.com/)
* [Gruyere codelab](https://google-gruyere.appspot.com/)
* [The Matasano Crypto Challenges](http://cryptopals.com/)
