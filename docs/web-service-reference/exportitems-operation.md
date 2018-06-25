---
title: Операция ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: e2846abb-0b16-4732-bbd8-038a674672f6
description: ExportItems операции экспорта элементов из почтового ящика.
ms.openlocfilehash: 6f0760705c05de2a615544fe52ac50b398be6040
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762441"
---
# <a name="exportitems-operation"></a><span data-ttu-id="b4f94-103">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-103">ExportItems operation</span></span>

<span data-ttu-id="b4f94-104">**ExportItems** операции экспорта элементов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b4f94-104">The **ExportItems** operation exports items out of a mailbox.</span></span> 
  
## <a name="exportitems-request-example"></a><span data-ttu-id="b4f94-105">Пример запроса ExportItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-105">ExportItems request example</span></span>

### <a name="description"></a><span data-ttu-id="b4f94-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f94-106">Description</span></span>

<span data-ttu-id="b4f94-107">В следующем примере запрос **ExportItems** показано, как для формирования запроса для получения трех элементов, экспортированные из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b4f94-107">The following example of an **ExportItems** request shows how to form a request to get three items exported from a mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b4f94-108">Программа</span><span class="sxs-lookup"><span data-stu-id="b4f94-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b4f94-109">Комментарий</span><span class="sxs-lookup"><span data-stu-id="b4f94-109">Comment</span></span>

<span data-ttu-id="b4f94-110">Идентификаторы элементов в примере URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b4f94-110">The item identifiers in the example have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="b4f94-111">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="b4f94-111">Request elements</span></span>

<span data-ttu-id="b4f94-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b4f94-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b4f94-113">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b4f94-113">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="b4f94-114">ExportItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-114">ExportItems</span></span>](exportitems.md)
    
- [<span data-ttu-id="b4f94-115">Что ItemID (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="b4f94-115">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
    
- [<span data-ttu-id="b4f94-116">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b4f94-116">ItemId</span></span>](itemid.md)
    
## <a name="successful-exportitems-response-example"></a><span data-ttu-id="b4f94-117">Пример успешного ответа ExportItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-117">Successful ExportItems response example</span></span>

### <a name="description"></a><span data-ttu-id="b4f94-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f94-118">Description</span></span>

<span data-ttu-id="b4f94-119">В следующем примере показано успешного ответа на запрос **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="b4f94-119">The following example shows a successful response to an **ExportItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b4f94-120">Программа</span><span class="sxs-lookup"><span data-stu-id="b4f94-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <t:ServerVersionInfo MajorVersion="14"
    MinorVersion="1"
    MajorBuildNumber="139"
    MinorBuildNumber="0"
    Version="Exchange2010_SP1"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
    xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            QAAyAAAh9SpR08oBAwAEQAMAFkANABMOAwAAQAMAIQ4AAAAAsIQSN0oAAAAyAGEAYgAxADYA
            MQA2ADYALQBhAGUANQBkAC0ANAAyAGUAZgAtAGEANQA1ADkALQBjADgAOQAwADgANwBkADIA
            MwBkADgANAAAAAMACzf/////AwAgDmQEAAADAPcPAAAAAEAABzBPMXstUdPKAUAACDBPMXst
            UdPKAQMABTcFAAAAsIQONx4AAABtAGUAcwBzAGEAZwBlAC8AcgBmAGMAOAAyADIAAACwhAEw
            IgAAAE0AbwBzAHQAIABmAGEAcwBjAGkAbgBhAHQAaQBuAGcAAAACAfkPBAAAAAAAAAADAAFA
            FABKZ3QrAAAAZF2mAwAXAAEAAACwhBoAEgAAAEkAUABNAC4ATgBvAHQAZQAAAAMANgAAAAAA
            sIQ3ACIAAABNAG8AcwB0ACAAZgBhAHMAYwBpAG4AYQB0AGkAbgBnAAAAQAA5AACq+za80coB
            AgE7AGUAAABFWDovTz1GSVJTVCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RS
            QVRJVkUgR1JPVVAgKEZZRElCT0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05F
            ALCEPQACAAAAAAACAUEAfgAAAAAAAADcp0DIwEIQGrS5CAArL+GCAQAAAAAAAAAvTz1GSVJT
            VCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RSQVRJVkUgR1JPVVAgKEZZRElC
            T0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05FALCEQgAQAAAAVQB
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            BAAAAAYAAAABDouAAAACAAAAEiAAAOSECEBbAAAAL089RklSU1QgT1JHQU5JWkFUSU9OL09V
            PUVYQ0hBTkdFIEFETUlOSVNUUkFUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJF
            Q0lQSUVOVFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAAALACMAAAAL
            ACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUAcwB0AGkAbgBnACAALQAgAGYAcgBv
            AG0AIABFAFcAUwBNAEEAAABAADkAAHZeFxfRygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FO
            SVpBVElPTi9PVT1FWENIQU5HRSBBRE1JTklTVFJBVElWRSBHUk9VUCAoRllESUJPSEYyM1NQ
            RExUKS9DTj1SRUNJUElFTlRTL0NOPVVTRVJPTkUAsIQ9AAIAAAAAAAIBPwB+AAAAAAAAANyn
            QMjAQhAatLkIACsv4YIBAAAAAAAAAC9PPUZJUlNUIE9SR0FOSVpBVElPTi9PVT1FWENIQU5H
          </m:Data>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b4f94-121">Комментарий</span><span class="sxs-lookup"><span data-stu-id="b4f94-121">Comment</span></span>

<span data-ttu-id="b4f94-122">Идентификаторы элементов и ключей изменения в примере URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b4f94-122">The item identifiers and change keys in the example have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="b4f94-123">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="b4f94-123">Response elements</span></span>

<span data-ttu-id="b4f94-124">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b4f94-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b4f94-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b4f94-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b4f94-126">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b4f94-126">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="b4f94-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b4f94-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b4f94-128">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b4f94-128">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="b4f94-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b4f94-129">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b4f94-130">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b4f94-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b4f94-131">Данные (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="b4f94-131">Data (base64Binary)</span></span>](data-base64binary.md)
    
## <a name="exportitems-error-response-example"></a><span data-ttu-id="b4f94-132">Пример ответа об ошибке ExportItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-132">ExportItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b4f94-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f94-133">Description</span></span>

<span data-ttu-id="b4f94-134">В следующем примере показано ответа на запрос **ExportItems** , содержащий два ошибки, один элемент успешно экспортированного.</span><span class="sxs-lookup"><span data-stu-id="b4f94-134">The following example shows a response to the **ExportItems** request that contains two errors and one successfully exported item.</span></span> <span data-ttu-id="b4f94-135">Первый элемент в примере успешно экспортирован.</span><span class="sxs-lookup"><span data-stu-id="b4f94-135">The first item in the example is successfully exported.</span></span> <span data-ttu-id="b4f94-136">Второй элемент содержит неправильные изменить ключ.</span><span class="sxs-lookup"><span data-stu-id="b4f94-136">The second item contains an incorrect change key.</span></span> <span data-ttu-id="b4f94-137">Третий элемент представляет при попытке экспорта элемента из неверный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="b4f94-137">The third item represents an attempt to export an item from the wrong mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b4f94-138">Программа</span><span class="sxs-lookup"><span data-stu-id="b4f94-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGU0oMf0GPIQeAAAAUC8iAABseAAAAUFZ7AAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>No mailbox with such guid.</m:MessageText>
          <m:ResponseCode>ErrorNonExistentMailbox</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:Value Name="MailboxGuid">f3f6f699-2254-40ce-9994-388d9d98419e</t:Value>
          </m:MessageXml>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="comments"></a><span data-ttu-id="b4f94-139">Комментарии</span><span class="sxs-lookup"><span data-stu-id="b4f94-139">Comments</span></span>

<span data-ttu-id="b4f94-140">Идентификаторы элементов, измените ключи и данных в примере URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b4f94-140">The item identifiers, change keys, and data in the example have been shortened to preserve readability.</span></span>
  
### <a name="error-response-elements"></a><span data-ttu-id="b4f94-141">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="b4f94-141">Error response elements</span></span>

<span data-ttu-id="b4f94-142">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b4f94-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b4f94-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b4f94-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b4f94-144">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b4f94-144">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="b4f94-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b4f94-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b4f94-146">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b4f94-146">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="b4f94-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b4f94-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b4f94-148">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b4f94-148">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b4f94-149">Данные (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="b4f94-149">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="b4f94-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="b4f94-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b4f94-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b4f94-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b4f94-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b4f94-152">MessageXml</span></span>](messagexml.md)
    
- <span data-ttu-id="b4f94-153">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b4f94-153">**Value**</span></span>
    
> [!NOTE]
> <span data-ttu-id="b4f94-154">**Значение** элемента не существует в схеме.</span><span class="sxs-lookup"><span data-stu-id="b4f94-154">The **Value** element does not exist in the schema.</span></span> <span data-ttu-id="b4f94-155">Этот элемент является допустимым, так как элемент [MessageXml](messagexml.md) , появлении **значение** экземпляра элемента может содержать любые правильности XML-кода.</span><span class="sxs-lookup"><span data-stu-id="b4f94-155">This element is valid because the [MessageXml](messagexml.md) element, in which the **Value** instance element occurs, can contain any well-formed XML.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b4f94-156">См. также</span><span class="sxs-lookup"><span data-stu-id="b4f94-156">See also</span></span>



[<span data-ttu-id="b4f94-157">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="b4f94-157">UploadItems operation</span></span>](uploaditems-operation.md)


[<span data-ttu-id="b4f94-158">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b4f94-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="b4f94-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b4f94-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

