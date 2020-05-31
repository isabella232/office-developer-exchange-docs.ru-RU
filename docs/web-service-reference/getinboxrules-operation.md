---
title: Операция GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: Операция GetInboxRules использует веб-службы Exchange для получения правил для папки "Входящие" в почтовом ящике определенного пользователя.
ms.openlocfilehash: f8a5068b1f189cc6fd5feef6dfec29204a0b8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762814"
---
# <a name="getinboxrules-operation"></a>Операция GetInboxRules

Операция **GetInboxRules** использует веб-службы Exchange для получения правил для папки "Входящие" в почтовом ящике определенного пользователя. 
  
## <a name="getinboxrules-request-example"></a>Пример запроса GetInboxRules

### <a name="description"></a>Описание

В следующем примере показан XML-код запроса, который клиент отправляет на сервер. Запрос идентифицирует пользователя в элементе [маилбокссмтпаддресс](mailboxsmtpaddress.md) . Все правила для папки "Входящие" для указанного пользователя возвращаются в ответе. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetInboxRules>
      <m:MailboxSmtpAddress>User1@Contoso.com</m:MailboxSmtpAddress>
    </m:GetInboxRules>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

Запрос включает следующий необязательный элемент:
  
- [маилбокссмтпаддресс](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a>Пример успешного ответа GetInboxRules

### <a name="description"></a>Описание

В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **GetInboxRules** . В этом примере ответ включает одно правило. 
  
> [!NOTE]
> Значения **ID** и атрибуты **чанжекэй** элемента [FolderId](folderid.md) были сокращены для сохранения удобочитаемости. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <RuleId>dCsAAABjzvA=</RuleId>
          <DisplayName>MoveInterestingToJunk</DisplayName>
          <Priority>1</Priority>
          <IsEnabled>true</IsEnabled>
          <Conditions>
            <ContainsSubjectStrings>
              <String>Interesting</String>
            </ContainsSubjectStrings>
          </Conditions>
          <Actions>
            <MoveToFolder>
              <FolderId ChangeKey="AQAAAA==" Id="AAMkAGYzZjZm" />
            </MoveToFolder>
          </Actions>
        </Rule>
      </InboxRules>
    </GetInboxRulesResponse>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a>Элементы Response

В ответ включаются следующие элементы:
  
- [жетинбоксрулесреспонсе](getinboxrulesresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [аутлукрулеблобексистс](outlookruleblobexists.md)
    
- [инбоксрулес](inboxrules.md)
    
## <a name="see-also"></a>См. также



[Операция UpdateInboxRules](updateinboxrules-operation.md)

