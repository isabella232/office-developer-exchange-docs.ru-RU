---
title: Операция ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Найдите сведения об операции ConvertId EWS.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452554"
---
# <a name="convertid-operation"></a><span data-ttu-id="bffa9-103">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-103">ConvertId operation</span></span>

<span data-ttu-id="bffa9-104">Найдите сведения об **операции ConvertId** EWS.</span><span class="sxs-lookup"><span data-stu-id="bffa9-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="bffa9-105">Операция **ConvertId** Веб-службы Exchange (EWS) преобразует идентификаторы элементов и папок между форматами, которые принимаются Exchange Online, Exchange Online как часть Office 365, и локальной версией Exchange, начиная с Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bffa9-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="bffa9-106">Использование операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-106">Using the ConvertId operation</span></span>
<span data-ttu-id="bffa9-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-107"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="bffa9-108">С помощью операции **ConvertId** можно преобразовать следующие идентификаторы:</span><span class="sxs-lookup"><span data-stu-id="bffa9-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="bffa9-109">Формат идентификатора для EWS в первоначальной версии выпуска Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="bffa9-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="bffa9-110">Этот код представлен значением `EwsLegacyId` enumeration в индексе [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="bffa9-111">Формат идентификатора для EWS в Exchange 2007 с sp1 или Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="bffa9-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="bffa9-112">Это представлено значением `EwsId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-112">This is represented by the  `EwsId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="bffa9-113">Идентификатор MAPI, как в свойстве **PR_ENTRYID.**</span><span class="sxs-lookup"><span data-stu-id="bffa9-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="bffa9-114">Этот код представлен значением `EntryId` из нумерации [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="bffa9-115">Идентификатор события календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="bffa9-115">The availability calendar event identifier.</span></span> <span data-ttu-id="bffa9-116">Это представление свойства, закодированное в **PR_ENTRYID** кодировки.</span><span class="sxs-lookup"><span data-stu-id="bffa9-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="bffa9-117">Этот код представлен значением `HexEntryId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="bffa9-118">Идентификатор магазина Exchange.</span><span class="sxs-lookup"><span data-stu-id="bffa9-118">The Exchange store identifier.</span></span> <span data-ttu-id="bffa9-119">Это представлено значением `StoreId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-119">This is represented by the  `StoreId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="bffa9-120">Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор магазина.</span><span class="sxs-lookup"><span data-stu-id="bffa9-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="bffa9-121">Идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="bffa9-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="bffa9-122">Это представлено значением  `OwaId` нумерации в [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="bffa9-122">This is represented by the  `OwaId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="bffa9-123">Передача URL-адресов, созданных из этого идентификатора в Outlook Web App не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffa9-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="bffa9-124">Идентификатор Outlook Web App применяется к Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="bffa9-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="bffa9-125">Outlook Web App Exchange Online и версии Exchange, начиная с Exchange Server 2013, используют идентификаторы EWS.</span><span class="sxs-lookup"><span data-stu-id="bffa9-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="bffa9-126">Операция **ConvertId** работает не так, как ожидалось при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор магазина в Exchange Online и Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="bffa9-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="bffa9-127">Вы можете вручную обновить идентификатор, который возвращается в качестве обходного решения.</span><span class="sxs-lookup"><span data-stu-id="bffa9-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="bffa9-128">Обновление идентификатора вручную:</span><span class="sxs-lookup"><span data-stu-id="bffa9-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="bffa9-129">В коде приложения определите, находится ли целевой элемент или папка в общедоступных папках.</span><span class="sxs-lookup"><span data-stu-id="bffa9-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="bffa9-130">Декодировать строку идентификатора в коде Base64.</span><span class="sxs-lookup"><span data-stu-id="bffa9-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="bffa9-131">Убедитесь, что для типа "byte" (21st byte) занося значение 7.</span><span class="sxs-lookup"><span data-stu-id="bffa9-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="bffa9-132">Значение 7 указывает, что идентификатор имеет неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="bffa9-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="bffa9-133">Пропустите первые четыре bytes.</span><span class="sxs-lookup"><span data-stu-id="bffa9-133">Skip the first four bytes.</span></span> <span data-ttu-id="bffa9-134">Для них должно быть установлено значение 0.</span><span class="sxs-lookup"><span data-stu-id="bffa9-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="bffa9-135">Обновите следующие 16 bytes с помощью следующего GUID: 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="bffa9-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="bffa9-136">Обновите следующий (введите) значение 9.</span><span class="sxs-lookup"><span data-stu-id="bffa9-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="bffa9-137">Измените идентификатор на строку в коде Base64.</span><span class="sxs-lookup"><span data-stu-id="bffa9-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="bffa9-138">Операция **ConvertId** проверяет, имеет ли данный SMTP-адрес допустимый формат.</span><span class="sxs-lookup"><span data-stu-id="bffa9-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="bffa9-139">Операция не определяет, представляет ли SMTP-адрес допустимый почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="bffa9-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="bffa9-140">Операция **ConvertId** может использовать заглавные листы SOAP, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="bffa9-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="bffa9-141">**Таблица 1. ConvertId operation SOAP headers**</span><span class="sxs-lookup"><span data-stu-id="bffa9-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="bffa9-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="bffa9-142">**Header**</span></span>|<span data-ttu-id="bffa9-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bffa9-143">**Element**</span></span>|<span data-ttu-id="bffa9-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bffa9-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bffa9-145">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="bffa9-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="bffa9-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="bffa9-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="bffa9-147">Определяет пользователя, которого подает клиентский приложение.</span><span class="sxs-lookup"><span data-stu-id="bffa9-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="bffa9-148">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="bffa9-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bffa9-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="bffa9-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="bffa9-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="bffa9-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bffa9-151">Определяет версию схемы для запроса на операцию. Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="bffa9-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bffa9-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="bffa9-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="bffa9-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bffa9-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bffa9-154">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="bffa9-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bffa9-155">Это применимо к отклику.</span><span class="sxs-lookup"><span data-stu-id="bffa9-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="bffa9-156">Пример запроса на операцию ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-156">ConvertId operation request example</span></span>
<span data-ttu-id="bffa9-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-157"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="bffa9-158">В следующем примере запроса **ConvertId** показано, как преобразовать идентификатор EWS в Outlook Web App идентификатора.</span><span class="sxs-lookup"><span data-stu-id="bffa9-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="bffa9-159">Для работы этой операции необходимо установить для элемента [RequestServerVersion](requestserverversion.md) в заголе SOAP Exchange2007_SP1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="bffa9-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bffa9-160">Идентификатор элемента был сокращен для сохранения читаемости.</span><span class="sxs-lookup"><span data-stu-id="bffa9-160">The item identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a><span data-ttu-id="bffa9-161">Пример отклика операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-161">ConvertId operation response example</span></span>
<span data-ttu-id="bffa9-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-162"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="bffa9-163">В следующем примере показан успешный ответ на запрос **ConvertId.**</span><span class="sxs-lookup"><span data-stu-id="bffa9-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="bffa9-164">В этом примере ответа содержится Outlook Web App идентификатора.</span><span class="sxs-lookup"><span data-stu-id="bffa9-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bffa9-165">Идентификатор Outlook Web App был сокращен для сохранения читаемости.</span><span class="sxs-lookup"><span data-stu-id="bffa9-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="bffa9-166">Пример отклика об ошибке операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-166">ConvertId operation error response example</span></span>
<span data-ttu-id="bffa9-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-167"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="bffa9-168">В следующем примере показан ответ на запрос, содержащий неправильный тип формата идентификатора.</span><span class="sxs-lookup"><span data-stu-id="bffa9-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="bffa9-169">Различия версий</span><span class="sxs-lookup"><span data-stu-id="bffa9-169">Version differences</span></span>
<span data-ttu-id="bffa9-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-170"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

<span data-ttu-id="bffa9-171">Формат идентификатора EWS изменился между первоначальной версией выпуска Exchange 2007 и Exchange 2007 Пакет обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bffa9-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="bffa9-172">Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010, использует тот же формат идентификаторов, что и Exchange 2007 с sp1.</span><span class="sxs-lookup"><span data-stu-id="bffa9-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="bffa9-173">Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор магазина в Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="bffa9-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bffa9-174">См. также</span><span class="sxs-lookup"><span data-stu-id="bffa9-174">See also</span></span>
<span data-ttu-id="bffa9-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="bffa9-175"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

- [<span data-ttu-id="bffa9-176">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="bffa9-176">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="bffa9-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="bffa9-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="bffa9-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="bffa9-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

