---
title: Как рассчитывается получившийся кредит от партнера
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как рассчитывается план Azure для получения кредита (PEC). Сюда входят требования к допустимости для партнеров и косвенных поставщиков.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 065cf0c8f95667b470081edcb1b66398235604b3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948140"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a>Как рассчитывается кредитный счет партнера (PEC) для партнеров в программе поставщика облачных решений

**Соответствующие роли**

- Глобальный администратор
- Администратор выставления счетов

Партнеры, владеющие Круглосуточная эксплуатацией ИТ или всей среды Azure своих клиентов в CSP, получают с помощью PEC. PEC предоставляется в качестве части счета партнеру, имеющему прямую связь с корпорацией Майкрософт. Кредит вычисляется ежедневно и отражается в месячном счете. По умолчанию в CSP партнерам предоставляются необходимые права доступа к подписке клиента, позволяющие круглосуточно управлять ресурсами в подписке и управлять ими. Дополнительные способы, с помощью которых клиент может подготавливать доступ для передействующего партнера, описаны в следующем разделе.


## <a name="important-eligibility-and-calculation-requirements"></a>Важные требования к допустимости и вычислениям:

- Партнер должен иметь активное соглашение MPN и допустимую роль управления учетными записями на основе правил (RBAC), чтобы получить заработанный кредит для ресурсов Azure, которыми они управляют. Дополнительные сведения [допустимые роли RBAC]

- Косвенный поставщик будет иметь право на PEC, если они или их непрямое торговые посредники, или оба имеют Круглосуточная оперативный контроль и управление ресурсами Azure клиента в CSP.

- Партнерский кредит связан с оплачиваемым (платным) использованием инфраструктуры Azure клиента в CSP, управляемой партнером. 

- PEC доступен только партнерам в CSP, за которые взимается плата Майкрософт (косвенный поставщик и прямой счет).

- Подходящие службы: заработанный кредитный курс применяется ко всем ресурсам Azure 1PP Azure, указанным в прайс-списке. Существуют исключения, включая, но не ограниченные, 3PP и резервирование Azure.

- PEC вычисляется ежедневно и может быть просмотрен в ежедневном разведывательную файле. Партнер (поставщик или торговый посредник (через поставщика услуг) должен иметь доступ ко всему дню (круглосуточно), чтобы гарантировать получение PEC.

- Партнерский кредит начисляется на уровне ресурсов Azure. Если у партнера есть допустимый доступ в подписке или на уровне группы ресурсов, каждый ресурс, который имеет роль до более высокой сущности, будет получать PEC. 

- PEC будет включен в ежемесячный счет партнера. В счете указана чистая оплата. Сведения отображаются в файле счета разведывательную.

Сведения о получении доступа к управлению подписками Azure и о том, как связать идентификатор MPN с ролями RBAC, см. в статье [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md).

Дополнительные сведения

- [План Azure — выставление счетов](azure-plan-billing.md)

- [Прейскурант для новой коммерческой модели в CSP](azure-plan-price-list.md)