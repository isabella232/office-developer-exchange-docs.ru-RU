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
ms.openlocfilehash: f4c4c03f55c9f32be4a067024f4387888edd5fe9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457937"
---
# <a name="getinboxrules-operation"></a><span data-ttu-id="36709-103">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="36709-103">GetInboxRules operation</span></span>

<span data-ttu-id="36709-104">Операция **GetInboxRules** использует веб-службы Exchange для получения правил для папки "Входящие" в почтовом ящике определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="36709-104">The **GetInboxRules** operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.</span></span> 
  
## <a name="getinboxrules-request-example"></a><span data-ttu-id="36709-105">Пример запроса GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="36709-105">GetInboxRules request example</span></span>

### <a name="description"></a><span data-ttu-id="36709-106">Описание</span><span class="sxs-lookup"><span data-stu-id="36709-106">Description</span></span>

<span data-ttu-id="36709-107">В следующем примере показан XML-код запроса, который клиент отправляет на сервер.</span><span class="sxs-lookup"><span data-stu-id="36709-107">The following example shows the request XML that the client sends to the server.</span></span> <span data-ttu-id="36709-108">Запрос идентифицирует пользователя в элементе [маилбокссмтпаддресс](mailboxsmtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="36709-108">The request identifies the user in the [MailboxSmtpAddress](mailboxsmtpaddress.md) element.</span></span> <span data-ttu-id="36709-109">Все правила для папки "Входящие" для указанного пользователя возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="36709-109">All Inbox rules for the identified user are to be returned in the response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="36709-110">Код</span><span class="sxs-lookup"><span data-stu-id="36709-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

### <a name="request-elements"></a><span data-ttu-id="36709-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="36709-111">Request elements</span></span>

<span data-ttu-id="36709-112">Запрос включает следующий необязательный элемент:</span><span class="sxs-lookup"><span data-stu-id="36709-112">The request includes the following optional element:</span></span>
  
- [<span data-ttu-id="36709-113">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="36709-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a><span data-ttu-id="36709-114">Пример успешного ответа GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="36709-114">Successful GetInboxRules response example</span></span>

### <a name="description"></a><span data-ttu-id="36709-115">Описание</span><span class="sxs-lookup"><span data-stu-id="36709-115">Description</span></span>

<span data-ttu-id="36709-116">В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **GetInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="36709-116">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetInboxRules** request.</span></span> <span data-ttu-id="36709-117">В этом примере ответ включает одно правило.</span><span class="sxs-lookup"><span data-stu-id="36709-117">In this example, the response includes one rule.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="36709-118">Значения **ID** и атрибуты **чанжекэй** элемента [FolderId](folderid.md) были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36709-118">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="36709-119">Код</span><span class="sxs-lookup"><span data-stu-id="36709-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="response-elements"></a><span data-ttu-id="36709-120">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="36709-120">Response elements</span></span>

<span data-ttu-id="36709-121">В ответ включаются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36709-121">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="36709-122">жетинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="36709-122">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
    
- [<span data-ttu-id="36709-123">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="36709-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="36709-124">аутлукрулеблобексистс</span><span class="sxs-lookup"><span data-stu-id="36709-124">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
    
- [<span data-ttu-id="36709-125">инбоксрулес</span><span class="sxs-lookup"><span data-stu-id="36709-125">InboxRules</span></span>](inboxrules.md)
    
## <a name="see-also"></a><span data-ttu-id="36709-126">См. также</span><span class="sxs-lookup"><span data-stu-id="36709-126">See also</span></span>



[<span data-ttu-id="36709-127">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36709-127">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)

