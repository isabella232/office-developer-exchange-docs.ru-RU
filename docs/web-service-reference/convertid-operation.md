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
description: Найдите сведения о веб-служб Exchange ConvertId операции.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761826"
---
# <a name="convertid-operation"></a><span data-ttu-id="1a40d-103">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="1a40d-103">ConvertId operation</span></span>

<span data-ttu-id="1a40d-104">Найдите сведения о **ConvertId** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a40d-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="1a40d-105">Операции веб-служб Exchange (EWS) **ConvertId** преобразует идентификаторы элементов и папок между форматы, поддерживаемые Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1a40d-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="1a40d-106">С помощью операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="1a40d-106">Using the ConvertId operation</span></span>
<span data-ttu-id="1a40d-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-107"></span></span>

<span data-ttu-id="1a40d-108">Следующие идентификаторы можно преобразовать с помощью операции **ConvertId** :</span><span class="sxs-lookup"><span data-stu-id="1a40d-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="1a40d-109">Формат идентификатора для веб-служб Exchange в первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="1a40d-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="1a40d-110">Представляет `EwsLegacyId` значение перечисления в перечислении [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1a40d-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="1a40d-111">Формат идентификатора для веб-служб Exchange в Exchange 2007 с пакетом обновления 1 или Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="1a40d-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="1a40d-112">Представляет `EwsId` значение перечисления в [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1a40d-112">This is represented by the  `EwsId` enumeration value in [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="1a40d-113">Идентификатор MAPI, как и свойство **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="1a40d-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="1a40d-114">Представляет `EntryId` значение перечисления в перечислении [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1a40d-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="1a40d-115">Идентификатор события календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="1a40d-115">The availability calendar event identifier.</span></span> <span data-ttu-id="1a40d-116">Это представление шестнадцатеричном формате **PR_ENTRYID** свойства.</span><span class="sxs-lookup"><span data-stu-id="1a40d-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="1a40d-117">Представляет `HexEntryId` значение перечисления в [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1a40d-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="1a40d-118">Идентификатор хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a40d-118">The Exchange store identifier.</span></span> <span data-ttu-id="1a40d-119">Представляет `StoreId` значение перечисления в [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1a40d-119">This is represented by the  `StoreId` enumeration value in [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="1a40d-120">Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора веб-служб Exchange на идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="1a40d-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="1a40d-121">Идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="1a40d-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="1a40d-122">Представляет `OwaId` значение перечисления в [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1a40d-122">This is represented by the  `OwaId` enumeration value in [IdFormat](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="1a40d-123">Передача URL-адреса, создаваемые из этот идентификатор в Outlook Web App не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a40d-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="1a40d-124">Идентификатор Outlook Web App можно применять к Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="1a40d-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="1a40d-125">Outlook Web App для Exchange Online и версии Exchange, начиная с Exchange Server 2013 использует идентификаторы веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a40d-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="1a40d-126">Операция **ConvertId** работать неправильно при преобразовании идентификаторы общедоступных папок из идентификатора веб-служб Exchange с идентификатором хранилища в Exchange Online и Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="1a40d-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="1a40d-127">Идентификатор, который возвращается в качестве решения можно обновлять вручную.</span><span class="sxs-lookup"><span data-stu-id="1a40d-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="1a40d-128">Чтобы вручную обновить идентификатор:</span><span class="sxs-lookup"><span data-stu-id="1a40d-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="1a40d-129">В коде приложения определите, является ли элемент или папку в общей папке.</span><span class="sxs-lookup"><span data-stu-id="1a40d-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="1a40d-130">Декодирования строка идентификатора кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="1a40d-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="1a40d-131">Убедитесь, что тип byte (21 байтов) имеет значение 7.</span><span class="sxs-lookup"><span data-stu-id="1a40d-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="1a40d-132">Значение 7 указывает, что идентификатор является неверный формат.</span><span class="sxs-lookup"><span data-stu-id="1a40d-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="1a40d-133">Пропустите первые четыре байта.</span><span class="sxs-lookup"><span data-stu-id="1a40d-133">Skip the first four bytes.</span></span> <span data-ttu-id="1a40d-134">Они должны иметь значение нулю.</span><span class="sxs-lookup"><span data-stu-id="1a40d-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="1a40d-135">Обновление следующего 16 байт с помощью следующих GUID: 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="1a40d-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="1a40d-136">Обновите следующий байт (типа byte) со значением 9.</span><span class="sxs-lookup"><span data-stu-id="1a40d-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="1a40d-137">Измените идентификатор строка в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="1a40d-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1a40d-138">Операция **ConvertId** проверяет, что для данного SMTP-адрес имеет допустимый формат.</span><span class="sxs-lookup"><span data-stu-id="1a40d-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="1a40d-139">Операция не определяет, представляет ли SMTP-адрес допустимым почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1a40d-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="1a40d-140">Операция **ConvertId** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1a40d-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="1a40d-141">**В таблице 1. Заголовки SOAP ConvertId операции**</span><span class="sxs-lookup"><span data-stu-id="1a40d-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="1a40d-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="1a40d-142">**Header**</span></span>|<span data-ttu-id="1a40d-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a40d-143">**Element**</span></span>|<span data-ttu-id="1a40d-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a40d-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1a40d-145">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="1a40d-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="1a40d-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1a40d-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1a40d-147">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="1a40d-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1a40d-148">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="1a40d-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1a40d-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="1a40d-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="1a40d-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1a40d-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1a40d-151">Определяет версию схемы для запроса операции, которые применяются к запросу.</span><span class="sxs-lookup"><span data-stu-id="1a40d-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1a40d-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="1a40d-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="1a40d-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1a40d-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1a40d-154">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="1a40d-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1a40d-155">Это применимо для ответа.</span><span class="sxs-lookup"><span data-stu-id="1a40d-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="1a40d-156">Пример запроса ConvertId операции</span><span class="sxs-lookup"><span data-stu-id="1a40d-156">ConvertId operation request example</span></span>
<span data-ttu-id="1a40d-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-157"></span></span>

<span data-ttu-id="1a40d-158">В следующем примере запрос **ConvertId** показано, как для преобразования из идентификатора веб-служб Exchange в Outlook Web App идентификатора.</span><span class="sxs-lookup"><span data-stu-id="1a40d-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="1a40d-159">Необходимо задать элемент [RequestServerVersion](requestserverversion.md) в заголовке SOAP, чтобы Exchange2007_SP1 или более поздней версии для успешного выполнения этой операции.</span><span class="sxs-lookup"><span data-stu-id="1a40d-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1a40d-160">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1a40d-160">The item identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a><span data-ttu-id="1a40d-161">Пример ответа ConvertId операции</span><span class="sxs-lookup"><span data-stu-id="1a40d-161">ConvertId operation response example</span></span>
<span data-ttu-id="1a40d-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-162"></span></span>

<span data-ttu-id="1a40d-163">В следующем примере показано успешного ответа на запрос **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="1a40d-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="1a40d-164">В этом примере ответа содержит идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="1a40d-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1a40d-165">Идентификатор Outlook Web App был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1a40d-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="1a40d-166">Пример ответа об ошибке ConvertId операции</span><span class="sxs-lookup"><span data-stu-id="1a40d-166">ConvertId operation error response example</span></span>
<span data-ttu-id="1a40d-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-167"></span></span>

<span data-ttu-id="1a40d-168">В следующем примере показано ответа на запрос, который содержит неверный тип формат идентификатора.</span><span class="sxs-lookup"><span data-stu-id="1a40d-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="version-differences"></a><span data-ttu-id="1a40d-169">Различия версий</span><span class="sxs-lookup"><span data-stu-id="1a40d-169">Version differences</span></span>
<span data-ttu-id="1a40d-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-170"></span></span>

<span data-ttu-id="1a40d-171">Формат идентификатора веб-служб Exchange, изменились при переходе от первоначальной версии Exchange 2007 и Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1a40d-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="1a40d-172">Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010 использовать тот же идентификатор формат, который использует Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="1a40d-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="1a40d-173">Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора веб-служб Exchange идентификатор хранилища в Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="1a40d-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1a40d-174">См. также</span><span class="sxs-lookup"><span data-stu-id="1a40d-174">See also</span></span>
<span data-ttu-id="1a40d-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="1a40d-175"></span></span>

- [<span data-ttu-id="1a40d-176">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="1a40d-176">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="1a40d-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="1a40d-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="1a40d-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="1a40d-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

