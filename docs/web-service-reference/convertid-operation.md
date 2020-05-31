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
description: Поиск сведений о ConvertIdной операции EWS.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761826"
---
# <a name="convertid-operation"></a><span data-ttu-id="7fbd4-103">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-103">ConvertId operation</span></span>

<span data-ttu-id="7fbd4-104">Поиск сведений о **ConvertIdной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="7fbd4-105">**ConvertId** веб-служб Exchange (EWS) преобразует идентификаторы элементов и папок между форматами, принятыми Exchange Online, Exchange Online в составе Office 365, и локальными версиями Exchange, начиная с Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="7fbd4-106">Использование операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-106">Using the ConvertId operation</span></span>
<span data-ttu-id="7fbd4-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-107"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="7fbd4-108">С помощью операции **ConvertId** можно преобразовать следующие идентификаторы:</span><span class="sxs-lookup"><span data-stu-id="7fbd4-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="7fbd4-109">Формат идентификатора для EWS в первой версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="7fbd4-110">Представляется значением `EwsLegacyId` перечисления в перечислении [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7fbd4-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="7fbd4-111">Формат идентификатора для EWS в Exchange 2007 с пакетом обновления 1 (SP1) или Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="7fbd4-112">Представляется значением `EwsId` перечисления в [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7fbd4-112">This is represented by the  `EwsId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="7fbd4-113">Идентификатор MAPI, как в свойстве **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="7fbd4-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="7fbd4-114">Представляется значением `EntryId` перечисления в перечислении [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7fbd4-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="7fbd4-115">Идентификатор события календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-115">The availability calendar event identifier.</span></span> <span data-ttu-id="7fbd4-116">Это представление свойства **PR_ENTRYID** в шестнадцатеричной кодировке.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="7fbd4-117">Представляется значением `HexEntryId` перечисления в [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7fbd4-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="7fbd4-118">Идентификатор хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-118">The Exchange store identifier.</span></span> <span data-ttu-id="7fbd4-119">Представляется значением `StoreId` перечисления в [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7fbd4-119">This is represented by the  `StoreId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="7fbd4-120">Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="7fbd4-121">Идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="7fbd4-122">Представляется значением `OwaId` перечисления в [идформат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7fbd4-122">This is represented by the  `OwaId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="7fbd4-123">Передача URL-адресов, созданных из этого идентификатора в Outlook Web App, не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="7fbd4-124">Идентификатор Outlook Web App применяется к Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="7fbd4-125">Outlook Web App для Exchange Online и версии Exchange, начиная с Exchange Server 2013, используют идентификаторы EWS.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="7fbd4-126">Операция **ConvertId** не работает должным образом при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор хранилища в Exchange Online и Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="7fbd4-127">Вы можете вручную обновить идентификатор, возвращаемый в качестве обходного пути.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="7fbd4-128">Чтобы вручную обновить идентификатор, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7fbd4-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="7fbd4-129">В коде приложения определите, находится ли целевой элемент или папка в общедоступной папке.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="7fbd4-130">Расшифровать строку идентификатора в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="7fbd4-131">Убедитесь, что тип Byte (21-байтовый) имеет значение 7.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="7fbd4-132">Значение 7 указывает на то, что идентификатор имеет недопустимый формат.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="7fbd4-133">Пропустите первые четыре байта.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-133">Skip the first four bytes.</span></span> <span data-ttu-id="7fbd4-134">Им необходимо присвоить нулевое значение.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="7fbd4-135">Обновите следующие 16 байт с помощью следующего GUID: 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="7fbd4-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="7fbd4-136">Обновите следующий байт (тип Byte) со значением 9.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="7fbd4-137">Замените идентификатор на строку в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7fbd4-138">Операция **ConvertId** проверяет, что заданный SMTP-адрес имеет допустимый формат.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="7fbd4-139">Эта операция не определяет, представляет ли SMTP-адрес действительный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="7fbd4-140">Операция **ConvertId** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="7fbd4-141">**Таблица 1. Заголовки SOAP операции ConvertId**</span><span class="sxs-lookup"><span data-stu-id="7fbd4-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="7fbd4-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="7fbd4-142">**Header**</span></span>|<span data-ttu-id="7fbd4-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7fbd4-143">**Element**</span></span>|<span data-ttu-id="7fbd4-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7fbd4-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7fbd4-145">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="7fbd4-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="7fbd4-146">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="7fbd4-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7fbd4-147">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7fbd4-148">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7fbd4-149">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="7fbd4-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="7fbd4-150">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="7fbd4-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7fbd4-151">Определяет версию схемы для запроса операции это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7fbd4-152">серверверсион</span><span class="sxs-lookup"><span data-stu-id="7fbd4-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="7fbd4-153">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="7fbd4-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7fbd4-154">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7fbd4-155">Это относится к отклику.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="7fbd4-156">Пример запроса операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-156">ConvertId operation request example</span></span>
<span data-ttu-id="7fbd4-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-157"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="7fbd4-158">В приведенном ниже примере запроса **ConvertId** показано, как преобразовать идентификатор EWS в идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="7fbd4-159">Чтобы эта операция работала, элемент [рекуестсерверверсион](requestserverversion.md) в заголовке SOAP должен иметь значение Exchange2007_SP1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7fbd4-160">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-160">The item identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-response-example"></a><span data-ttu-id="7fbd4-161">Пример ответа операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-161">ConvertId operation response example</span></span>
<span data-ttu-id="7fbd4-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-162"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="7fbd4-163">В следующем примере показан успешный ответ на запрос **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="7fbd4-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="7fbd4-164">В этом примере ответа содержится идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7fbd4-165">Идентификатор Outlook Web App был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="7fbd4-166">Пример ответа на сообщение об ошибке операции ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-166">ConvertId operation error response example</span></span>
<span data-ttu-id="7fbd4-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-167"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="7fbd4-168">В следующем примере показан ответ на запрос, который содержит недопустимый тип формата идентификатора.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
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

## <a name="version-differences"></a><span data-ttu-id="7fbd4-169">Различия версий</span><span class="sxs-lookup"><span data-stu-id="7fbd4-169">Version differences</span></span>
<span data-ttu-id="7fbd4-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-170"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

<span data-ttu-id="7fbd4-171">Формат идентификатора EWS изменился между исходной версией Exchange 2007 и Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7fbd4-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="7fbd4-172">Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010, используют тот же формат идентификатора, который использует Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7fbd4-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="7fbd4-173">Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор хранилища в Exchange 2007 и Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="7fbd4-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7fbd4-174">См. также</span><span class="sxs-lookup"><span data-stu-id="7fbd4-174">See also</span></span>
<span data-ttu-id="7fbd4-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="7fbd4-175"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

- [<span data-ttu-id="7fbd4-176">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="7fbd4-176">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="7fbd4-177">конвертидтипе</span><span class="sxs-lookup"><span data-stu-id="7fbd4-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="7fbd4-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="7fbd4-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

