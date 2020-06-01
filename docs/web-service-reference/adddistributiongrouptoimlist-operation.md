---
title: Операция AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Поиск сведений о AddDistributionGroupToImListной операции EWS.
ms.openlocfilehash: e68e21b6994af5773f5cf991d55129e1db3367ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463694"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="cd7c4-103">Операция AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="cd7c4-104">Поиск сведений о **AddDistributionGroupToImListной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="cd7c4-105">**AddDistributionGroupToImList** веб-служб Exchange (EWS) добавляет группу рассылки в список обмена мгновенными сообщениями в едином хранилище контактов.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="cd7c4-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="cd7c4-107">Использование операции AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="cd7c4-108">Операция **AddDistributionGroupToImList** принимает один аргумент, определяющий группу рассылки, которую необходимо добавить в список мгновенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="cd7c4-109">Эта операция не создает группу рассылки; Группа рассылки уже должна быть создана.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="cd7c4-110">Эта операция может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="cd7c4-111">**Таблица 1. Заголовки SOAP операции AddDistributionGroupToImList**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="cd7c4-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-112">**Header name**</span></span>|<span data-ttu-id="cd7c4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-113">**Element**</span></span>|<span data-ttu-id="cd7c4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cd7c4-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cd7c4-116">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="cd7c4-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cd7c4-117">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cd7c4-118">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd7c4-119">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cd7c4-120">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="cd7c4-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cd7c4-121">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cd7c4-122">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd7c4-123">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cd7c4-124">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="cd7c4-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cd7c4-125">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cd7c4-126">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd7c4-127">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="cd7c4-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cd7c4-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="cd7c4-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cd7c4-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cd7c4-130">Это относится к отклику.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="cd7c4-131">Пример запроса операции AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="cd7c4-132">В следующем примере запроса операции **AddDistributionGroupToImList** показано, как добавить группу рассылки в список мгновенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cd7c4-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd7c4-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cd7c4-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="cd7c4-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="cd7c4-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="cd7c4-136">Успешный отклик операции AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="cd7c4-137">В следующем примере показан успешный ответ на запрос операции **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="cd7c4-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="cd7c4-138">Успешный ответ содержит отображаемое имя группы рассылки, класс хранилища Exchange для группы рассылки и идентификатор EWS новой группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cd7c4-139">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd7c4-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cd7c4-140">адддистрибутионграуптоимлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="cd7c4-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="cd7c4-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="cd7c4-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cd7c4-142">Группа</span><span class="sxs-lookup"><span data-stu-id="cd7c4-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="cd7c4-143">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="cd7c4-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="cd7c4-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="cd7c4-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="cd7c4-145">ексчанжестореид</span><span class="sxs-lookup"><span data-stu-id="cd7c4-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="cd7c4-146">Ответ об ошибке Ерроринвалидимдистрибутионграупсмтпаддресс операции AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="cd7c4-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="cd7c4-147">В следующем примере показан ответ об ошибке для запроса операции **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="cd7c4-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="cd7c4-148">При попытке добавить группу рассылки, которая не существует в хранилище Exchange, возникает следующий ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd7c4-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cd7c4-149">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd7c4-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cd7c4-150">адддистрибутионграуптоимлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="cd7c4-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="cd7c4-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="cd7c4-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cd7c4-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="cd7c4-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="cd7c4-153">См. также</span><span class="sxs-lookup"><span data-stu-id="cd7c4-153">See also</span></span>

- [<span data-ttu-id="cd7c4-154">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="cd7c4-154">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="cd7c4-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cd7c4-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="cd7c4-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="cd7c4-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

