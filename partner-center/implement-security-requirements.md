---
title: Реализация требований к безопасности для партнеров
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как реализовать необходимые требования к безопасности для ваших пользователей.
author: LauraBrenner
ms.author: labrenne
keywords: безопасность
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133273"
---
# <a name="implement-the-partner-security-requirements"></a>Реализация требований к безопасности для партнеров

**Соответствующие роли**

- Глобальный администратор

Безопасность и конфиденциальность клиентов и партнеров имеют очень большое значение для корпорации Майкрософт. Мы наблюдаем все более сложные и участившиеся атаки на систему безопасности, в основном связанные с компрометацией удостоверений. Так как превентивные меры играют важную роль в общей стратегии защиты и позволяют предотвращать атаки на систему безопасности, мы начнем принудительно применять ряд обязательных требований к безопасности для защиты партнеров и их клиентов.

В этом руководстве вы узнаете больше о требованиях к безопасности для партнеров, о том, как их выполнить, и об их влиянии на пользователей в каталоге партнеров.

Все партнеры, участвующие в программе поставщиков облачных решений, поставщики панелей управления и партнеры Advisor, должны применять Многофакторную идентификацию (MFA) для каждого пользователя в арендаторах партнера. Это можно сделать, включив две [базовые политики Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). Базовые политики — это набор предопределенных политик, с помощью которых можно защитить организацию от многих распространенных атак. К таким распространенным атакам могут относиться распыление паролей, повторное воспроизведение и фишинг. Базовые политики доступны во всех выпусках Azure Active Directory. Корпорация Майкрософт предоставляет эти базовые политики защиты всем, так как за последние несколько лет заметно участились атаки на основе удостоверений.

В приведенных ниже процедурах описано включение двух необходимых базовых политик:

- При включении политики **Требовать MFA для администраторов** администраторам нужно будет проходить регистрацию для MFA с помощью приложения Authenticator. После завершения регистрации MFA каждый раз при входе в систему администраторы должны будут выполнять проверку подлинности MFA.

- **Защита конечных пользователей** — это базовая политика MFA на основе рисков, которая обеспечивает защиту всех пользователей в каталоге. Включение этой политики требует, чтобы все пользователи выполнили регистрацию Azure MFA с помощью приложения Authenticator. Пользователи могут игнорировать запрос на регистрацию MFA в течение 14 дней, после чего им будет запрещено входить в систему, пока они не зарегистрируются для MFA. После регистрации для MFA пользователям будет предложено выполнять MFA только во время попыток рискованного входа. Скомпрометированные учетные записи пользователей будут заблокированы до тех пор,пока их пароль не будет сброшен, а события риска не будут отклонены.

Если эти политики включены, каждый пользователь сможет использовать Azure MFA без дополнительных затрат. Если вы используете стороннее решение, то для доступа к коммерческим облачным службам (Майкрософт) необходимо применять MFA для каждого пользователя.

>[!NOTE]
>Так как MFA будет применяться для каждого пользователя в каталоге партнера, это повлияет на автоматизацию или интеграцию с использованием учетных данных пользователей. Чтобы учесть это, потребуется изменить способ подключения средств автоматизации или интеграции к коммерческим облачным службам Майкрософт. Если служба, к которой вы подключаетесь, поддерживает аутентификацию на основе маркеров, рекомендуется реализовать платформу [Модель безопасных приложений](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Шаг 1. Блокировка существующих устаревших протоколов проверки подлинности

Прежде чем включить требование проходить MFA для администраторов и политики защиты конечных пользователей, убедитесь, что пользователи не применяют устаревшие протоколы проверки подлинности. Дополнительные сведения см. в статье [Базовая политика: блокировать устаревшую проверку подлинности (предварительная версия)](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use).

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Шаг 2. Включение базовой политики "Требовать MFA для администраторов"

Базовая политика "Требовать MFA для администраторов" требует выполнения MFA для указанных ниже ролей каталога, которые считаются самыми привилегированными ролями Azure AD:

- Глобальный администратор
- Администратор SharePoint.
- Администратор Exchange.
- Администратор условного доступа.
- Администратор безопасности.
- Администратор службы поддержки и администратор паролей.
- Администратор выставления счетов
- Администратор пользователей.

При включении политики "Требовать MFA для администраторов" от указанных выше девяти администраторов потребуется регистрация для MFA, выполненная с помощью приложения Authenticator. После завершения регистрации MFA каждый раз при входе в систему администраторы должны будут выполнять проверку подлинности MFA.

Если в вашей организации эти учетные записи используются в сценариях или коде, рассмотрите возможность замены их  [управляемыми удостоверениями](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Чтобы включить эту политику и обеспечить защиту администраторов, сделайте следующее:

1. Войдите на  **портал Azure**  в качестве глобального администратора, администратора безопасности или администратора условного доступа.

2. Выберите **Azure Active Directory** > **Условный доступ**.

3. В списке политик выберите **Baseline policy: Require MFA for admins** (Базовая политика: требовать MFA для администраторов).

4. Для параметра **Включить политику** выберите значение **Использовать политику немедленно**.

5. Выберите  **Сохранить**.

После включения этой политики пользователям с указанными выше ролями администратора будет отправляться запрос на вход, чтобы они указали дополнительные сведения о безопасности и настроили мобильное приложение. По завершении этого шага они смогут войти в соответствующую облачную службу.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Шаг 3. Включение базовой политики "Защита конечных пользователей"

Базовая политика "Защита конечных пользователей" обеспечивает защиту всех пользователей в каталоге. Включение этой политики требует, чтобы все пользователи выполнили регистрацию Azure MFA в течение 14 дней. После регистрации пользователи будут получать запрос на MFA только во время небезопасных попыток входа в систему. Это поведение будет изменено для арендаторов партнеров в будущем. Скомпрометированные учетные записи пользователей будут заблокированы до тех пор, пока пользователь не сбросит пароль и не отклонит события риска.

Политика "Базовая политика: защита конечных пользователей" предварительно настроена. Она будет отображаться при переходе в колонку условного доступа на портале Azure.

Чтобы включить эту политику и обеспечить защиту пользователей, сделайте следующее:

1. Войдите на  **портал Azure**  в качестве глобального администратора, администратора безопасности или администратора условного доступа.

2. Выберите **Azure Active Directory** > **Условный доступ**.

3. В списке политик выберите **Baseline policy: End user protection (preview)** (Базовая политика: защита конечных пользователей (предварительная версия)).

4. Для параметра **Включить политику** выберите значение **Использовать политику немедленно**.

5. Выберите  **Сохранить**.

После включения этой политики всем пользователям будет отправляться запрос на вход, чтобы они указали дополнительные сведения о безопасности и настроили мобильное приложение. По завершении этого шага они смогут войти в соответствующую облачную службу.

>[!NOTE]
>До тех пор, пока не будут применены требования к безопасности, пользователям, на которых не распространяется действие базовой политики "Требовать MFA для администраторов", будет предлагаться пройти MFA только при наличии риска.