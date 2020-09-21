---
title: Application Center Insights — отчеты о Клаудасцентии выручки
description: Сведения об отчетах о Клаудасцентии, которые находятся на панели мониторинга центра партнеров.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 510f85b053ec17fa0a2a66217a19c006e7ca2bc9
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811383"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="87c3e-103">Отчеты о Клаудасцентии доступности, доступные на панели мониторинга центра партнеров</span><span class="sxs-lookup"><span data-stu-id="87c3e-103">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="87c3e-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="87c3e-104">**Appropriate roles**</span></span>
- <span data-ttu-id="87c3e-105">Средство просмотра исполнительных отчетов</span><span class="sxs-lookup"><span data-stu-id="87c3e-105">Executive report viewer</span></span>
- <span data-ttu-id="87c3e-106">Средство просмотра отчетов</span><span class="sxs-lookup"><span data-stu-id="87c3e-106">Report viewer</span></span>

<span data-ttu-id="87c3e-107">На панели мониторинга центра партнеров содержатся загружаемые данные о выручкой из программы Клаудасцент.</span><span class="sxs-lookup"><span data-stu-id="87c3e-107">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="87c3e-108">В данных отображаются сведения о выручкой клиентов для приобретения продуктов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-108">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="87c3e-109">В этой статье описывается разбивка этих данных, использование оценки и то, что это значит.</span><span class="sxs-lookup"><span data-stu-id="87c3e-109">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="87c3e-110">Сводные определения</span><span class="sxs-lookup"><span data-stu-id="87c3e-110">Summary definitions</span></span>

- <span data-ttu-id="87c3e-111">**Пользователи SMC**— это общее число клиентов в загружаются загрузок.</span><span class="sxs-lookup"><span data-stu-id="87c3e-111">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="87c3e-112">Клиенты определяются партнером по записи.</span><span class="sxs-lookup"><span data-stu-id="87c3e-112">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="87c3e-113">**Соглашения об истечении срока действия**— в пределах текущего финансового года мы предоставляем число соглашений об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="87c3e-113">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="87c3e-114">**Срок действия дохода**— доход, связанный с соглашениями об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="87c3e-114">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="87c3e-115">**Срок действия открытого дохода**— доход, связанный с открытыми соглашениями об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="87c3e-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="87c3e-117">Сегментация SMB Клаудасцент</span><span class="sxs-lookup"><span data-stu-id="87c3e-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="87c3e-118">Сегмент малого и среднего бизнеса (SMB) дополнительно делится на три отдельных подсегмента.</span><span class="sxs-lookup"><span data-stu-id="87c3e-118">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="87c3e-119">" **Лучшие неуправляемые** " включает в себя наибольшее число клиентов SMB с наибольшими возможными сделками для Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="87c3e-120">Типичные лучшие неуправляемые клиенты имеют аналогичные характеристики в качестве управляемых учетных записей, с большим количеством сотрудников, большими ИТ бюджетами и расходами, а также большими объемами потенциального дохода корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-120">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="87c3e-121">Мы определяем первые неуправляемые два способа:</span><span class="sxs-lookup"><span data-stu-id="87c3e-121">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="87c3e-122">**Лучшие неуправляемые пользователи**— включает учетные записи с 300 или более сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="87c3e-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="87c3e-123">Учетные записи на основе пользователей — это отличные целевые объекты для первого приобретения или расширения таких продуктов, как M365, D365 или Surface.</span><span class="sxs-lookup"><span data-stu-id="87c3e-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="87c3e-124">**Лучшие неуправляемые на основе вычислений** — включает учетные записи с потенциальным объемом Azure более чем на 10 000.</span><span class="sxs-lookup"><span data-stu-id="87c3e-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="87c3e-125">Учетные записи на основе вычислений включают существующий Azure.</span><span class="sxs-lookup"><span data-stu-id="87c3e-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="87c3e-126">учетные записи с значительным годом в будущем и учетными записями, у которых еще нет возможности приобрести Azure, но потенциально могут быть больше, чем на 10 000.</span><span class="sxs-lookup"><span data-stu-id="87c3e-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="87c3e-127">**Компания среднего бизнеса** включает в себя существующих клиентов и учетные записи делового отношения с 25 до 300 сотрудников.</span><span class="sxs-lookup"><span data-stu-id="87c3e-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="87c3e-128">**Малый бизнес** включает в себя все остальные компании, у которых менее 25 сотрудников.</span><span class="sxs-lookup"><span data-stu-id="87c3e-128">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Клиент по типу SMC.":::

<span data-ttu-id="87c3e-130">**Лучшие неуправляемые** и **средние** подсегменты представляют высокие значения времени жизни (ЛТВ) для партнеров Майкрософт и Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-130">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="87c3e-131">Поэтому они являются ведущими областями, влияющими на рост в этом сегменте.</span><span class="sxs-lookup"><span data-stu-id="87c3e-131">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="87c3e-132">В этих двух подсегментах мы лучше полагаться на приобретение сокета с помощью M365, монетизации в дальнейшем с D365 или бизнес-приложениями Azure, а также реализовать высокий ЛТВ для Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-132">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="87c3e-133">Сегодня у нас есть две основные области возможностей — 1.</span><span class="sxs-lookup"><span data-stu-id="87c3e-133">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="87c3e-134">Наши клиенты расширяют возможности роста; открыт.</span><span class="sxs-lookup"><span data-stu-id="87c3e-134">our customer adds growth; 2.</span></span> <span data-ttu-id="87c3e-135">Хотя мы очень хорошо получаем облачные сокеты, ведущие с M365, у нас есть большая возможность в D365 и Azure.</span><span class="sxs-lookup"><span data-stu-id="87c3e-135">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="87c3e-136">На следующем снимке экрана представлены три подсегмента SMB и оптимизированные маршруты к рынку.</span><span class="sxs-lookup"><span data-stu-id="87c3e-136">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="87c3e-137">Клаудасцент назначает приоритеты для профилирования, оценки и моделирования всех ведущих неуправляемых и средних бизнес-учетных записей.</span><span class="sxs-lookup"><span data-stu-id="87c3e-137">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Снимок экрана: подсегменты SMB.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="87c3e-139">Клаудасцент Машинное обучение</span><span class="sxs-lookup"><span data-stu-id="87c3e-139">CloudAscent Machine Learning</span></span>

<span data-ttu-id="87c3e-140">Протокол SMB использует технологию машинного обучения для управления прогнозами продаж и маркетинга в рамках основных неуправляемых и средних бизнес-сегментов.</span><span class="sxs-lookup"><span data-stu-id="87c3e-140">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="87c3e-141">Как собираются и включаются в рекомендации по выручкой?</span><span class="sxs-lookup"><span data-stu-id="87c3e-141">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="87c3e-142">**Сбор данных**. веб-обходчики проверяют и собираются миллиарды клиентских сигналов путем проверки связи с доменами компании и мониторинга: публикации в блогах, Пресс-релизы, социальные потоки и технические форумы.</span><span class="sxs-lookup"><span data-stu-id="87c3e-142">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="87c3e-143">Помимо собранных сигналов фирмографикс сведения собираются из внутренних и внешних источников, таких как D&B, внутренняя подписка Майкрософт и данные о транзакциях.</span><span class="sxs-lookup"><span data-stu-id="87c3e-143">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="87c3e-144">**Машинное обучение**. сигналы поступают в модель машинного обучения, которая выводит структурированный набор данных прогнозов продаж и маркетинга для каждого клиента по облачным продуктам и кластерам.</span><span class="sxs-lookup"><span data-stu-id="87c3e-144">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="87c3e-145">Каждый клиент оценивается с помощью похожих моделей на основные SMB Майкрософт, которые определяют соответствие клиента и алгоритмы машинного обучения, которые интегрируют интерактивное поведение клиента, определяются как намерение.</span><span class="sxs-lookup"><span data-stu-id="87c3e-145">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="87c3e-146">Эта оценка объединяется в кластеры, которые показывают, как выделяются покупатели для приобретения Microsoft Cloud продуктов.</span><span class="sxs-lookup"><span data-stu-id="87c3e-146">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="87c3e-147">**Оптимизация**. машинное обучение система оптимизирует модели, используя данные транзакций ежемесячно, а данные подписки ежеквартально.</span><span class="sxs-lookup"><span data-stu-id="87c3e-147">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="87c3e-148">Используя данные выигрыша и потери, Машинное обучение корректирует алгоритмы и проверяет, что модели работают должным образом, сравнивая рекомендации кластера с возможностями, выполненными на главном сервере.</span><span class="sxs-lookup"><span data-stu-id="87c3e-148">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Снимок экрана машинного обучения SMB.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="87c3e-150">Клаудасцентие выручки</span><span class="sxs-lookup"><span data-stu-id="87c3e-150">CloudAscent Propensity</span></span>

<span data-ttu-id="87c3e-151">Как создаются рекомендации по выручкой?</span><span class="sxs-lookup"><span data-stu-id="87c3e-151">How are propensity recommendations created?</span></span>

<span data-ttu-id="87c3e-152">Используя сигналы, собранные с помощью веб-обходчиков и данных из различных источников, мы консолидируем данные фирмографикс и сигналы социальных сетей клиента.</span><span class="sxs-lookup"><span data-stu-id="87c3e-152">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="87c3e-153">Эта оценка использует эти сигналы и данные в моделях сравнения для соответствия и оценки моделей.</span><span class="sxs-lookup"><span data-stu-id="87c3e-153">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="87c3e-154">Соответствие учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="87c3e-154">Customer Account Fit</span></span>

   - <span data-ttu-id="87c3e-155">Внутренние и внешние точки данных, определяющие фирмографикс.</span><span class="sxs-lookup"><span data-stu-id="87c3e-155">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="87c3e-156">Оценка соответствия использует ту же модель, что и наш лучший протокол SMB для сравнения клиентов, и позволяет узнать, подходят ли они для Microsoft Cloud продуктов.</span><span class="sxs-lookup"><span data-stu-id="87c3e-156">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="87c3e-157">Оценка соответствия обновляется ежеквартально</span><span class="sxs-lookup"><span data-stu-id="87c3e-157">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="87c3e-158">Цель учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="87c3e-158">Customer Account Intent</span></span>

   - <span data-ttu-id="87c3e-159">Сигналы, связанные с социальными носителями и определением поведения клиента в Интернете, определяют намерение.</span><span class="sxs-lookup"><span data-stu-id="87c3e-159">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="87c3e-160">Оценка намерения перемещается поверх, чтобы определить кластеры.</span><span class="sxs-lookup"><span data-stu-id="87c3e-160">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="87c3e-161">Оценка намерения обновляется ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="87c3e-161">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Клаудасцент прогнозные модели SMB.":::

3. <span data-ttu-id="87c3e-163">Кластеризация</span><span class="sxs-lookup"><span data-stu-id="87c3e-163">Clustering</span></span>

   <span data-ttu-id="87c3e-164">Сигналы для соответствия и намерения объединяются в оценку кластеризации.</span><span class="sxs-lookup"><span data-stu-id="87c3e-164">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="87c3e-165">Клаудасцент имеет четыре кластера:</span><span class="sxs-lookup"><span data-stu-id="87c3e-165">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="87c3e-166">Действующие сейчас — клиенты, готовые к продажам</span><span class="sxs-lookup"><span data-stu-id="87c3e-166">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="87c3e-167">Оцените клиентов, готовых к маркетингу</span><span class="sxs-lookup"><span data-stu-id="87c3e-167">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="87c3e-168">Обучайте — кампании по осведомленности о поддержке дисков</span><span class="sxs-lookup"><span data-stu-id="87c3e-168">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="87c3e-169">Обучение — обучение и отслеживание намерения</span><span class="sxs-lookup"><span data-stu-id="87c3e-169">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="87c3e-170">Кластеризация позволяет пользователям ориентироваться на конкретные клиенты по продажам и маркетингу на основе коэффициентов сегментов, например: продукта, географической, отрасли и вертикальной.</span><span class="sxs-lookup"><span data-stu-id="87c3e-170">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="87c3e-171">На вкладке **модель выручки** в книгах клаудасцент используются общие показатели выручки и предполагаемого пробела.</span><span class="sxs-lookup"><span data-stu-id="87c3e-171">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="87c3e-172">Чтобы определить кластеризацию и цель, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="87c3e-172">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="87c3e-173">Используя модели машинного обучения, мы сначала Рассчитайте оценку соответствия и оценку намерения заказчика на шкале 100.</span><span class="sxs-lookup"><span data-stu-id="87c3e-173">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="87c3e-174">Точные показатели будут зависеть от моделей машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="87c3e-174">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="87c3e-175">Пример оценки ниже:</span><span class="sxs-lookup"><span data-stu-id="87c3e-175">Example Scores Below:</span></span>

         |<span data-ttu-id="87c3e-176">**Классификация**</span><span class="sxs-lookup"><span data-stu-id="87c3e-176">**Classification**</span></span>|<span data-ttu-id="87c3e-177">**Оценка**</span><span class="sxs-lookup"><span data-stu-id="87c3e-177">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="87c3e-178">Высокий</span><span class="sxs-lookup"><span data-stu-id="87c3e-178">High</span></span>|<span data-ttu-id="87c3e-179">75-100</span><span class="sxs-lookup"><span data-stu-id="87c3e-179">75 - 100</span></span>|
         |<span data-ttu-id="87c3e-180">Средний</span><span class="sxs-lookup"><span data-stu-id="87c3e-180">Medium</span></span>|<span data-ttu-id="87c3e-181">55-74</span><span class="sxs-lookup"><span data-stu-id="87c3e-181">55 - 74</span></span>|
         |<span data-ttu-id="87c3e-182">Низкий</span><span class="sxs-lookup"><span data-stu-id="87c3e-182">Low</span></span>|<span data-ttu-id="87c3e-183">30 - 54</span><span class="sxs-lookup"><span data-stu-id="87c3e-183">30 - 54</span></span>|
         |<span data-ttu-id="87c3e-184">Очень низкий</span><span class="sxs-lookup"><span data-stu-id="87c3e-184">Very Low</span></span>|<span data-ttu-id="87c3e-185">0 - 29</span><span class="sxs-lookup"><span data-stu-id="87c3e-185">0 - 29</span></span>|

      2. <span data-ttu-id="87c3e-186">Используя приведенное выше правило, мы будем классифицировать компании как высокие, средние, низкие и очень низкие по отношению к обоим клиентам.</span><span class="sxs-lookup"><span data-stu-id="87c3e-186">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="87c3e-187">Мы выводите сигналы соответствия и намерения клиентов по двухмерной матрице с каждым пересечением, представляющим выручкой.</span><span class="sxs-lookup"><span data-stu-id="87c3e-187">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="87c3e-188">Например, высокая степень соответствия + высокая цель = a1, представляющая наибольшую степень выручки.</span><span class="sxs-lookup"><span data-stu-id="87c3e-188">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="87c3e-189">Наконец, эти сегменты группируются в виде кластеров.</span><span class="sxs-lookup"><span data-stu-id="87c3e-189">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="87c3e-190">Например, a1, a2, A3, A4 формируют кластер "подготовить сейчас".</span><span class="sxs-lookup"><span data-stu-id="87c3e-190">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Модели Клаудасцент.":::

   <span data-ttu-id="87c3e-192">Для этих клиентов рекомендуется ориентироваться на "действовать сейчас" и оценивать клиентов.</span><span class="sxs-lookup"><span data-stu-id="87c3e-192">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="87c3e-193">Клаудасцент Products & Models</span><span class="sxs-lookup"><span data-stu-id="87c3e-193">CloudAscent Products & Models</span></span>

<span data-ttu-id="87c3e-194">На следующем рисунке представлено представление каждой модели выручки в Клаудасцент:</span><span class="sxs-lookup"><span data-stu-id="87c3e-194">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Модель Клаудасцентного распределителя.":::

<span data-ttu-id="87c3e-196">Модели пробельных символов состоят из прогнозов для существующих клиентов Майкрософт, где они не имеют продукта и (или) являются клиентами новых перспективных клиентов.</span><span class="sxs-lookup"><span data-stu-id="87c3e-196">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="87c3e-197">При продаже моделей используются данные транзакций для прогнозирования потенциальных продаж в Azure и SKU M365.</span><span class="sxs-lookup"><span data-stu-id="87c3e-197">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="87c3e-198">EOS использует конечные клиенты для Win 7, Office 2010, SQL Server и Windows Server.</span><span class="sxs-lookup"><span data-stu-id="87c3e-198">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="87c3e-199">Данные EOS извлекаются из MS Sales и перемещаются с моделированием Клаудасцентя, где это возможно.</span><span class="sxs-lookup"><span data-stu-id="87c3e-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="87c3e-200">Данные EOS находятся в современных работах и в продажах Azure.</span><span class="sxs-lookup"><span data-stu-id="87c3e-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>