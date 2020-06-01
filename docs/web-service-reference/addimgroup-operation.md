---
title: Операция AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Поиск сведений о AddImGroupной операции EWS.
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462817"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="cac92-103">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-103">AddImGroup operation</span></span>

<span data-ttu-id="cac92-104">Поиск сведений о **AddImGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="cac92-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="cac92-105">При выполнении операции веб-служб Exchange **AddImGroup** в почтовый ящик добавляется новая группа обмена мгновенными сообщениями (IM).</span><span class="sxs-lookup"><span data-stu-id="cac92-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="cac92-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cac92-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="cac92-107">Использование операции AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="cac92-108">Для операции **AddImGroup** используется только один аргумент Display Name.</span><span class="sxs-lookup"><span data-stu-id="cac92-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="cac92-109">Эта операция возвращает отображаемое имя, тип группы и идентификатор хранилища Exchange для новой группы.</span><span class="sxs-lookup"><span data-stu-id="cac92-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="cac92-110">Операция **AddImGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="cac92-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="cac92-111">**Таблица 1. Заголовки SOAP операции AddImGroup**</span><span class="sxs-lookup"><span data-stu-id="cac92-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="cac92-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="cac92-112">**Header name**</span></span>|<span data-ttu-id="cac92-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cac92-113">**Element**</span></span>|<span data-ttu-id="cac92-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cac92-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cac92-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="cac92-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cac92-116">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="cac92-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cac92-117">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="cac92-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cac92-118">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cac92-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cac92-119">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="cac92-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cac92-120">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="cac92-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cac92-121">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cac92-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cac92-122">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cac92-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cac92-123">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="cac92-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cac92-124">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="cac92-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cac92-125">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="cac92-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cac92-126">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="cac92-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cac92-127">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="cac92-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cac92-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="cac92-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cac92-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="cac92-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cac92-130">Это относится к отклику.</span><span class="sxs-lookup"><span data-stu-id="cac92-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="cac92-131">Пример запроса операции AddImGroup: создание новой группы для обмена мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="cac92-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="cac92-132">В следующем примере запроса операции **AddImGroup** показано, как создать группу обмена мгновенными сообщениями с именем микустомерграуп.</span><span class="sxs-lookup"><span data-stu-id="cac92-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cac92-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cac92-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cac92-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="cac92-135">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="cac92-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="cac92-136">Успешный отклик операции AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="cac92-137">В следующем примере показан успешный ответ на запрос операции **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="cac92-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
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
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cac92-138">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cac92-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cac92-139">аддимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="cac92-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="cac92-140">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="cac92-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cac92-141">Группа</span><span class="sxs-lookup"><span data-stu-id="cac92-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="cac92-142">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="cac92-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="cac92-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="cac92-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="cac92-144">ексчанжестореид</span><span class="sxs-lookup"><span data-stu-id="cac92-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="cac92-145">Ответ об ошибке операции AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-145">AddImGroup operation error response</span></span>

<span data-ttu-id="cac92-146">В следующем примере показан ответ об ошибке для запроса операции **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="cac92-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="cac92-147">Это ответ на запрос, который содержит символ, который не может использоваться в отображаемом имени.</span><span class="sxs-lookup"><span data-stu-id="cac92-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="cac92-148">Обратите внимание, что это неисправность SOAP, а не сообщение об ошибке на основе схемы.</span><span class="sxs-lookup"><span data-stu-id="cac92-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="cac92-149">Отображаемое имя, отправленное в запросе, — ~! @ # $% ^ &amp; , и в &amp; символе возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="cac92-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="cac92-150">&amp;На одиннадцатую строку и символ 33rd в полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="cac92-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="cac92-151">Получен ответ с кодом HTTP 500.</span><span class="sxs-lookup"><span data-stu-id="cac92-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="cac92-152">См. также</span><span class="sxs-lookup"><span data-stu-id="cac92-152">See also</span></span>

- [<span data-ttu-id="cac92-153">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="cac92-153">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="cac92-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="cac92-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="cac92-155">SetImGroup</span></span>](setimgroup.md)
    

