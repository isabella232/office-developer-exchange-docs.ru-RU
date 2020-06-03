---
title: Создание списка конечных точек автообнаружения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: Узнайте, как создать приоритетный список конечных точек автообнаружения.
localization_priority: Priority
ms.openlocfilehash: db888c8d562f57bd46edc251f4917e9e03d85d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528101"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a><span data-ttu-id="3d5b0-103">Создание списка конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3d5b0-103">Generate a list of Autodiscover endpoints</span></span>

<span data-ttu-id="3d5b0-104">Узнайте, как создать приоритетный список конечных точек автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-104">Find out how to generate a prioritized list of Autodiscover endpoints.</span></span>
  
<span data-ttu-id="3d5b0-105">Первая задача [процесса автообнаружения](autodiscover-for-exchange.md) — создание списка конечных точек автообнаружения приложения для попытки.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-105">The first task in the [Autodiscover process](autodiscover-for-exchange.md) is to generate a list of Autodiscover endpoints for your application to try.</span></span> <span data-ttu-id="3d5b0-106">Эти конечные точки автообнаружения могут быть получены из [поиска SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) или могут быть получены из адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-106">These Autodiscover endpoints can come from an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) or can be derived from the user's email address.</span></span> <span data-ttu-id="3d5b0-107">В конце вы можете создать большое количество конечных точек.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-107">In the end, you can end up with a large number of endpoints.</span></span> <span data-ttu-id="3d5b0-108">Давайте посмотрим, как можно упорядочивать их по приоритету.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-108">Let's take a look at how you can organize them by priority.</span></span> 
  
## <a name="start-with-scp-lookup"></a><span data-ttu-id="3d5b0-109">Начало поиска SCP</span><span class="sxs-lookup"><span data-stu-id="3d5b0-109">Start with SCP lookup</span></span>
<span data-ttu-id="3d5b0-110"><a name="bk_StartWithScp"> </a></span><span class="sxs-lookup"><span data-stu-id="3d5b0-110"><a name="bk_StartWithScp"> </a></span></span>

<span data-ttu-id="3d5b0-111">Конечные точки автообнаружения, поступающие из [поиска SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) , должны иметь наивысший приоритет в списке.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-111">Autodiscover endpoints that come from an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) should have top priority in your list.</span></span> <span data-ttu-id="3d5b0-112">Администраторы могут настроить объекты SCP для маршрутизации клиента в ближайшую или наиболее эффективную конечную точку автообнаружения, поэтому рекомендуется начать с этих конечных точек.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-112">Administrators can configure SCP objects to route your client to the closest or most efficient Autodiscover endpoint, so it is a good idea to start with these endpoints.</span></span> <span data-ttu-id="3d5b0-113">Так как процесс поиска SCP имеет собственную схему определения приоритетов, результаты поиска SCP уже имеют приоритет, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-113">Because the SCP lookup process has its own prioritization scheme, the results of an SCP lookup are already prioritized, as follows:</span></span> 
  
1. <span data-ttu-id="3d5b0-114">Конечные точки автообнаружения из объектов SCP заменяются на сайт Active Directory, к которому относится клиентский компьютер.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-114">Autodiscover endpoints from SCP objects scoped to the Active Directory site that the client computer belongs to.</span></span>
    
2. <span data-ttu-id="3d5b0-115">Конечные точки автообнаружения из объектов SCP не ограничены ни одним сайтом Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-115">Autodiscover endpoints from SCP objects not scoped to any Active Directory site.</span></span>
    
3. <span data-ttu-id="3d5b0-116">Конечные точки автообнаружения из объектов SCP заменяются на другой сайт Active Directory, чем сайт, к которому принадлежит клиентский компьютер.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-116">Autodiscover endpoints from SCP objects scoped to a different Active Directory site than the site that the client computer belongs to.</span></span>
    
<span data-ttu-id="3d5b0-117">После получения результатов процедуры поиска SCP можно добавить конечные точки, производные от адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-117">After you have the results of the SCP lookup process, you can add endpoints that derive from the user's email address.</span></span> <span data-ttu-id="3d5b0-118">Они могут использоваться в качестве набора конечных точек по умолчанию и резервного варианта в случае отсутствия результатов SCP или конечных точек, возвращенных из поиска SCP, недостаточно.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-118">These can serve as a default set of endpoints and a fallback in case there are no SCP results or the endpoints returned from the SCP lookup are not sufficient.</span></span>
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a><span data-ttu-id="3d5b0-119">Добавление конечных точек, производных от адреса электронной почты пользователя</span><span class="sxs-lookup"><span data-stu-id="3d5b0-119">Add endpoints derived from the user's email address</span></span>
<span data-ttu-id="3d5b0-120"><a name="bk_AddDerivedEndpoints"> </a></span><span class="sxs-lookup"><span data-stu-id="3d5b0-120"><a name="bk_AddDerivedEndpoints"> </a></span></span>

<span data-ttu-id="3d5b0-121">Если поиск SCP не работает или конечные точки, возвращенные функцией поиска SCP, не возвращают успешный ответ, можно получить набор конечных точек автообнаружения по умолчанию из адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-121">When SCP lookup doesn't work, or the endpoints returned by the SCP lookup don't return a successful response, you can derive a set of default Autodiscover endpoints from the user's email address.</span></span> <span data-ttu-id="3d5b0-122">Эти конечные точки должны иметь более низкий приоритет, чем все, которые берутся из поиска SCP, но они могут понадобиться, если не удалось выполнить поиск SCP.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-122">These endpoints should be a lower priority than any that come from an SCP lookup, but you might need them if the SCP lookup was not successful.</span></span>
  
### <a name="to-derive-autodiscover-endpoints"></a><span data-ttu-id="3d5b0-123">Получение конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3d5b0-123">To derive Autodiscover endpoints</span></span>

1. <span data-ttu-id="3d5b0-124">Извлеките имя домена из адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-124">Extract the domain name from the user's email address.</span></span> <span data-ttu-id="3d5b0-125">Например, если адрес электронной почты пользователя — Sadie.Daniels@contoso.com, доменное имя будет contoso.com.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-125">For example, if the user's email address is Sadie.Daniels@contoso.com, the domain name would be contoso.com.</span></span>
    
2. <span data-ttu-id="3d5b0-126">Создание URL-адресов конечных точек без расширений файлов в следующих форматах:</span><span class="sxs-lookup"><span data-stu-id="3d5b0-126">Construct endpoint URLs without file extensions in the following formats:</span></span>
    
  - <span data-ttu-id="3d5b0-127">"https://" + домен + "/Autodiscover/Autodiscover"</span><span class="sxs-lookup"><span data-stu-id="3d5b0-127">"https://" + domain + "/autodiscover/autodiscover"</span></span>
    
  - <span data-ttu-id="3d5b0-128">"https://autodiscover."</span><span class="sxs-lookup"><span data-stu-id="3d5b0-128">"https://autodiscover."</span></span> <span data-ttu-id="3d5b0-129">+ домен + "/Autodiscover/Autodiscover"</span><span class="sxs-lookup"><span data-stu-id="3d5b0-129">+ domain + "/autodiscover/autodiscover"</span></span>
    
<span data-ttu-id="3d5b0-130">После компиляции списка URL-адресов конечной точки, которые являются производными от поиска SCP и электронного адреса пользователя, может потребоваться изменить расширения имен файлов в этих URL-адресах в зависимости от того, используется ли [веб-служба автообнаружения SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) или [веб-служба автообнаружения POX](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3d5b0-130">After you compile the list of endpoint URLs that derive from both SCP lookup and the user's email address, you might need to revise file name extensions in those URLs, depending on whether you're using the [SOAP Autodiscover web service](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) or the [POX Autodiscover web service](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).</span></span>
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a><span data-ttu-id="3d5b0-131">Добавление или замена расширений имен файлов в URL-адресах конечной точки</span><span class="sxs-lookup"><span data-stu-id="3d5b0-131">Add or replace file name extensions in endpoint URLs</span></span>
<span data-ttu-id="3d5b0-132"><a name="bk_FileExtensions"> </a></span><span class="sxs-lookup"><span data-stu-id="3d5b0-132"><a name="bk_FileExtensions"> </a></span></span>

<span data-ttu-id="3d5b0-133">Доступ к службе автообнаружения можно получить с помощью веб-службы автообнаружения SOAP или веб-службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-133">You can access the Autodiscover service by using either the SOAP Autodiscover web service or the POX Autodiscover web service.</span></span> <span data-ttu-id="3d5b0-134">Каждая служба использует похожие URL-адреса конечной точки, единственное отличие от расширения имени файла.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-134">Each service uses similar endpoint URLs, with the only difference being the file name extension.</span></span> <span data-ttu-id="3d5b0-135">Веб-служба автообнаружения SOAP использует расширение имени файла SVC, а веб-служба автообнаружения POX использует расширение имени файла ". XML".</span><span class="sxs-lookup"><span data-stu-id="3d5b0-135">The SOAP Autodiscover web service uses the ".svc" file name extension, and the POX Autodiscover web service uses the ".xml" file name extension.</span></span>
  
<span data-ttu-id="3d5b0-136">По умолчанию URL-адреса конечных точек автообнаружения, возвращенные из поиска SCP, являются URL-адресами POX.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-136">By default, the Autodiscover endpoint URLs returned from an SCP lookup are POX URLs.</span></span> <span data-ttu-id="3d5b0-137">Однако при использовании автообнаружения SOAP можно просто изменить расширение имени файла с ". XML" на SVC и попробовать SOAP-запрос.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-137">However, if you are using SOAP Autodiscover, you can simply change the file name extension from ".xml" to ".svc" and try a SOAP request.</span></span>
  
<span data-ttu-id="3d5b0-138">Для URL-адресов конечной точки автообнаружения расширение файла не указывается.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-138">For the derived Autodiscover endpoint URLs, the file extension is omitted.</span></span> <span data-ttu-id="3d5b0-139">Добавьте соответствующее расширение файла для веб-службы автообнаружения, которую вы используете, прежде чем пытаться использовать URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-139">Add the appropriate file extension for the Autodiscover web service you are using prior to trying the URL.</span></span>
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a><span data-ttu-id="3d5b0-140">Пример: Создание списка конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3d5b0-140">Example: Generating a list of Autodiscover endpoints</span></span>
<span data-ttu-id="3d5b0-141"><a name="bk_Example"> </a></span><span class="sxs-lookup"><span data-stu-id="3d5b0-141"><a name="bk_Example"> </a></span></span>

<span data-ttu-id="3d5b0-142">Давайте рассмотрим пример.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-142">Let's take a look at an example.</span></span> <span data-ttu-id="3d5b0-143">Ольга Даниелс (Sadie.Daniels@contoso.com) в первый раз использует приложение веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="3d5b0-143">Sadie Daniels (Sadie.Daniels@contoso.com) is using an Exchange Web Services (EWS) application for the first time.</span></span> <span data-ttu-id="3d5b0-144">Приложение использует службу автообнаружения для настройки.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-144">The application uses Autodiscover to configure itself.</span></span> <span data-ttu-id="3d5b0-145">Компьютер Ольга присоединен к домену contoso.com и находится на сайте Redmond Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-145">Sadie's computer is joined to the contoso.com domain and is in the Redmond Active Directory site.</span></span> <span data-ttu-id="3d5b0-146">Приложение создает список конечных точек автообнаружения, показанный на рисунке 1.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-146">The application generates the list of Autodiscover endpoints shown in Figure 1.</span></span>
  
<span data-ttu-id="3d5b0-147">**Рисунок 1: пример списка конечных точек автообнаружения**</span><span class="sxs-lookup"><span data-stu-id="3d5b0-147">**Figure 1: Sample list of Autodiscover endpoints**</span></span>

![Пример списка конечных точек службы автообнаружения, где конечные точки, полученные с помощью поиска SCP, имеют более высокий приоритет, чем производные конечные точки.](media/Ex15_Autodiscover_GenerateList_Example.png)
  
<span data-ttu-id="3d5b0-149">В этом примере приложение EWS предпочитает веб-службу автообнаружения SOAP, поэтому перед отправкой SOAP-запросов в службу обнаружения имен файлов для точки подключения к этой службе изменяется расширение имени файла.</span><span class="sxs-lookup"><span data-stu-id="3d5b0-149">The EWS application in this example prefers the SOAP Autodiscover web service, so it changes the file name extension for the SCP results to ".svc" before sending SOAP requests to them.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="3d5b0-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3d5b0-150">Next steps</span></span>
<span data-ttu-id="3d5b0-151"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="3d5b0-151"><a name="bk_NextSteps"> </a></span></span>

<span data-ttu-id="3d5b0-152">После создания списка конечных точек автообнаружения попробуйте [отправить запросы на эти конечные точки](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="3d5b0-152">After you generate a list of Autodiscover endpoints, try them by [sending requests to those endpoints](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="3d5b0-153">См. также</span><span class="sxs-lookup"><span data-stu-id="3d5b0-153">See also</span></span>


- [<span data-ttu-id="3d5b0-154">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d5b0-154">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="3d5b0-155">Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d5b0-155">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="3d5b0-156">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3d5b0-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    

