---
title: Операция SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Поиск сведений о SetImGroupной операции EWS.
ms.openlocfilehash: 37b290559fff0b2de57669741547ba4b1b56c28c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438077"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="3c313-103">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-103">SetImGroup operation</span></span>

<span data-ttu-id="3c313-104">Поиск сведений о **SetImGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="3c313-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3c313-105">Операция **SetImGroup** изменяет отображаемое имя группы обмена мгновенными сообщениями (IM).</span><span class="sxs-lookup"><span data-stu-id="3c313-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="3c313-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c313-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="3c313-107">Использование операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="3c313-108">Для операции **SetImGroup** используется только один аргумент Display Name.</span><span class="sxs-lookup"><span data-stu-id="3c313-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="3c313-109">Заголовки SOAP операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="3c313-110">Операция **SetImGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="3c313-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3c313-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="3c313-111">**Header name**</span></span>|<span data-ttu-id="3c313-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c313-112">**Element**</span></span>|<span data-ttu-id="3c313-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c313-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3c313-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="3c313-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3c313-115">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="3c313-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3c313-116">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="3c313-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3c313-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3c313-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3c313-118">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="3c313-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3c313-119">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="3c313-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3c313-120">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="3c313-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3c313-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3c313-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3c313-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="3c313-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3c313-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="3c313-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3c313-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="3c313-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3c313-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3c313-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3c313-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="3c313-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3c313-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="3c313-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3c313-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="3c313-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3c313-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="3c313-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="3c313-130">Пример запроса операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-130">SetImGroup operation request example</span></span>

<span data-ttu-id="3c313-131">В следующем примере запроса операции **SetImGroup** показано, как изменить отображаемое имя группы IM на "миневграупнаме".</span><span class="sxs-lookup"><span data-stu-id="3c313-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3c313-132">Идентификатор хранилища Exchange был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="3c313-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3c313-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3c313-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3c313-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="3c313-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="3c313-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="3c313-136">невдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3c313-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="3c313-137">Успешный отклик операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="3c313-138">В следующем примере показан успешный ответ на запрос операции **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3c313-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="3c313-139">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3c313-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3c313-140">сетимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="3c313-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="3c313-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3c313-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="3c313-142">Ответ об ошибке операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-142">SetImGroup operation error response</span></span>

<span data-ttu-id="3c313-143">В следующем примере показан ответ об ошибке для запроса операции **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3c313-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="3c313-144">Следующий ответ об ошибке возникает при попытке изменить отображаемое имя группы на отображаемое имя существующей группы.</span><span class="sxs-lookup"><span data-stu-id="3c313-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3c313-145">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3c313-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3c313-146">сетимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="3c313-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="3c313-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="3c313-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3c313-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3c313-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3c313-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="3c313-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="3c313-150">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="3c313-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="3c313-151">См. также</span><span class="sxs-lookup"><span data-stu-id="3c313-151">See also</span></span>

- [<span data-ttu-id="3c313-152">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="3c313-152">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3c313-153">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="3c313-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3c313-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

