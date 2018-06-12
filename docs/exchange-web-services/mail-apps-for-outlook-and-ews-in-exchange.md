---
title: Приложения электронной почты для Outlook и EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Найдите сведения о почтовых приложений для Outlook и работы с веб-служб Exchange в Exchange.
ms.openlocfilehash: 2f44045d80a74ed6a835604d516949ca3bc27379
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761146"
---
# <a name="mail-apps-for-outlook-and-ews-in-exchange"></a><span data-ttu-id="4524f-103">Приложения электронной почты для Outlook и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4524f-103">Mail apps for Outlook and EWS in Exchange</span></span>

<span data-ttu-id="4524f-104">Найдите сведения о почтовых приложений для Outlook и работы с веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4524f-104">Find information about mail apps for Outlook and how they work with EWS in Exchange.</span></span>
  
<span data-ttu-id="4524f-105">Почтовые приложения для Outlook укажите единый интерфейс и модель программирования, которая использует веб-стандартов для создания пользовательского интерфейса для пользователей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4524f-105">Mail apps for Outlook provide a single interface and programming model that uses web standards to enable you to create a custom experience for your email users.</span></span> <span data-ttu-id="4524f-106">Можно создать почтовых приложений, отображающих сведения о контекстной или полезны в кадре HTML5, размещенных в Outlook; к примеру почтовое приложение позволяет показывать карты Bing с адресом выделен, если сообщение электронной почты содержит адрес.</span><span class="sxs-lookup"><span data-stu-id="4524f-106">You can create mail apps that display contextual or helpful information in an HTML5 frame hosted in Outlook; for example, a mail app can show a Bing map with an address highlighted when an email message contains an address.</span></span> <span data-ttu-id="4524f-107">Или при создании сообщения в почтового приложения можно отобразить дополнительные сведения о получателе и Вставить стандартный приветствие в сообщение электронной почты нажатием кнопки.</span><span class="sxs-lookup"><span data-stu-id="4524f-107">Or when a user is composing a message, a mail app can show additional information about the recipient, and insert a standard greeting into the email at the touch of a button.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4524f-108">В этой статье "Outlook" означает расширенный клиент Outlook, Outlook RT, Outlook Web App и OWA для устройств.</span><span class="sxs-lookup"><span data-stu-id="4524f-108">"Outlook" in this article refers to the Outlook rich client, Outlook RT, Outlook Web App, and OWA for Devices.</span></span> 
  
<span data-ttu-id="4524f-109">Интерфейс приложения почты является частью JavaScript API для Office.</span><span class="sxs-lookup"><span data-stu-id="4524f-109">The mail apps interface is part of the JavaScript API for Office.</span></span> <span data-ttu-id="4524f-110">API можно использовать для доступа к сведениям в Exchange для включения вашего почтового приложения:</span><span class="sxs-lookup"><span data-stu-id="4524f-110">You can use the API to access information in Exchange to enable your mail app to:</span></span>
  
- <span data-ttu-id="4524f-111">[Распознавать сущности](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), как адреса, номера телефонов, предложения задач или предложения о собраниях в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4524f-111">[Recognize entities](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), like addresses, phone numbers, task suggestions, or meeting suggestions in an email.</span></span> 
    
- <span data-ttu-id="4524f-112">Открытие и отображение существующих [сообщений](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) и [встреч](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) в отдельном представлении, чтобы пользователи могут перекрестная ссылка сведения в одно или несколько сообщений.</span><span class="sxs-lookup"><span data-stu-id="4524f-112">Open and display existing [messages](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) and [appointments](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) in a separate view so that users can cross-reference information in one or more messages.</span></span> 
    
- <span data-ttu-id="4524f-113">[Запросы на выполнение веб-служб Exchange](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) на сервере Exchange, на котором размещен почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="4524f-113">[Make EWS requests](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) to the Exchange server that hosts the user's mailbox.</span></span> <span data-ttu-id="4524f-114">Почтовое приложение например, список можно получить папок, чтобы пользователя можно выбрать один для хранения сообщения или отображение всех элементов в беседе или пометить как нежелательные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4524f-114">A mail app can, for example, get a list of folders so that the user can choose one to store the message, or show all the items in a conversation, or mark an email message as junk.</span></span> 
    
- <span data-ttu-id="4524f-115">[Получить маркер](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) для уникальной идентификации учетной записи электронной почты для включения единого входа службе сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="4524f-115">[Get a token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) to uniquely identify an email account to enable single sign on on a third-party service.</span></span> 
    
- <span data-ttu-id="4524f-116">[Получить маркер](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) , позволяющий сторонних служб мог выполнять запросы EWS от имени пользователя, например, чтобы извлечь вложения из элемента или для получения элемента с сервера Exchange server для дальнейшей обработки.</span><span class="sxs-lookup"><span data-stu-id="4524f-116">[Get a token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) that enables a third-party service to make EWS requests on behalf of the user, for example, to extract the attachments from an item, or to get an item from the Exchange server for further processing.</span></span> 
    
<span data-ttu-id="4524f-117">Почтовые приложения можно использовать для настройки взаимодействия Outlook Web App для пользователей; Если необходимо настроить «внешний вид и функции» из Outlook Web App, отображается в этих статьях на сайте TechNet:</span><span class="sxs-lookup"><span data-stu-id="4524f-117">You can use mail apps to customize the Outlook Web App experience for your users; if, however, you want to customize the "look and feel" of Outlook Web App, see these articles on TechNet:</span></span>
  
- [<span data-ttu-id="4524f-118">Создание темы для Outlook Web App</span><span class="sxs-lookup"><span data-stu-id="4524f-118">Create a theme for Outlook Web App</span></span>](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="4524f-119">Настройка Outlook Web App входа, выбора языка и страницы ошибок</span><span class="sxs-lookup"><span data-stu-id="4524f-119">Customize the Outlook Web App sign-in, language selection, and error pages</span></span>](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)
    
<span data-ttu-id="4524f-120">Вашей организации можно установить почтовых приложений на внутреннем сервере для ограничения доступа к авторизованные пользователи, или вы разработчиков приложений и других почтовых приложений можно размещать почтовых приложений в [Магазине Office](http://office.microsoft.com/store/) для продажи для всех.</span><span class="sxs-lookup"><span data-stu-id="4524f-120">Your organization can install mail apps on an internal server to limit access to authorized users, or you and other mail app developers can put mail apps on the [Office Store](http://office.microsoft.com/store/) for sale to the general public.</span></span> <span data-ttu-id="4524f-121">Любой пользователь, запущен Outlook можно загрузить, установить и использовать почтовые приложения из магазина.</span><span class="sxs-lookup"><span data-stu-id="4524f-121">Anyone who is running Outlook can download, install, and use mail apps from the marketplace.</span></span> 
  
<span data-ttu-id="4524f-122">Если вы хотите узнать больше о создании почтовых приложений, извлечь [почтовых приложений для Outlook документации](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx) или пример [выполнения запроса веб-служб Exchange](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .</span><span class="sxs-lookup"><span data-stu-id="4524f-122">If you want to learn more about creating mail apps, check out the [mail apps for Outlook documentation](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx) or the [Make an EWS request](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) sample.</span></span> 
  
## <a name="ews-and-mail-apps-for-outlook"></a><span data-ttu-id="4524f-123">Веб-служб Exchange и почтового приложения для Outlook</span><span class="sxs-lookup"><span data-stu-id="4524f-123">EWS and mail apps for Outlook</span></span>

<span data-ttu-id="4524f-124">Можно использовать подмножества операций веб-служб Exchange на сервере Exchange, на котором размещается учетная запись, запускающая почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="4524f-124">You can use a subset of EWS operations on the Exchange server that hosts the account that runs a mail app.</span></span>
  
<span data-ttu-id="4524f-125">Функция [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) позволяет выполнять запросы EWS из почтового приложения на сервере, на котором размещен почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="4524f-125">The [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) function enables you to make EWS requests from your mail app back to the server that hosts the user's mailbox.</span></span> <span data-ttu-id="4524f-126">Создайте конверте SOAP и XML-запрос и вызовы функций **makeEwsRequestAsync** веб-служб Exchange с помощью маркера проверки подлинности, который идентифицирует почтовый ящик и почтовые приложения, делающего запрос.</span><span class="sxs-lookup"><span data-stu-id="4524f-126">You create the SOAP envelope and XML request, and the **makeEwsRequestAsync** function calls EWS with an authentication token that identifies the mailbox and mail app that is making the request.</span></span> <span data-ttu-id="4524f-127">Для улучшения защиты почтового ящика пользователя, Exchange server будет отклонять все запросы, полученные из почтового приложения или из почтового ящика, который не находится на сервере.</span><span class="sxs-lookup"><span data-stu-id="4524f-127">To help secure the user's mailbox, the Exchange server will reject any requests that do not come from the mail app or from a mailbox that is not hosted on the server.</span></span> 
  
<span data-ttu-id="4524f-128">Как и другие приложения почтовое приложение должно разрешения для работы.</span><span class="sxs-lookup"><span data-stu-id="4524f-128">Like any other application, a mail app needs permissions to work.</span></span> <span data-ttu-id="4524f-129">Администратор должен:</span><span class="sxs-lookup"><span data-stu-id="4524f-129">Your administrator needs to:</span></span>
  
- <span data-ttu-id="4524f-130">[Веб-служб Exchange предоставление доступа](controlling-client-application-access-to-ews-in-exchange.md) к пользователю почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="4524f-130">[Grant EWS access](controlling-client-application-access-to-ews-in-exchange.md) to the mail apps user.</span></span> 
    
- <span data-ttu-id="4524f-131">[Набор параметра «OAuthAuthentication» имеет значение true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) в каталоге Client Access Server EWS.</span><span class="sxs-lookup"><span data-stu-id="4524f-131">[Set "OAuthAuthentication" to true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) on the Client Access Server EWS directory.</span></span> 
    
<span data-ttu-id="4524f-132">Необходимо также убедитесь в том, что ваше приложение запрашивает разрешение чтение и запись почтового ящика в приложениях для Office [модель разрешений](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4524f-132">You also need to make sure that your app requests the read/write mailbox permission in the apps for Office [permission model](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="4524f-133">После выполнения этих шагов подмножество папки и операции EWS элемента доступны для почтового приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="4524f-133">When these steps are complete, a subset of folder and item EWS operations are available for the mail app to use.</span></span> 
  
<span data-ttu-id="4524f-134">**В таблице 1. Можно использовать операции папок и элементов веб-служб Exchange, почтовые приложения**</span><span class="sxs-lookup"><span data-stu-id="4524f-134">**Table 1. EWS folder and item operations that mail apps can use**</span></span>

|<span data-ttu-id="4524f-135">**Папка операций**</span><span class="sxs-lookup"><span data-stu-id="4524f-135">**Folder operations**</span></span>|<span data-ttu-id="4524f-136">**Операции с элементами**</span><span class="sxs-lookup"><span data-stu-id="4524f-136">**Item operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4524f-137">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-137">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-138">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-138">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-139">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-139">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-140">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4524f-140">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[<span data-ttu-id="4524f-141">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-141">CopyItem operation</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-142">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-142">CreateItem operation</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-143">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-143">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-144">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-144">FindConversation operation</span></span>](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-145">GetConversationItems operation</span><span class="sxs-lookup"><span data-stu-id="4524f-145">GetConversationItems operation</span></span>](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-146">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-146">GetItem operation</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-147">MarkAsJunk Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-147">MarkAsJunk operation</span></span>](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-148">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-148">MoveItem operation</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-149">SendItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-149">SendItem operation</span></span>](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [<span data-ttu-id="4524f-150">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="4524f-150">UpdateItem operation</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
   
### <a name="service-callback-tokens"></a><span data-ttu-id="4524f-151">Служба маркеров обратного вызова</span><span class="sxs-lookup"><span data-stu-id="4524f-151">Service callback tokens</span></span>

<span data-ttu-id="4524f-152">Служба маркеров обратного вызова включите почтовые приложения передать маркер доступа к службе сторонних производителей, чтобы службы можно выполнять запросы EWS на сервере Exchange, на котором размещен почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="4524f-152">Service callback tokens enable mail apps to pass an access token to a third-party service so that the service can make EWS requests to the Exchange server that hosts the mailbox.</span></span> <span data-ttu-id="4524f-153">Например почтового приложения можно передать маркер обратного вызова службы сторонних служб вместе со списком идентификаторы вложений для изображений, подключенного к сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4524f-153">For example, a mail app can pass a service callback token to a third-party service along with a list of attachment IDs for pictures attached to an email.</span></span> <span data-ttu-id="4524f-154">Служба будет использовать идентификаторы вложений и маркер обратного вызова для выполнения запроса EWS для пользователя Exchange server для получения вложенных рисунков.</span><span class="sxs-lookup"><span data-stu-id="4524f-154">The service can then use the attachment IDs and the callback token to make an EWS request to the user's Exchange server to get the attached pictures.</span></span> <span data-ttu-id="4524f-155">Также почтовые приложения могут использовать маркер обратного вызова службы со списком идентификаторов элементов для получения элементов электронной почты и встречи с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="4524f-155">Mail apps can also use the service callback token with a list of item IDs to get email and appointment items from the Exchange server.</span></span>
  
<span data-ttu-id="4524f-156">Маркер обратного вызова службы — это непрозрачный маркера, который подключает службы сторонних производителей для запроса веб-служб Exchange в заголовок проверки подлинности носителя.</span><span class="sxs-lookup"><span data-stu-id="4524f-156">The service callback token is an opaque token that the third-party service attaches to the EWS request in a bearer authentication header.</span></span> <span data-ttu-id="4524f-157">Маркер определяет почтового приложения и почтовых ящиков для улучшения защиты запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4524f-157">The token identifies the mail app and the mailbox to help secure the EWS request.</span></span> <span data-ttu-id="4524f-158">Чтобы узнать, как использовать службы маркеров обратного вызова, обратитесь к разделу [почтовые приложения для Outlook: получение вложений с сервера Exchange,](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) образца.</span><span class="sxs-lookup"><span data-stu-id="4524f-158">To learn how to use service callback tokens, see the [Mail apps for Outlook: Get attachments from an Exchange server](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) sample.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4524f-159">См. также</span><span class="sxs-lookup"><span data-stu-id="4524f-159">See also</span></span>


- [<span data-ttu-id="4524f-160">Управление доступом к клиентского приложения для веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4524f-160">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)
    
- [<span data-ttu-id="4524f-161">Метод Mailbox.makeEwsRequestAsync (API JavaScript для Office)</span><span class="sxs-lookup"><span data-stu-id="4524f-161">Mailbox.makeEwsRequestAsync method (JavaScript API for Office)</span></span>](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)
    
- [<span data-ttu-id="4524f-162">Надстройки Outlook</span><span class="sxs-lookup"><span data-stu-id="4524f-162">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    
- [<span data-ttu-id="4524f-163">Метод Mailbox.getUserIdentityTokenAsync (API JavaScript для Office)</span><span class="sxs-lookup"><span data-stu-id="4524f-163">Mailbox.getUserIdentityTokenAsync method (JavaScript API for Office)</span></span>](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)
    
- [<span data-ttu-id="4524f-164">Проверка подлинности надстройки Outlook с помощью маркеров удостоверений Exchange</span><span class="sxs-lookup"><span data-stu-id="4524f-164">Authenticate an Outlook add-in by using Exchange identity tokens</span></span>](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)
    
- [<span data-ttu-id="4524f-165">Общие сведения о разрешениях для надстроек Outlook</span><span class="sxs-lookup"><span data-stu-id="4524f-165">Understanding Outlook add-in permissions</span></span>](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx)
    
- [<span data-ttu-id="4524f-166">SET-WebServicesVirtualDirectory</span><span class="sxs-lookup"><span data-stu-id="4524f-166">Set-WebServicesVirtualDirectory</span></span>](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="4524f-167">Почтовые приложения для Outlook: для выполнения запроса EWS</span><span class="sxs-lookup"><span data-stu-id="4524f-167">Mail apps for Outlook: Make an EWS request</span></span>](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)
    
- [<span data-ttu-id="4524f-168">Почтовые приложения для Outlook: Использование маркера удостоверения клиента</span><span class="sxs-lookup"><span data-stu-id="4524f-168">Mail apps for Outlook: Use a client identity token</span></span>](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)
    
- [<span data-ttu-id="4524f-169">Почтовые приложения для Outlook: получение вложений с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="4524f-169">Mail apps for Outlook: Get attachments from an Exchange server</span></span>](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
    
