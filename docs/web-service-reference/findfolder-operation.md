---
title: FindFolder Operation
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
description: Операция FindFolder использует веб-служб Exchange, чтобы найти вложенные папки заданной папки и возвращает набор свойств, описывающих вложенные папки.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762560"
---
# <a name="findfolder-operation"></a><span data-ttu-id="ea06b-103">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="ea06b-103">FindFolder operation</span></span>

<span data-ttu-id="ea06b-104">Операция **FindFolder** использует веб-служб Exchange, чтобы найти вложенные папки заданной папки и возвращает набор свойств, описывающих вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="ea06b-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ea06b-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="ea06b-105">Remarks</span></span>

<span data-ttu-id="ea06b-106">FindFolder возвращает только первые 512 байт поддерживающего потоковую передачу свойства.</span><span class="sxs-lookup"><span data-stu-id="ea06b-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="ea06b-107">Для Юникод возвращает первые 255 символов, используя строку Юникода символом null.</span><span class="sxs-lookup"><span data-stu-id="ea06b-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="ea06b-108">Запросы глубокий обзор не может быть выполнена для общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="ea06b-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="ea06b-109">Ограничения разрешены и следует использовать только свойства папки, но не свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="ea06b-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="ea06b-110">Функциональные возможности сортировки для ответов **FindFolder** недоступен.</span><span class="sxs-lookup"><span data-stu-id="ea06b-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="ea06b-111">Сгруппированные запросы недоступны для **FindFolder** запросов.</span><span class="sxs-lookup"><span data-stu-id="ea06b-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="ea06b-112">**Примечание** Операция **FindFolder** также используется для управляемых папок поиска.</span><span class="sxs-lookup"><span data-stu-id="ea06b-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="ea06b-113">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="ea06b-113">SOAP Headers</span></span>

<span data-ttu-id="ea06b-114">Операция **FindFolder** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ea06b-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ea06b-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="ea06b-115">**Header**</span></span>|<span data-ttu-id="ea06b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea06b-116">**Element**</span></span>|<span data-ttu-id="ea06b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea06b-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ea06b-118">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="ea06b-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="ea06b-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ea06b-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ea06b-120">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="ea06b-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ea06b-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ea06b-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="ea06b-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ea06b-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ea06b-123">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="ea06b-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ea06b-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ea06b-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ea06b-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ea06b-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ea06b-126">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="ea06b-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ea06b-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ea06b-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ea06b-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ea06b-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ea06b-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="ea06b-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="ea06b-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ea06b-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="ea06b-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ea06b-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="ea06b-132">Определяет часовой пояс, который будет использоваться для всех ответов с сервера.</span><span class="sxs-lookup"><span data-stu-id="ea06b-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="ea06b-133">Пример запроса FindFolder</span><span class="sxs-lookup"><span data-stu-id="ea06b-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ea06b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ea06b-134">Description</span></span>

<span data-ttu-id="ea06b-135">Пример запроса **FindFolder** показано, как для формирования запроса, чтобы найти все папки, расположенной в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="ea06b-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ea06b-136">Программа</span><span class="sxs-lookup"><span data-stu-id="ea06b-136">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="ea06b-137">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ea06b-137">Comments</span></span>

<span data-ttu-id="ea06b-138">Используется значение по умолчанию для [BaseShape](baseshape.md), ответ возвращает имя папки, идентификатор папки количество вложенных папок, количество вложенных папок в папке и количество непрочитанных элементов.</span><span class="sxs-lookup"><span data-stu-id="ea06b-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="ea06b-139">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="ea06b-139">Request elements</span></span>

<span data-ttu-id="ea06b-140">В этом запросе **FindFolder** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ea06b-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="ea06b-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ea06b-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="ea06b-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="ea06b-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="ea06b-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ea06b-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ea06b-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="ea06b-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="ea06b-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ea06b-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="ea06b-146">Дополнительные элементы запроса **FindFolder** см.</span><span class="sxs-lookup"><span data-stu-id="ea06b-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="ea06b-147">Пример ответа FindFolder</span><span class="sxs-lookup"><span data-stu-id="ea06b-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="ea06b-148">Описание</span><span class="sxs-lookup"><span data-stu-id="ea06b-148">Description</span></span>

<span data-ttu-id="ea06b-149">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="ea06b-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="ea06b-150">Ответ содержит элементы, которые возвращаются при используется значение по умолчанию для [BaseShape](baseshape.md) .</span><span class="sxs-lookup"><span data-stu-id="ea06b-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ea06b-151">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ea06b-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ea06b-152">Программа</span><span class="sxs-lookup"><span data-stu-id="ea06b-152">Code</span></span>

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

### <a name="response-elements"></a><span data-ttu-id="ea06b-153">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="ea06b-153">Response elements</span></span>

<span data-ttu-id="ea06b-154">Свойства, возвращаемого в ответе определяются [BaseShape](baseshape.md) и [AdditionalProperties](additionalproperties.md) , если они используются.</span><span class="sxs-lookup"><span data-stu-id="ea06b-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="ea06b-155">Успешного ответа **FindFolder** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ea06b-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ea06b-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ea06b-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ea06b-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ea06b-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ea06b-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ea06b-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ea06b-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea06b-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="ea06b-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ea06b-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ea06b-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ea06b-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="ea06b-162">Папки</span><span class="sxs-lookup"><span data-stu-id="ea06b-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ea06b-163">Folder</span><span class="sxs-lookup"><span data-stu-id="ea06b-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="ea06b-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="ea06b-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="ea06b-165">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="ea06b-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="ea06b-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ea06b-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="ea06b-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ea06b-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="ea06b-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ea06b-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="ea06b-169">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ea06b-169">Comments</span></span>

 <span data-ttu-id="ea06b-170">**FindFolder** ответы на запрос с фигурой ответа **AllProperties** не возвращает [TotalCount](totalcount.md) и элементы [UnreadCount](unreadcount.md) для общедоступных папок поиска.</span><span class="sxs-lookup"><span data-stu-id="ea06b-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="ea06b-171">Пример ответа об ошибке FindFolder</span><span class="sxs-lookup"><span data-stu-id="ea06b-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ea06b-172">Описание</span><span class="sxs-lookup"><span data-stu-id="ea06b-172">Description</span></span>

<span data-ttu-id="ea06b-173">В следующем примере тело SOAP показано возврату ошибки, возникающих при выполнении поиска для папки, который идентифицируется по идентификатору неверно сформированные папки.</span><span class="sxs-lookup"><span data-stu-id="ea06b-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="ea06b-174">Программа</span><span class="sxs-lookup"><span data-stu-id="ea06b-174">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="ea06b-175">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="ea06b-175">Error response elements</span></span>

<span data-ttu-id="ea06b-176">Отклик **FindFolder** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ea06b-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ea06b-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ea06b-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ea06b-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ea06b-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ea06b-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="ea06b-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ea06b-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ea06b-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ea06b-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ea06b-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="ea06b-182">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="ea06b-182">Additional Information</span></span>

- <span data-ttu-id="ea06b-183">Элемент [DisplayName (string)](displayname-string.md) папки всегда включается в форме по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ea06b-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="ea06b-184">Элемент [UnreadCount](unreadcount.md) входит в папках задач и заметок.</span><span class="sxs-lookup"><span data-stu-id="ea06b-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="ea06b-185">Используйте значение **PropertyTag** 0x672D с типом свойства **целого числа со знаком** для определения управляемых папок с помощью элемента [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="ea06b-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="ea06b-186">См. также</span><span class="sxs-lookup"><span data-stu-id="ea06b-186">See also</span></span>



[<span data-ttu-id="ea06b-187">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="ea06b-187">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

