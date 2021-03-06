---
title: Добавление нескольких пользователей для учетной записи клиента
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, отправьте файл данных в центр партнеров, используя формат файла значений с разделителями-запятыми (CSV).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535744"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Передача CSV-файла пользователей в учетную запись клиента


**Относится к**

- Центр партнеров

**Соответствующие роли**

- Глобальный администратор

Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Создание файла пользователей клиентов и отправка их в учетную запись клиента

1. Создайте файл данных с разделителями-запятыми (CSV) с данными, описанными выше. Сохраните файл, чтобы выбрать его позднее. [Чтобы импортировать нескольких пользователей для учетной записи клиента, см. поля для CSV-файла](file-customer-users.md). 

2. Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.

3. В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.

4. Выберите вкладку **Пользователи и лицензии** клиента, а затем щелкните **отправить пользователей**.

5. В разделе **Передача данных пользователя** нажмите кнопку **Обзор**.

6. В средство выбора файлов выберите ваш файл данных, а затем нажмите **Открыть**.

7. Выберите **Проверить**.

    **Примечание**    . Большинство ошибок создания учетной записи вызвано проблемами с файлами данных, в том числе отсутствующими сведениями, неправильно сформированными или повторяющимися адресами электронной почты или слишком большим числом записей в файле.

8. После того как центр партнеров проверит файл, выберите географическое **Расположение** для новых пользователей.
9. Щелкните **Сохранить**.
10. Скачайте временный пароль нового пользователя.

    >[!IMPORTANT]
    > Не забудьте скачать файл с временными паролями, так как вы не сможете сделать это позже. Новым пользователям необходимо выполнить вход в новую учетную запись, используя временный пароль.

11. Новым пользователям автоматически назначаются разрешения **Может использовать лицензии и службы**. 

## <a name="next-steps"></a>Дальнейшие действия

- [Предоставление клиентам доступа в центре партнеров для приобретения своих продуктов или услуг](give-customers-permission.md)
