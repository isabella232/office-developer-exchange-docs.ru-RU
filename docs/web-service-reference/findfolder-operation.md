---
title: Операция FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: Операция FindFolder использует веб-службы Exchange для поиска вложенных папок в определенной папке и возвращает набор свойств, описывающих набор вложенных папок.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762560"
---
# <a name="findfolder-operation"></a><span data-ttu-id="b84c6-103">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="b84c6-103">FindFolder operation</span></span>

<span data-ttu-id="b84c6-104">Операция **FindFolder** использует веб-службы Exchange для поиска вложенных папок в определенной папке и возвращает набор свойств, описывающих набор вложенных папок.</span><span class="sxs-lookup"><span data-stu-id="b84c6-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b84c6-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="b84c6-105">Remarks</span></span>

<span data-ttu-id="b84c6-106">FindFolder возвращает только первые 512 байт любого потокового свойства.</span><span class="sxs-lookup"><span data-stu-id="b84c6-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="b84c6-107">Для Юникода он возвращает первые 255 символов, используя строку Юникода с завершающим нулем.</span><span class="sxs-lookup"><span data-stu-id="b84c6-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="b84c6-108">Запросы с глубоким обходом не могут выполняться в общедоступных папках.</span><span class="sxs-lookup"><span data-stu-id="b84c6-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="b84c6-109">Ограничения разрешены и должны использовать только свойства папки, а не свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="b84c6-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="b84c6-110">Функция сортировки недоступна для ответов **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="b84c6-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="b84c6-111">Сгруппированные запросы недоступны для запросов **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="b84c6-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="b84c6-112">**Note (Примечание** ) Операция **FindFolder** также используется для поиска управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="b84c6-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="b84c6-113">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="b84c6-113">SOAP Headers</span></span>

<span data-ttu-id="b84c6-114">В операции **FindFolder** могут использоваться заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b84c6-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="b84c6-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="b84c6-115">**Header**</span></span>|<span data-ttu-id="b84c6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b84c6-116">**Element**</span></span>|<span data-ttu-id="b84c6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b84c6-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b84c6-118">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="b84c6-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="b84c6-119">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="b84c6-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b84c6-120">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="b84c6-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="b84c6-121">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b84c6-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="b84c6-122">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b84c6-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b84c6-123">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b84c6-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="b84c6-124">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="b84c6-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="b84c6-125">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b84c6-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b84c6-126">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b84c6-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="b84c6-127">серверверсион</span><span class="sxs-lookup"><span data-stu-id="b84c6-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="b84c6-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b84c6-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b84c6-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b84c6-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="b84c6-130">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="b84c6-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="b84c6-131">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="b84c6-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="b84c6-132">Определяет часовой пояс, который будет использоваться для всех ответов сервера.</span><span class="sxs-lookup"><span data-stu-id="b84c6-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="b84c6-133">Пример запроса FindFolder</span><span class="sxs-lookup"><span data-stu-id="b84c6-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="b84c6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b84c6-134">Description</span></span>

<span data-ttu-id="b84c6-135">В следующем примере запроса **FindFolder** показано, как сформировать запрос на поиск всех папок, расположенных в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="b84c6-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b84c6-136">Код</span><span class="sxs-lookup"><span data-stu-id="b84c6-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b84c6-137">Comments</span><span class="sxs-lookup"><span data-stu-id="b84c6-137">Comments</span></span>

<span data-ttu-id="b84c6-138">При использовании значения по умолчанию для [басешапе](baseshape.md), ответ возвращает имя папки, идентификатор папки, количество вложенных папок, количество вложенных папок в папке и количество непрочитанных элементов.</span><span class="sxs-lookup"><span data-stu-id="b84c6-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="b84c6-139">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="b84c6-139">Request elements</span></span>

<span data-ttu-id="b84c6-140">Этот запрос **FindFolder** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b84c6-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="b84c6-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="b84c6-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="b84c6-142">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="b84c6-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="b84c6-143">басешапе</span><span class="sxs-lookup"><span data-stu-id="b84c6-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="b84c6-144">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="b84c6-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="b84c6-145">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="b84c6-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="b84c6-146">Дополнительные элементы запроса **FindFolder** приведены в схеме.</span><span class="sxs-lookup"><span data-stu-id="b84c6-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="b84c6-147">Пример отклика FindFolder</span><span class="sxs-lookup"><span data-stu-id="b84c6-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="b84c6-148">Описание</span><span class="sxs-lookup"><span data-stu-id="b84c6-148">Description</span></span>

<span data-ttu-id="b84c6-149">В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="b84c6-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="b84c6-150">Ответ содержит элементы, которые возвращаются при использовании значения по умолчанию для [басешапе](baseshape.md) .</span><span class="sxs-lookup"><span data-stu-id="b84c6-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b84c6-151">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b84c6-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b84c6-152">Код</span><span class="sxs-lookup"><span data-stu-id="b84c6-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="b84c6-153">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="b84c6-153">Response elements</span></span>

<span data-ttu-id="b84c6-154">Свойства, возвращаемые в ответе, определяются [басешапе](baseshape.md) и [аддитионалпропертиес](additionalproperties.md) , если они используются.</span><span class="sxs-lookup"><span data-stu-id="b84c6-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="b84c6-155">Успешный отклик **FindFolder** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b84c6-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="b84c6-156">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b84c6-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b84c6-157">финдфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="b84c6-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="b84c6-158">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b84c6-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b84c6-159">финдфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b84c6-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="b84c6-160">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b84c6-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b84c6-161">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="b84c6-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="b84c6-162">Folders</span><span class="sxs-lookup"><span data-stu-id="b84c6-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b84c6-163">Folder</span><span class="sxs-lookup"><span data-stu-id="b84c6-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="b84c6-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="b84c6-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="b84c6-165">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="b84c6-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b84c6-166">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="b84c6-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="b84c6-167">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="b84c6-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="b84c6-168">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="b84c6-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="b84c6-169">Comments</span><span class="sxs-lookup"><span data-stu-id="b84c6-169">Comments</span></span>

 <span data-ttu-id="b84c6-170">Элементы **FindFolder** отклика на запрос с фигурой ответа **аллпропертиес** не возвращают элементы [тоталкаунт](totalcount.md) и [унреадкаунт](unreadcount.md) для поиска в общедоступных папках.</span><span class="sxs-lookup"><span data-stu-id="b84c6-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="b84c6-171">Пример отклика на сообщение об ошибке FindFolder</span><span class="sxs-lookup"><span data-stu-id="b84c6-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b84c6-172">Описание</span><span class="sxs-lookup"><span data-stu-id="b84c6-172">Description</span></span>

<span data-ttu-id="b84c6-173">В следующем примере сообщения SOAP показан ответ об ошибке, возникающий при поиске папки, которая определяется с помощью искаженного идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="b84c6-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="b84c6-174">Код</span><span class="sxs-lookup"><span data-stu-id="b84c6-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="b84c6-175">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="b84c6-175">Error response elements</span></span>

<span data-ttu-id="b84c6-176">Ответ об ошибке **FindFolder** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b84c6-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="b84c6-177">финдфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="b84c6-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="b84c6-178">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b84c6-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b84c6-179">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b84c6-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b84c6-180">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b84c6-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b84c6-181">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b84c6-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="b84c6-182">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="b84c6-182">Additional Information</span></span>

- <span data-ttu-id="b84c6-183">Элемент [DisplayName (строка)](displayname-string.md) папки всегда включается в фигуру по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b84c6-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="b84c6-184">Элемент [унреадкаунт](unreadcount.md) включается в папки "задачи" и "Заметки".</span><span class="sxs-lookup"><span data-stu-id="b84c6-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="b84c6-185">Используйте значение **пропертитаг** для 0x672D с типом свойства **Integer** , чтобы определить управляемую папку с помощью элемента [екстендедфиелдури](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="b84c6-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="b84c6-186">См. также</span><span class="sxs-lookup"><span data-stu-id="b84c6-186">See also</span></span>



[<span data-ttu-id="b84c6-187">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="b84c6-187">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

