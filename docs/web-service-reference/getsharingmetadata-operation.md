---
title: Операция GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: eaf29427-ecf8-4a5e-9a54-db2e6414b35e
description: Операция GetSharingMetadata получает маркер непрозрачной проверки подлинности, определяющий приглашение к совместному использованию.
ms.openlocfilehash: e2e04d83310e7a8a731cca655a432325574cd9e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833671"
---
# <a name="getsharingmetadata-operation"></a><span data-ttu-id="f4dbe-103">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f4dbe-103">GetSharingMetadata operation</span></span>

<span data-ttu-id="f4dbe-104">Операция **GetSharingMetadata** получает маркер непрозрачной проверки подлинности, определяющий приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-104">The **GetSharingMetadata** operation gets an opaque authentication token that identifies a sharing invitation.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="f4dbe-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="f4dbe-105">SOAP Headers</span></span>

<span data-ttu-id="f4dbe-106">Операция **GetSharingMetadata** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-106">The **GetSharingMetadata** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="f4dbe-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="f4dbe-107">**Header**</span></span>|<span data-ttu-id="f4dbe-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4dbe-108">**Element**</span></span>|<span data-ttu-id="f4dbe-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4dbe-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f4dbe-110">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="f4dbe-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="f4dbe-111">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="f4dbe-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f4dbe-112">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="f4dbe-113">серверверсион</span><span class="sxs-lookup"><span data-stu-id="f4dbe-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="f4dbe-114">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="f4dbe-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f4dbe-115">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingmetadata-request-example"></a><span data-ttu-id="f4dbe-116">Пример запроса GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f4dbe-116">GetSharingMetadata request example</span></span>

### <a name="description"></a><span data-ttu-id="f4dbe-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f4dbe-117">Description</span></span>

<span data-ttu-id="f4dbe-118">В приведенном ниже примере показано, как сформировать запрос на получение непрозрачного маркера проверки подлинности, определяющего приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-118">The following example shows how to form a request to get an opaque authentication token that identifies a sharing invitation.</span></span> <span data-ttu-id="f4dbe-119">В этом примере user1@contoso.com хочет предоставить общий доступ к папке, указанной элементом [идоффолдертошаре](idoffoldertoshare.md) , с user1@fabikam.com и user2@test.com.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-119">In this example, user1@contoso.com wants to share the folder that is specified by the [IdOfFolderToShare](idoffoldertoshare.md) element with user1@fabikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f4dbe-120">Код</span><span class="sxs-lookup"><span data-stu-id="f4dbe-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingMetadata>
      <m:IdOfFolderToShare Id="AAMkAD=" ChangeKey="AwAAA=" />
      <m:SenderSmtpAddress>user1@contoso.com</m:SenderSmtpAddress>
      <m:Recipients>
        <t:SmtpAddress>user1@fabrikam.com</t:SmtpAddress>
        <t:SmtpAddress>user2@test.com</t:SmtpAddress>
      </m:Recipients>
    </m:GetSharingMetadata>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f4dbe-121">Comments</span><span class="sxs-lookup"><span data-stu-id="f4dbe-121">Comments</span></span>

<span data-ttu-id="f4dbe-122">Элемент [Recipients (аррайофсмтпаддресстипе)](recipients-arrayofsmtpaddresstype.md) содержит один элемент [SmtpAddress](smtpaddress.md) для каждого получателя приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-122">The [Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) element contains one [SmtpAddress](smtpaddress.md) element for each intended recipient of the sharing invitation.</span></span> 
  
## <a name="successful-getsharingmetadata-response"></a><span data-ttu-id="f4dbe-123">Успешный ответ GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f4dbe-123">Successful GetSharingMetadata Response</span></span>

### <a name="description"></a><span data-ttu-id="f4dbe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f4dbe-124">Description</span></span>

<span data-ttu-id="f4dbe-125">В следующем примере показан успешный ответ на запрос **GetSharingMetadata** .</span><span class="sxs-lookup"><span data-stu-id="f4dbe-125">The following example shows a successful response to a **GetSharingMetadata** request.</span></span> <span data-ttu-id="f4dbe-126">В этом примере в соответствующем запросе **GetSharingMetadata** указаны два получателя: user1@fabrikam.com и user2@test.com.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-126">In this example, two recipients were specified in the corresponding **GetSharingMetadata** request: user1@fabrikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f4dbe-127">Код</span><span class="sxs-lookup"><span data-stu-id="f4dbe-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingMetadataResponseMessage ResponseClass="Success" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</ResponseCode>
      <m:EncryptedSharedFolderDataCollection>
        <t:EncryptedSharedFolderData>
          <t:Token>
            <EncryptedData Id="Assertion0" Type="http://www.w3.org/2001/04/xmlenc#Element" xmlns="http://www.w3.org/2001/04/xmlenc#">
              <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#tripledes-cbc"></EncryptionMethod>
              <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
                <EncryptedKey>
                  <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#rsa-oaep-mgf1p"></EncryptionMethod>
                  <ds:KeyInfo Id="keyinfo">
                    <wsse:SecurityTokenReference xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
                      <wsse:KeyIdentifier 
                                  EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary" 
                                  ValueType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0#X509SubjectKeyIdentifier">
                        B4VEEAf=
                      </wsse:KeyIdentifier>
                    </wsse:SecurityTokenReference>
                  </ds:KeyInfo>
                  <CipherData>
                    <CipherValue>GI/Dxqvw2na==</CipherValue>
                  </CipherData>
                </EncryptedKey>
              </ds:KeyInfo>
              <CipherData>
                <CipherValue>L77I7Hr06z</CipherValue>
              </CipherData>
            </EncryptedData>
          </t:Token>
          <t:Data>
            <EncryptedData Type="http://www.w3.org/2001/04/xmlenc#Element" xmlns="http://www.w3.org/2001/04/xmlenc#">
              <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#aes256-cbc" />
              <KeyInfo xmlns="http://www.w3.org/2000/09/xmldsig#">
                <EncryptedKey xmlns="http://www.w3.org/2001/04/xmlenc#">
                  <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#kw-tripledes" />
                  <KeyInfo xmlns="http://www.w3.org/2000/09/xmldsig#">
                    <KeyName>key</KeyName>
                  </KeyInfo>
                  <CipherData>
                    <CipherValue>9UgtjrHiU</CipherValue>
                  </CipherData>
                </EncryptedKey>
              </KeyInfo>
              <CipherData>
                <CipherValue>NCNsJoGtQ==</CipherValue>
              </CipherData>
            </EncryptedData>
          </t:Data>
        </t:EncryptedSharedFolderData>
      </m:EncryptedSharedFolderDataCollection>
      <m:InvalidRecipients>
        <t:InvalidRecipient>
          <t:SmtpAddress>user2@test.com</t:SmtpAddress>
          <t:ResponseCode>RecipientOrganizationNotFederated</t:ResponseCode>
          <m:MessageText>The organization of these recipients is not federated for external sharing.</m:MessageText>
        </t:InvalidRecipient>
      </m:InvalidRecipients>
    </GetSharingMetadataResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f4dbe-128">Comments</span><span class="sxs-lookup"><span data-stu-id="f4dbe-128">Comments</span></span>

<span data-ttu-id="f4dbe-129">Ответ содержит один элемент [енкриптедшаредфолдердата](encryptedsharedfolderdata.md) для каждой организации, представленной действительными получателями, указанными в запросе **GetSharingMetadata** .</span><span class="sxs-lookup"><span data-stu-id="f4dbe-129">The response contains one [EncryptedSharedFolderData](encryptedsharedfolderdata.md) element for each organization that is represented by valid recipients that are specified in the **GetSharingMetadata** request.</span></span> 
  
<span data-ttu-id="f4dbe-130">Запрос **GetSharingMetadata** будет успешным, даже если в запросе указаны недопустимые получатели.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-130">The **GetSharingMetadata** request will succeed even if invalid recipients are specified in the request.</span></span> <span data-ttu-id="f4dbe-131">Элемент [инвалидреЦипиентс](invalidrecipients.md) содержит сведения о недопустимых получателях.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-131">The [InvalidRecipients](invalidrecipients.md) element contains information about invalid recipients.</span></span> <span data-ttu-id="f4dbe-132">Сведения о причинах недопустимых получателей можно узнать в статье [респонсекоде (инвалидреЦипиентреспонсекодетипе)](responsecode-invalidrecipientresponsecodetype.md).</span><span class="sxs-lookup"><span data-stu-id="f4dbe-132">For information about the reasons why a recipient might be invalid, see [ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md).</span></span>
  
<span data-ttu-id="f4dbe-133">Если все предполагаемые получатели являются недопустимыми, элемент [енкриптедшаредфолдердатаколлектион](encryptedsharedfolderdatacollection.md) будет пустым.</span><span class="sxs-lookup"><span data-stu-id="f4dbe-133">If all intended recipients are invalid, the [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) element will be empty.</span></span> 
  
## <a name="getsharingmetadata-error-response"></a><span data-ttu-id="f4dbe-134">Ответ об ошибке GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f4dbe-134">GetSharingMetadata error response</span></span>

### <a name="description"></a><span data-ttu-id="f4dbe-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f4dbe-135">Description</span></span>

<span data-ttu-id="f4dbe-136">В следующем примере показан ответ об ошибке для запроса **GetSharingMetadata** .</span><span class="sxs-lookup"><span data-stu-id="f4dbe-136">The following example shows an error response to a **GetSharingMetadata** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f4dbe-137">Код</span><span class="sxs-lookup"><span data-stu-id="f4dbe-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingMetadataResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>The SMTP address format is invalid.</MessageText>
      <m:ResponseCode>ErrorInvalidSmtpAddress</ResponseCode>
      <m:DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetSharingMetadataResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f4dbe-138">См. также</span><span class="sxs-lookup"><span data-stu-id="f4dbe-138">See also</span></span>



[<span data-ttu-id="f4dbe-139">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f4dbe-139">GetSharingMetadata</span></span>](getsharingmetadata.md)
  
[<span data-ttu-id="f4dbe-140">жетшарингметадататипе</span><span class="sxs-lookup"><span data-stu-id="f4dbe-140">GetSharingMetadataType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataType.aspx)
  
[<span data-ttu-id="f4dbe-141">жетшарингметадатареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f4dbe-141">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md)
  
[<span data-ttu-id="f4dbe-142">жетшарингметадатареспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="f4dbe-142">GetSharingMetadataResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataResponseMessageType.aspx)


[<span data-ttu-id="f4dbe-143">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4dbe-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="f4dbe-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4dbe-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

