# server-app
Клиент-серверное приложение, с базой данных, регистрацией клиентов, запросом имени/фамилии/email/пароля( и т.д.), под защитой SpringSecurity. 
Использован алгоритм хэширования паролей BCrypt.
Простое spring mvc приложение, с ипользованием spring boot, spring security и framework. 
Имеем слой контроллеров, который предоставляет страницы с расширением ftlh. 
Контроллер осуществляет обработку http и предоставляет страницы написанные на freemarker.
Модель User Мапится в таблицу и работает с базой данных. Eсть отдельный репозиторий, который базируется на технологии Spring GPA.
Отдельно настроена безопасность, которая пускает на страницу SainUp и SainIn, и не пускает на страницу Users.
Hастроен доступ UserDeteilService который достает из базы информацию о пользователе по его емэйлу, и оборачивает в обьект UserDeteilImpl который имплементрует интерфейс UserDeteils и отвечает на вопросы которые задает Spring Security.
