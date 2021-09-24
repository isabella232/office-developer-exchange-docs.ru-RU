---
title: Операция UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: Операция UpdateInboxRules обновляет правила проверки подлинности пользователя в почтовых ящиках, применяя указанные операции. UpdateInboxRules используется для создания правила "Входящие", для набора правила "Входящие" или для удаления правила "Входящие".
ms.openlocfilehash: 08f46219bcb01f5f1c9d69cfaa8b4934e82ff5bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510717"
---
# <a name="updateinboxrules-operation"></a>Операция UpdateInboxRules

Операция UpdateInboxRules обновляет правила проверки подлинности пользователя в почтовых ящиках, применяя указанные операции. **UpdateInboxRules** используется для создания правила "Входящие", для набора правила "Входящие" или для удаления правила "Входящие". 
  
При использовании операции **UpdateInboxRules** Exchange веб-службы удаляют правила отправки с клиентской стороны. Правила отправки на стороне клиента хранятся на клиенте в сообщении Попутной информации папки правила (FAI) и нигде больше. EWS удаляет сообщение FAI этого правила по умолчанию, основываясь на ожидании того, что Outlook его воссоздает. Однако Outlook не могут воссоздать правила, которые также не существуют в качестве расширенного правила, а правила отправки на стороне клиента не существуют в качестве расширенных правил. В результате эти правила теряются. Мы рекомендуем учитывать это при разработке решения. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Пример запроса UpdateInboxRules (Создание правила)

Вы можете Exchange веб-службы для создания правила "Входящие" в почтовом ящике пользователя в Exchange магазине. Чтобы создать правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) совместно с элементом [CreateRuleOperation.](createruleoperation.md) 
  
### <a name="description"></a>Описание

Клиент строит XML запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В этом примере создается правило, которое перемещает сообщение электронной почты в папку нежелательной почты, если тема электронной почты содержит строку, равную "Interesting".
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** содержит следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [CreateRuleOperation](createruleoperation.md) для создания правила. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Пример ответа UpdateInboxRules (Создание правила)

### <a name="description"></a>Описание

В следующем примере Протокол SOAP (SOAP) показан успешный ответ на запрос **UpdateInboxRules,** создав правило. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="updateinboxrules-set-rule-request-example"></a>Пример запроса UpdateInboxRules (Set Rule)

Вы можете Exchange веб-службы для изменения правила почтовых ящиков в почтовом ящике пользователя в Exchange магазине. Чтобы изменить правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) совместно с элементом [SetRuleOperation.](setruleoperation.md) 
  
### <a name="description"></a>Описание

Клиент строит XML запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

В этом примере имя отображения изменяется на "(Изменено) Это нежелательно".
  
> [!NOTE]
> Для читаемости сокращены значения атрибутов **Id** и **ChangeKey** элемента [FolderId.](folderid.md) 
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** содержит следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [SetRuleOperation](setruleoperation.md) для изменения правила. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Пример ответа UpdateInboxRules (Set Rule)

### <a name="description"></a>Описание

В следующем примере Протокол SOAP (SOAP) показан успешный ответ на запрос **UpdateInboxRules,** который изменяет правило. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Пример запроса UpdateInboxRules (Правило удаления)

Вы можете Exchange веб-службы, чтобы удалить правило "Входящие" в почтовом ящике пользователя в Exchange магазине. Чтобы удалить правило, используйте [UpdateInboxRules](updateinboxrules.md) совместно с элементом [DeleteRuleOperation.](deleteruleoperation.md) 
  
### <a name="description"></a>Описание

Клиент строит XML запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В этом примере удаляется существующее идентифицированное правило.
  
### <a name="request-elements"></a>Элементы запроса

Запрос **UpdateInboxRules** содержит следующие элементы: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [DeleteRuleOperation](deleteruleoperation.md) для удаления правила. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Пример ответа UpdateInboxRules (Правило удаления)

### <a name="description"></a>Описание

В следующем примере Протокол SOAP (SOAP) показан успешный ответ на запрос **UpdateInboxRules,** который удаляет правило. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

