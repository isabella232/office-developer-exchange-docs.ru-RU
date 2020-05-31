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
description: Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности, применяя указанные операции. UpdateInboxRules используется для создания правила папки "Входящие", установки правила для папки "Входящие" или удаления правила для папки "Входящие".
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840343"
---
# <a name="updateinboxrules-operation"></a>Операция UpdateInboxRules

Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности, применяя указанные операции. **UpdateInboxRules** используется для создания правила папки "Входящие", установки правила для папки "Входящие" или удаления правила для папки "Входящие". 
  
При использовании операции **UpdateInboxRules** веб-службы Exchange удаляют правила отправки на стороне клиента. Правила отправки на стороне клиента хранятся в клиенте в сообщении о связанной папке правила (ФАИ), но не в других. По умолчанию служба EWS удаляет это правило ФАИ по умолчанию, в зависимости от того, что Outlook будет воссоздать его. Однако Outlook не может создавать правила, которые не существуют как расширенное правило, а правила отправки на стороне клиента не являются расширенными правилами. В результате эти правила теряются. Мы рекомендуем использовать это при проектировании решения. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Пример запроса UpdateInboxRules (Create Rule)

Вы можете использовать веб-службы Exchange, чтобы создать правило для папки "Входящие" в почтовом ящике пользователя в хранилище Exchange. Чтобы создать правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [креатерулеоператион](createruleoperation.md) . 
  
### <a name="description"></a>Описание

Клиент создает XML-код запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В этом примере создается правило, которое переместит сообщение электронной почты в папку нежелательной почты, если тема сообщения содержит строку, содержательную "интересное".
  
### <a name="request-elements"></a>Элементы Request

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [маилбокссмтпаддресс](mailboxsmtpaddress.md)
    
- [ремовеаутлукрулеблоб](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [креатерулеоператион](createruleoperation.md) для создания правила. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Пример отклика UpdateInboxRules (Create Rule)

### <a name="description"></a>Описание

В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который создает правило. 
  
### <a name="code"></a>Код

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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Пример запроса UpdateInboxRules (Set Rule)

Вы можете использовать веб-службы Exchange для изменения правила папки "Входящие" в почтовом ящике пользователя в хранилище Exchange. Чтобы изменить правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [сетрулеоператион](setruleoperation.md) . 
  
### <a name="description"></a>Описание

Клиент создает XML-код запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В этом примере показано изменение отображаемого имени на "(изменено) это нежелательное".
  
> [!NOTE]
> Значения атрибутов **ID** и **чанжекэй** элемента [FolderId](folderid.md) сокращены для удобочитаемости. 
  
### <a name="request-elements"></a>Элементы Request

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [маилбокссмтпаддресс](mailboxsmtpaddress.md)
    
- [ремовеаутлукрулеблоб](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [сетрулеоператион](setruleoperation.md) для изменения правила. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Пример отклика UpdateInboxRules (Set Rule)

### <a name="description"></a>Описание

В следующем примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который изменяет правило. 
  
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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Пример запроса UpdateInboxRules (Delete Rule)

Вы можете использовать веб-службы Exchange для удаления правила папки "Входящие" в почтовом ящике пользователя в хранилище Exchange. Чтобы удалить правило, используйте [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [делетерулеоператион](deleteruleoperation.md) . 
  
### <a name="description"></a>Описание

Клиент создает XML-код запроса и отправляет его на сервер.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В этом примере удаляется существующее идентифицированное правило.
  
### <a name="request-elements"></a>Элементы Request

Запрос **UpdateInboxRules** включает следующие элементы: 
  
- [маилбокссмтпаддресс](mailboxsmtpaddress.md)
    
- [ремовеаутлукрулеблоб](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
Элемент [Operations](operations.md) содержит элемент [делетерулеоператион](deleteruleoperation.md) для удаления правила. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Пример отклика UpdateInboxRules (удаление правила)

### <a name="description"></a>Описание

В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который удаляет правило. 
  
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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="see-also"></a>См. также



[Операция GetInboxRules](getinboxrules-operation.md)

