---
title: Возобновление использования привилегий администратора для Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как помочь клиентам возобновить использования привилегий администратора партнера, чтобы партнер мог помочь в управлении клиентскими подписками Azure CSP.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811334"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Возобновление использования привилегий администратора для клиентских подписок Azure CSP  

**Подходящие роли**

- Глобальный администратор
- Агент по администрированию

Клиенты часто ожидают, что так как вы являетесь партнером CSP, то вы будете управлять использованием ресурсов Azure и их системами. Для этого требуются привилегии администратора. Одни привилегии предоставляются при установлении отношений торгового посредника между вами и клиентом. Другие привилегии предоставляются вашим клиентом.

## <a name="admin-privileges-for-azure-in-csp"></a>Привилегии администратора для Azure в CSP

Существуют два уровня привилегий администратора для Azure в CSP.

**Привилегии администратора уровня клиента** (**делегированные привилегии**). Партнеры CSP получают эти привилегии при установлении отношений торгового посредника CSP с клиентами. Это обеспечивает партнерам CSP доступ к арендаторам своих клиентов, что позволяет им выполнять административные функции, такие как добавление пользователей и управление ими, сброс паролей и управление лицензиями пользователей.

**Привилегии администратора уровня подписки**. Партнеры CSP получают эти привилегии при создании подписок Azure в CSP для своих клиентов. Такие привилегии обеспечивают партнерам в рамках CSP полный доступ к данным подпискам, что позволяет им подготавливать ресурсы Azure и управлять ими.

## <a name="reinstate-csp-partners-admin-privileges"></a>Возобновление использования привилегий администратора для партнеров CSP

Чтобы повторно получить делегированные привилегии администратора, необходимо обратиться к своему клиенту.

1. Войдите в Панель мониторинга Центра партнеров и в меню Центра партнеров выберите **Клиенты**.

2. Выберите клиента, с которым вы работаете, и **запросите установление отношений, в которых вы выполняете роль торгового посредника**. Будет создана ссылка на клиента, у которого есть привилегии администратора арендатора.

3. Этот пользователь должен выбрать ссылку и утвердить запрос на установление отношений, в которых вы выполняете роль торгового посредника.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Отношения, в которых вы выполняете роль торгового посредника":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Добавление группы агентов по администрированию в качестве владельца подписки Azure CSP

Клиенту потребуется добавить группу агентов по администрированию в качестве владельца подписки Azure в CSP.

1. Используйте консоль PowerShell или интегрированную среду сценариев PowerShell (ISE). Убедитесь, что установлены модули AzureAD.

2. Подключитесь к арендатору Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Получение ObjectId групп агентов по администрированию.

   ```powershell
   Get-AzureADGroup
   ```
   Следующие шаги выполняются пользователем в компании клиента, у которого есть доступ владельца к подписке Azure в CSP.

4. Пользователю с правами владельца подписки Azure в CSP следует войти в Azure с использованием своих учетных данных.

   ```powershell
   Connect-AzAccount
   ```

5. Затем этот пользователь может добавить группу агентов по администрированию в качестве владельца подписки Azure в CSP.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>Дальнейшие действия

[Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)
