---
title: Операция GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: Операция делегируемый извлекает параметры делегирования для указанного почтового ящика.
ms.openlocfilehash: 400bf5d1cafcbb789aaa749c62c7a908622d4ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461067"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="e94d1-103">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="e94d1-103">GetDelegate operation</span></span>

<span data-ttu-id="e94d1-104">Операция **делегируемый** извлекает параметры делегирования для указанного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e94d1-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="e94d1-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="e94d1-105">SOAP Headers</span></span>

<span data-ttu-id="e94d1-106">Операция **Delegate** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="e94d1-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="e94d1-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="e94d1-107">**Header**</span></span>|<span data-ttu-id="e94d1-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e94d1-108">**Element**</span></span>|<span data-ttu-id="e94d1-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e94d1-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e94d1-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="e94d1-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="e94d1-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="e94d1-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e94d1-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="e94d1-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="e94d1-113">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="e94d1-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="e94d1-114">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="e94d1-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e94d1-115">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="e94d1-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="e94d1-116">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="e94d1-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="e94d1-117">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="e94d1-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e94d1-118">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="e94d1-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="e94d1-119">серверверсион</span><span class="sxs-lookup"><span data-stu-id="e94d1-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="e94d1-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="e94d1-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e94d1-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="e94d1-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="e94d1-122">Пример запроса для делегата.</span><span class="sxs-lookup"><span data-stu-id="e94d1-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="e94d1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e94d1-123">Description</span></span>

<span data-ttu-id="e94d1-124">В приведенном ниже примере кода показано, как получить параметры делегата для всех делегатов, заданные в почтовом ящике user3's.</span><span class="sxs-lookup"><span data-stu-id="e94d1-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="e94d1-125">Все разрешения для каждого пользователя возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="e94d1-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="e94d1-126">Код</span><span class="sxs-lookup"><span data-stu-id="e94d1-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e94d1-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="e94d1-127">Comments</span></span>

<span data-ttu-id="e94d1-128">Вы можете использовать элемент [UserID](userid.md) , чтобы указать отдельных пользователей, вместо того чтобы возвращать всех пользователей, имеющих разрешения на доступ представителя в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e94d1-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e94d1-129">Веб-службы Exchange (EWS) не поддерживают управление представителями групп.</span><span class="sxs-lookup"><span data-stu-id="e94d1-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="e94d1-130">При вызове операции- **делегата** для субъекта, имеющего делегата группы безопасности, EWS возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="e94d1-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="e94d1-131">Пример ответа для делегата GetResponse</span><span class="sxs-lookup"><span data-stu-id="e94d1-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="e94d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e94d1-132">Description</span></span>

<span data-ttu-id="e94d1-133">Ниже приведен пример отклика **GetResponse, в котором показан** успешный ответ на запрос с помощью **делегата** .</span><span class="sxs-lookup"><span data-stu-id="e94d1-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="e94d1-134">Ответ содержит сведения о разрешениях для делегированного доступа, будь то делегат может просматривать частные элементы, независимо от того, получает ли представитель копии сообщений о собраниях и кому были доставлены приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="e94d1-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e94d1-135">Код</span><span class="sxs-lookup"><span data-stu-id="e94d1-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:GetDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="e94d1-136">См. также</span><span class="sxs-lookup"><span data-stu-id="e94d1-136">See also</span></span>



- [<span data-ttu-id="e94d1-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e94d1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

