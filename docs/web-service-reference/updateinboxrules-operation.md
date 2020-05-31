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
# <a name="updateinboxrules-operation"></a><span data-ttu-id="b5feb-104">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="b5feb-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="b5feb-105">Операция UpdateInboxRules обновляет правила папки "Входящие" пользователя, прошедшего проверку подлинности, применяя указанные операции.</span><span class="sxs-lookup"><span data-stu-id="b5feb-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="b5feb-106">**UpdateInboxRules** используется для создания правила папки "Входящие", установки правила для папки "Входящие" или удаления правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="b5feb-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="b5feb-107">При использовании операции **UpdateInboxRules** веб-службы Exchange удаляют правила отправки на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="b5feb-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="b5feb-108">Правила отправки на стороне клиента хранятся в клиенте в сообщении о связанной папке правила (ФАИ), но не в других.</span><span class="sxs-lookup"><span data-stu-id="b5feb-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="b5feb-109">По умолчанию служба EWS удаляет это правило ФАИ по умолчанию, в зависимости от того, что Outlook будет воссоздать его.</span><span class="sxs-lookup"><span data-stu-id="b5feb-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="b5feb-110">Однако Outlook не может создавать правила, которые не существуют как расширенное правило, а правила отправки на стороне клиента не являются расширенными правилами.</span><span class="sxs-lookup"><span data-stu-id="b5feb-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="b5feb-111">В результате эти правила теряются.</span><span class="sxs-lookup"><span data-stu-id="b5feb-111">As a result, these rules are lost.</span></span> <span data-ttu-id="b5feb-112">Мы рекомендуем использовать это при проектировании решения.</span><span class="sxs-lookup"><span data-stu-id="b5feb-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="b5feb-113">Пример запроса UpdateInboxRules (Create Rule)</span><span class="sxs-lookup"><span data-stu-id="b5feb-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="b5feb-114">Вы можете использовать веб-службы Exchange, чтобы создать правило для папки "Входящие" в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5feb-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="b5feb-115">Чтобы создать правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [креатерулеоператион](createruleoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="b5feb-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="b5feb-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-116">Description</span></span>

<span data-ttu-id="b5feb-117">Клиент создает XML-код запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="b5feb-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="b5feb-118">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-118">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="b5feb-119">Comments</span><span class="sxs-lookup"><span data-stu-id="b5feb-119">Comments</span></span>

<span data-ttu-id="b5feb-120">В этом примере создается правило, которое переместит сообщение электронной почты в папку нежелательной почты, если тема сообщения содержит строку, содержательную "интересное".</span><span class="sxs-lookup"><span data-stu-id="b5feb-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="b5feb-121">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="b5feb-121">Request elements</span></span>

<span data-ttu-id="b5feb-122">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="b5feb-123">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="b5feb-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="b5feb-124">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="b5feb-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="b5feb-125">Operations</span><span class="sxs-lookup"><span data-stu-id="b5feb-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="b5feb-126">Элемент [Operations](operations.md) содержит элемент [креатерулеоператион](createruleoperation.md) для создания правила.</span><span class="sxs-lookup"><span data-stu-id="b5feb-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="b5feb-127">Пример отклика UpdateInboxRules (Create Rule)</span><span class="sxs-lookup"><span data-stu-id="b5feb-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="b5feb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-128">Description</span></span>

<span data-ttu-id="b5feb-129">В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который создает правило.</span><span class="sxs-lookup"><span data-stu-id="b5feb-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b5feb-130">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-130">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="b5feb-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="b5feb-131">Successful response elements</span></span>

<span data-ttu-id="b5feb-132">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b5feb-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b5feb-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b5feb-134">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="b5feb-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="b5feb-135">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b5feb-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b5feb-136">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b5feb-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="b5feb-137">Пример запроса UpdateInboxRules (Set Rule)</span><span class="sxs-lookup"><span data-stu-id="b5feb-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="b5feb-138">Вы можете использовать веб-службы Exchange для изменения правила папки "Входящие" в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5feb-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="b5feb-139">Чтобы изменить правило, используйте элемент [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [сетрулеоператион](setruleoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="b5feb-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="b5feb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-140">Description</span></span>

<span data-ttu-id="b5feb-141">Клиент создает XML-код запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="b5feb-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="b5feb-142">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-142">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="b5feb-143">Comments</span><span class="sxs-lookup"><span data-stu-id="b5feb-143">Comments</span></span>

<span data-ttu-id="b5feb-144">В этом примере показано изменение отображаемого имени на "(изменено) это нежелательное".</span><span class="sxs-lookup"><span data-stu-id="b5feb-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="b5feb-145">Значения атрибутов **ID** и **чанжекэй** элемента [FolderId](folderid.md) сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5feb-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b5feb-146">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="b5feb-146">Request elements</span></span>

<span data-ttu-id="b5feb-147">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="b5feb-148">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="b5feb-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="b5feb-149">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="b5feb-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="b5feb-150">Operations</span><span class="sxs-lookup"><span data-stu-id="b5feb-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="b5feb-151">Элемент [Operations](operations.md) содержит элемент [сетрулеоператион](setruleoperation.md) для изменения правила.</span><span class="sxs-lookup"><span data-stu-id="b5feb-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="b5feb-152">Пример отклика UpdateInboxRules (Set Rule)</span><span class="sxs-lookup"><span data-stu-id="b5feb-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="b5feb-153">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-153">Description</span></span>

<span data-ttu-id="b5feb-154">В следующем примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который изменяет правило.</span><span class="sxs-lookup"><span data-stu-id="b5feb-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b5feb-155">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-155">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="b5feb-156">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="b5feb-156">Successful response elements</span></span>

<span data-ttu-id="b5feb-157">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b5feb-158">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b5feb-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b5feb-159">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="b5feb-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="b5feb-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b5feb-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b5feb-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b5feb-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="b5feb-162">Пример запроса UpdateInboxRules (Delete Rule)</span><span class="sxs-lookup"><span data-stu-id="b5feb-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="b5feb-163">Вы можете использовать веб-службы Exchange для удаления правила папки "Входящие" в почтовом ящике пользователя в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5feb-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="b5feb-164">Чтобы удалить правило, используйте [UpdateInboxRules](updateinboxrules.md) в сочетании с элементом [делетерулеоператион](deleteruleoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="b5feb-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="b5feb-165">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-165">Description</span></span>

<span data-ttu-id="b5feb-166">Клиент создает XML-код запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="b5feb-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="b5feb-167">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-167">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="b5feb-168">Comments</span><span class="sxs-lookup"><span data-stu-id="b5feb-168">Comments</span></span>

<span data-ttu-id="b5feb-169">В этом примере удаляется существующее идентифицированное правило.</span><span class="sxs-lookup"><span data-stu-id="b5feb-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="b5feb-170">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="b5feb-170">Request elements</span></span>

<span data-ttu-id="b5feb-171">Запрос **UpdateInboxRules** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="b5feb-172">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="b5feb-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="b5feb-173">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="b5feb-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="b5feb-174">Operations</span><span class="sxs-lookup"><span data-stu-id="b5feb-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="b5feb-175">Элемент [Operations](operations.md) содержит элемент [делетерулеоператион](deleteruleoperation.md) для удаления правила.</span><span class="sxs-lookup"><span data-stu-id="b5feb-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="b5feb-176">Пример отклика UpdateInboxRules (удаление правила)</span><span class="sxs-lookup"><span data-stu-id="b5feb-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="b5feb-177">Описание</span><span class="sxs-lookup"><span data-stu-id="b5feb-177">Description</span></span>

<span data-ttu-id="b5feb-178">В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **UpdateInboxRules** , который удаляет правило.</span><span class="sxs-lookup"><span data-stu-id="b5feb-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b5feb-179">Код</span><span class="sxs-lookup"><span data-stu-id="b5feb-179">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="b5feb-180">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="b5feb-180">Successful response elements</span></span>

<span data-ttu-id="b5feb-181">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b5feb-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b5feb-182">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b5feb-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b5feb-183">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="b5feb-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="b5feb-184">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b5feb-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b5feb-185">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b5feb-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="b5feb-186">См. также</span><span class="sxs-lookup"><span data-stu-id="b5feb-186">See also</span></span>



[<span data-ttu-id="b5feb-187">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="b5feb-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

