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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840343"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="4f465-104">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4f465-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="4f465-105">Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности с применением указанной операции.</span><span class="sxs-lookup"><span data-stu-id="4f465-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="4f465-106">**UpdateInboxRules** используется для создания правила папки «Входящие», правила папки "Входящие" или удаление правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="4f465-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="4f465-107">При использовании операции **UpdateInboxRules** веб-служб Exchange удаляет правила отправки со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="4f465-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="4f465-108">Отправить клиентские правила, хранятся в клиенте в правиле сообщение связанные сведения о папке (FAI) и нигде больше.</span><span class="sxs-lookup"><span data-stu-id="4f465-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="4f465-109">Веб-служб Exchange удаление этого правила FAI сообщения по умолчанию на основании считает, что Outlook будет создать его заново.</span><span class="sxs-lookup"><span data-stu-id="4f465-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="4f465-110">Тем не менее Outlook не удается заново создать правила несуществующим в качестве расширенного правила и отправки клиентские правила не существовать в качестве расширенного правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="4f465-111">В результате эти правила не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="4f465-111">As a result, these rules are lost.</span></span> <span data-ttu-id="4f465-112">Мы рекомендуем вам необходимо учитывать это при разработке решения.</span><span class="sxs-lookup"><span data-stu-id="4f465-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="4f465-113">Пример запроса UpdateInboxRules (создать правило)</span><span class="sxs-lookup"><span data-stu-id="4f465-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="4f465-114">Можно использовать веб-служб Exchange для создания правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f465-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4f465-115">Используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [CreateRuleOperation](createruleoperation.md) для создания правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4f465-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-116">Description</span></span>

<span data-ttu-id="4f465-117">Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="4f465-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f465-118">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-118">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="4f465-119">Комментарии</span><span class="sxs-lookup"><span data-stu-id="4f465-119">Comments</span></span>

<span data-ttu-id="4f465-120">В этом примере выполняется построение правило, которое будут перемещаться сообщения электронной почты в папку нежелательной почты, если тему сообщения электронной почты содержит строку, равный «Interesting».</span><span class="sxs-lookup"><span data-stu-id="4f465-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="4f465-121">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="4f465-121">Request elements</span></span>

<span data-ttu-id="4f465-122">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4f465-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4f465-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4f465-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4f465-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4f465-125">Операции</span><span class="sxs-lookup"><span data-stu-id="4f465-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="4f465-126">Элемент [операции](operations.md) содержит элемент [CreateRuleOperation](createruleoperation.md) для создания правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="4f465-127">Пример ответа UpdateInboxRules (создать правило)</span><span class="sxs-lookup"><span data-stu-id="4f465-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4f465-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-128">Description</span></span>

<span data-ttu-id="4f465-129">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , который создает правило.</span><span class="sxs-lookup"><span data-stu-id="4f465-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4f465-130">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-130">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="4f465-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="4f465-131">Successful response elements</span></span>

<span data-ttu-id="4f465-132">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4f465-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f465-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4f465-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4f465-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4f465-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4f465-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4f465-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4f465-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="4f465-137">Пример запроса UpdateInboxRules (задать правила)</span><span class="sxs-lookup"><span data-stu-id="4f465-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="4f465-138">Можно использовать веб-служб Exchange для изменения правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f465-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4f465-139">Используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [SetRuleOperation](setruleoperation.md) для изменения правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4f465-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-140">Description</span></span>

<span data-ttu-id="4f465-141">Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="4f465-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f465-142">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-142">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="4f465-143">Комментарии</span><span class="sxs-lookup"><span data-stu-id="4f465-143">Comments</span></span>

<span data-ttu-id="4f465-144">В этом примере изменяется отображаемое имя для «(изменено) это нежелательной».</span><span class="sxs-lookup"><span data-stu-id="4f465-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="4f465-145">Значения **Id** и **ChangeKey** атрибутов элемента [FolderId](folderid.md) URL были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="4f465-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="4f465-146">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="4f465-146">Request elements</span></span>

<span data-ttu-id="4f465-147">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4f465-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4f465-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4f465-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4f465-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4f465-150">Операции</span><span class="sxs-lookup"><span data-stu-id="4f465-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="4f465-151">Элемент [операции](operations.md) содержит элемент [SetRuleOperation](setruleoperation.md) для изменения правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="4f465-152">Пример ответа UpdateInboxRules (задать правила)</span><span class="sxs-lookup"><span data-stu-id="4f465-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4f465-153">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-153">Description</span></span>

<span data-ttu-id="4f465-154">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , обеспечивающий изменение правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4f465-155">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-155">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="4f465-156">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="4f465-156">Successful response elements</span></span>

<span data-ttu-id="4f465-157">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4f465-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f465-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4f465-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4f465-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4f465-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4f465-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4f465-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4f465-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="4f465-162">Пример запроса UpdateInboxRules (Удалить)</span><span class="sxs-lookup"><span data-stu-id="4f465-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="4f465-163">Можно использовать веб-служб Exchange для удаления правила папки «Входящие» в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f465-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4f465-164">Используйте совместно с элементом [DeleteRuleOperation](deleteruleoperation.md) [UpdateInboxRules](updateinboxrules.md) для удаления правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4f465-165">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-165">Description</span></span>

<span data-ttu-id="4f465-166">Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="4f465-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f465-167">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-167">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="4f465-168">Комментарии</span><span class="sxs-lookup"><span data-stu-id="4f465-168">Comments</span></span>

<span data-ttu-id="4f465-169">В этом примере удаляется существующий определенного правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="4f465-170">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="4f465-170">Request elements</span></span>

<span data-ttu-id="4f465-171">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4f465-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4f465-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4f465-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4f465-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4f465-174">Операции</span><span class="sxs-lookup"><span data-stu-id="4f465-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="4f465-175">Элемент [операции](operations.md) содержит элемент [DeleteRuleOperation](deleteruleoperation.md) удаление правила.</span><span class="sxs-lookup"><span data-stu-id="4f465-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="4f465-176">Пример ответа UpdateInboxRules (Удалить)</span><span class="sxs-lookup"><span data-stu-id="4f465-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4f465-177">Описание</span><span class="sxs-lookup"><span data-stu-id="4f465-177">Description</span></span>

<span data-ttu-id="4f465-178">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **UpdateInboxRules** , который удаляет правило.</span><span class="sxs-lookup"><span data-stu-id="4f465-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4f465-179">Программа</span><span class="sxs-lookup"><span data-stu-id="4f465-179">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="4f465-180">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="4f465-180">Successful response elements</span></span>

<span data-ttu-id="4f465-181">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4f465-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4f465-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f465-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4f465-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4f465-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4f465-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4f465-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4f465-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4f465-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="4f465-186">См. также</span><span class="sxs-lookup"><span data-stu-id="4f465-186">See also</span></span>



[<span data-ttu-id="4f465-187">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="4f465-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

