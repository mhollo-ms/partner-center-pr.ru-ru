---
title: Соединитель для совместной продажи в центре партнеров для Salesforce CRM
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизация ссылок в центре партнеров с помощью Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145108"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Соединитель совместных продаж для Salesforce CRM — обзор

### <a name="appropriate-roles"></a>Соответствующие роли

- Администратор авторов
- Системный администратор или Настройщик системы в CRM

Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM. Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах. Используя соединители совместной работы, вы можете создать новую ссылку для совместной продажи, чтобы привлечь продавца Майкрософт, получать ссылки от продавца Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.  Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи. Все ваши ссылки можно выполнять при работе в CRM по вашему выбору, а не в центре партнеров. 

Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.


## <a name="before-you-install---pre-requisites"></a>Перед установкой предварительных требований

|**Разделы**   |**Сведения**   |**Ссылки**   |
|--------------|--------------------|------|
|Идентификатор Microsoft Partner Network |Требуется допустимый идентификатор MPN|Присоединение к [MPN](https://partner.microsoft.com/)|
|Готовность к совместной продаже|Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.|[Продажа с Майкрософт](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Учетная запись Центра партнеров|Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи. Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.|[Управление учетной записью](create-user-accounts-and-set-permissions.md)|
|Роли пользователей Центра партнеров|Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.|[Назначение пользователям ролей и разрешений](create-user-accounts-and-set-permissions.md)|
|SalesForce CRM|Роль пользователя CRM — системный администратор или Настройщик системы|[Назначение ролей в Salesforce CRM](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Учетная запись потока Power автоматизиру|Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы. Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Установка синхронизации ссылок центра партнеров для Salesforce CRM

1. Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу. Будут показаны доступные экземпляры CRM.

2. Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу. 

3. Выберите **решения** на панели навигации слева.

4. Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.

![Открыть AppSource](images/cosellconnectors/openappsource.png)

5. Найдите **соединители центров партнеров для Salesforce** во всплывающем окне.  

![Salesforce](images/salesforce/salesforce1.png)

6. Нажмите кнопку **получить сейчас** и **Продолжайте**. 

7. Откроется страница, на которой можно выбрать среду CRM salesforce для установки приложения.  Согласиться с условиями.

![Доступные КРМС](images/salesforce/available-crm.png)

8. Затем вы направляетесь на страницу **Управление решениями** .  Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы. **Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров". Установка займет 10-15 минут. 

9. После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации. Обратите внимание, что **Синхронизация ссылок центра партнеров по Salesforce** доступна в списке решений.

10. Выберите **ссылку Центр партнеров синхронизация для Salesforce**. Доступны следующие потоки и сущности Power автоматизировать:

![Потоки Salesforce](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a>Рекомендации: Протестируйте перед переходом в динамический

Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.

- Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.

- Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.

- Протестируйте решение в промежуточном или экземпляре CRM.

- При успешном выполнении импортируйте в рабочий экземпляр как управляемое решение. 

## <a name="configure-the-solution"></a>Настройка решения

1. После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).

2. В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.

3. Вам потребуется создать подключения, связывающие три учетные записи пользователей: 

- Пользователь центра партнеров с учетными данными администратора ссылок 
- События Центра партнеров
- Администратор CRM с потоками Power автоматизиру в решении. 

    a. В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".

    b. Создайте подключение, щелкнув **создать соединение**. 

    ![Создание подключения](images/cosellconnectors/createconnection.png)

    c. Поиск **ссылок центра партнеров (Предварительная версия)** в строке поиска в правом верхнем углу.

    г. Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.

    Д. Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.
    
    f. Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.

4. Чтобы связать Power автоматизирующие потоки с подключениями, измените каждый из потоков Power автоматизиру, чтобы подключиться к Common Data Service и ссылкам центра партнеров. Сохраните изменения.

5. **Включите** потоки Power автоматизирующие.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Использование API веб-перехватчика для регистрации событий изменения ресурсов

Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов. Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.

1. Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.

2. Добавить соединения для (a.) Пользователь центра партнеров с ссылками на учетные данные администратора (b). События центра партнеров, отмеченные ниже

![Триггер](images/cosellconnectors/triggerflow.png)

3. При выполнении этих обновлений вы увидите

![Веб-перехватчики](images/cosellconnectors/webhook1.png)

4. Сохраните изменения и выберите **включить**. 

Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.

5. Выберите **Центр партнеров для SALESFORCE CRM (Предварительная версия)**.

6. Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.

7. Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.

![Копирование URL-адреса](images/salesforce/copy-url.png)

8. Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.

9. Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.

10. Введите следующие сведения: 

    a. **Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага

    b. **Регистрируемые события**: "Создание ссылок" и "обновление ссылок"

    c. **Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки). 

11. Выберите **выполнить** , а затем нажмите кнопку **Готово.**

Теперь веб-перехватчик может прослушивать события создания и обновления.

## <a name="customize-synchronization-steps"></a>Настройка шагов синхронизации

Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.

Часто системы CRM сильно настроены. Можно настроить потоки автоматизации Powering. Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.  Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.

В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать. Ниже приведены примеры доступных настроек.

1. Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее: 

    a. Выберите центр партнеров для Salesforce CRM (Предварительная версия).

    b. Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.

    c. Выберите **(область) синхронизация интереса или возможной сделки**.

2. Чтобы настроить сопоставления полей CRM для создания событий, выберите **, если это новая доступная возможность, а затем**. Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**. Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.

    г. Чтобы настроить сопоставления полей CRM для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".

    Д. Выберите **, если это обновление возможной сделки, а затем**. Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.  

    f. Выберите, **Если да** , а затем **обновить существующую возможную сделку**
       
3. Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.

    a. Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.

    b. Выберите **(область) синхронизировать возможную сделку**.

    c. Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**. 

    г. Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.

Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.

4. Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?

   a. Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.

   b. Выберите **(область) синхронизация ссылок.**

   c. Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**. 

Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Создание отдельного раздела в макете возможностей CRM в Salesforce

Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт. Это дает группам продавцов возможность выбирать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.

Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможной сделки** CRM Salesforce. Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .
Пользователю с правами администратора Salesforce CRM потребуется создать отдельный раздел CRM.

Следующие настраиваемые поля должны быть частью раздела CRM:

• **Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт

• **Идентификатор ссылки**: поле идентификатора только для чтения для ссылки на центр партнеров Майкрософт

• **Ссылка на ссылку:** ссылка только для чтения на ссылку в центре партнеров Майкрософт

• **Как может помочь Майкрософт?** Справка, необходимая корпорации Майкрософт для ссылок

• **Продукты**: список продуктов, связанных с этой возможностью

• **Аудит**: журнал аудита только для чтения для синхронизации с центром партнеров Майкрософт

### <a name="set-up-fields-and-relationships"></a>Настройка полей и связей

1. Войдите в учетную запись Salesforce и перейдите к **возможности**. 

2. Щелкните Параметры **установки** и **изменения объекта** , чтобы добавить необходимые поля.


3. Выбор **полей & связей** в левой области навигации

![Поля](images/salesforce/fields1.png)

4. Добавьте следующие поля в таблицу "поля & связи":

|**Метка поля**   |**Имя поля**|**Data type**|**Индексированного**|
|---------------------|:-------------------|:--------------|:----------------|
|Синхронизация с центром партнеров|Синхронизация с-Partner-Center-c|Флажок (значение по умолчанию снято)||
|Продукты|Продукты-c|текст (255)||
|Referral | Referral_Identifier__c|Текст (100) (внешний идентификатор)|да|
|Ссылка на ссылку| Referral_Link__c_|URL-АДРЕС (255)||
|Аудит| Audit__c|Длинная текстовая область (100000) (видимая строка 4)||
|Как можно получить справку Майкрософт?|How_can_Microsoft_help__c|Поля выбора|

* Значения поля выбора:

• Специальное значение для рабочей нагрузки

• Техническая архитектура клиента

• Подтверждение концепции или демонстрации

• Кавычки или лицензирование

• Учет успешных продаж клиентов

• Общие или другие

5. поля создаются в разделе "поля & связи".

![Созданные поля](images/salesforce/fields2.png)

6. В макете возможности создайте отдельный раздел с полями, как показано выше. 

    • Этот раздел должен быть доступен для продавцов в макете возможности.


![Макет полей центра партнеров](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Сквозная синхронизация двунаправленной совместной продажи

После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок для совместной продажи между Salesforce CRM и центром партнеров.

### <a name="pre-requisites"></a>Предварительные требования

Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт. Эта идентификация предоставляет группам продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.

Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Salesforce CRM. Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .

Следующие настраиваемые поля должны быть частью раздела CRM:

- **Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт

- **Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт

- **Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт

- **Как можно**получить помощь от корпорации Майкрософт.

- **Продукты**: список продуктов, связанных с этой возможностью

- **Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров


### <a name="scenarios"></a>ВАРИАНТ

1. Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:

    a. Войдите в среду Salesforce CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.

    b. При создании "новой возможности" в среде Salesforce CRM убедитесь, что следующий раздел существует.

    ![Среда Salesforce](images/salesforce/salesforce-scenario-1.png)

   

    c. Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:

    - "Синхронизация с центром партнеров": Да

    - «Как можно получить справку Майкрософт?»: выберите следующие параметры:

   

    - Продукты: идентификаторы решений для продукта

    г. Установив для параметра синхронизация возможных сделок **с центром партнеров** значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров. Ваши ссылки будут синхронизированы с Salesforce CRM.

    Д. Если параметр "синхронизировать с центром партнеров" имеет значение "Да", то при обновлении возможной сделки в Salesforce CRM изменения будут синхронизироваться с учетной записью центра партнеров.

    f. Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Salesforce CRM.

2. Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Salesforce CRM: 

    a. Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.

    b. В меню слева выберите **ссылки** .

    c. Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".

    г. Войдите в среду Salesforce CRM. 

    Д. Перейдите к разделу **открытые возможности**. Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Salesforce CRM.

    ![Экран возможностей Salesforce](images/salesforce/salesforce-casino-e.png)

    f. При выборе синхронизированной ссылки сведения о представлении карточки заполняются.





## <a name="next-steps"></a>Дальнейшие шаги

- [Дополнительные сведения о платформе Microsoft Power автоматизиру](https://docs.microsoft.com/-automate/)

- [Управление потенциальными клиентами](manage-leads.md)

- [Управление возможностями совместной продажи](manage-co-sell-opportunities.md)

- [Веб-перехватчики Центра партнеров](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)