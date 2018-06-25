---
title: Операция UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности с применением указанной операции. UpdateInboxRules используется для создания правила папки «Входящие», правила папки "Входящие" или удаление правила папки «Входящие».
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840343"
---
# <a name="updateinboxrules-operation"></a>Операция UpdateInboxRules

Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности с применением указанной операции. **UpdateInboxRules** используется для создания правила папки «Входящие», правила папки "Входящие" или удаление правила папки «Входящие». 
  
При использовании операции **UpdateInboxRules** веб-служб Exchange удаляет правила отправки со стороны клиента. Отправить клиентские правила, хранятся в клиенте в правиле сообщение связанные сведения о папке (FAI) и нигде больше. Веб-служб Exchange удаление этого правила FAI сообщения по умолчанию на основании считает, что Outlook будет создать его заново. Тем не менее Outlook не удается заново создать правила несуществующим в качестве расширенного правила и отправки клиентские правила не существовать в качестве расширенного правила. В результате эти правила не сохраняются. Мы рекомендуем вам необходимо учитывать это при разработке решения. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Пример запроса UpdateInboxRules (создать правило)

Можно использовать веб-служб Exchange для создания правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange. Используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [CreateRuleOperation](createruleoperation.md) для создания правила. 
  
### <a name="description"></a>Описание

Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:CreateRuleOperation>
            <t:Rule>
              <t:DisplayName>MoveInterestingToJunk</t:DisplayName>
              <t:Priority>1</t:Priority>
              <t:IsEnabled>true</t:IsEnabled>
              <t:Conditions>
                <t:ContainsSubjectStrings>
                  <t:String>Interesting</t:String>
                </t:ContainsSubjectStrings>
              </t:Conditions>
              <t:Exceptions />
              <t:Actions>
                <t:MoveToFolder>
                  <t:DistinguishedFolderId Id="junkemail" />
                </t:MoveToFolder>
              </t:Actions>
            </t:Rule>
          </t:CreateRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Комментарии

В этом примере выполняется построение правило, которое будут перемещаться сообщения электронной почты в папку нежелательной почты, если тему сообщения электронной почты содержит строку, равный «Interesting».
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Операции](operations.md)
    
Элемент [операции](operations.md) содержит элемент [CreateRuleOperation](createruleoperation.md) для создания правила. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Пример ответа UpdateInboxRules (создать правило)

### <a name="description"></a>Описание

В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , который создает правило. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Пример запроса UpdateInboxRules (задать правила)

Можно использовать веб-служб Exchange для изменения правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange. Используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [SetRuleOperation](setruleoperation.md) для изменения правила. 
  
### <a name="description"></a>Описание

Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <Rule>
              <RuleId>Nh8AAAAwW/w=</RuleId>
              <DisplayName>(Modified) This is Junk</DisplayName>
              <Priority>1</Priority>
              <IsEnabled>true</IsEnabled>
              <Conditions>
                <ContainsSubjectStrings>
                  <String>Interesting</String>
                </ContainsSubjectStrings>
              </Conditions>
              <Actions>
                <MoveToFolder>
                  <FolderId Id="AAMkADQ1YTE1" ChangeKey="AQAAAA==" />
                </MoveToFolder>
              </Actions>
            </Rule>
          </SetRuleOperation>
        </Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Комментарии

В этом примере изменяется отображаемое имя для «(изменено) это нежелательной».
  
> [!NOTE]
> Значения **Id** и **ChangeKey** атрибутов элемента [FolderId](folderid.md) URL были сокращены для удобства чтения. 
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Операции](operations.md)
    
Элемент [операции](operations.md) содержит элемент [SetRuleOperation](setruleoperation.md) для изменения правила. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Пример ответа UpdateInboxRules (задать правила)

### <a name="description"></a>Описание

В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , обеспечивающий изменение правила. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Пример запроса UpdateInboxRules (Удалить)

Можно использовать веб-служб Exchange для удаления правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange. Используйте совместно с элементом [DeleteRuleOperation](deleteruleoperation.md) [UpdateInboxRules](updateinboxrules.md) для удаления правила. 
  
### <a name="description"></a>Описание

Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:DeleteRuleOperation>
            <t:RuleId>Nh8AAAAwW/U=</t:RuleId>
          </t:DeleteRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Комментарии

В этом примере удаляется существующий определенного правила.
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Операции](operations.md)
    
Элемент [операции](operations.md) содержит элемент [DeleteRuleOperation](deleteruleoperation.md) удаление правила. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Пример ответа UpdateInboxRules (Удалить)

### <a name="description"></a>Описание

В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , который удаляет правило. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>См. также



[Операция GetInboxRules](getinboxrules-operation.md)

