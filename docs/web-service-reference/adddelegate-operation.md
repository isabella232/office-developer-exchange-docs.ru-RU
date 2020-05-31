---
title: Операция AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: Операция AddDelegate добавляет одного или нескольких делегатов в почтовый ящик участника и задает конкретные разрешения на доступ.
ms.openlocfilehash: 28d4ded2625efc3d6eade44f5fafc06c2ffca7ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761333"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="b78de-103">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b78de-103">AddDelegate operation</span></span>

<span data-ttu-id="b78de-104">Операция **AddDelegate** добавляет одного или нескольких делегатов в почтовый ящик участника и задает конкретные разрешения на доступ.</span><span class="sxs-lookup"><span data-stu-id="b78de-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="b78de-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="b78de-105">SOAP headers</span></span>

<span data-ttu-id="b78de-106">Операция **AddDelegate** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b78de-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="b78de-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="b78de-107">**Header**</span></span>|<span data-ttu-id="b78de-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b78de-108">**Element**</span></span>|<span data-ttu-id="b78de-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b78de-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b78de-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="b78de-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="b78de-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="b78de-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b78de-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="b78de-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="b78de-113">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b78de-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="b78de-114">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b78de-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b78de-115">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b78de-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="b78de-116">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="b78de-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="b78de-117">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b78de-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b78de-118">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b78de-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="b78de-119">серверверсион</span><span class="sxs-lookup"><span data-stu-id="b78de-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="b78de-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b78de-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b78de-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b78de-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="b78de-122">Пример запроса AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b78de-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="b78de-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b78de-123">Description</span></span>

<span data-ttu-id="b78de-124">В приведенном ниже примере запроса **AddDelegate** показана попытка предоставить представителю User1 разрешения на делегирование папок, владельцем которых является Пользователь2.</span><span class="sxs-lookup"><span data-stu-id="b78de-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="b78de-125">Пользователю User1 предоставляются разрешения на уровне автора для папки календаря user2's и разрешения на уровне просмотра для папки контактов user2's.</span><span class="sxs-lookup"><span data-stu-id="b78de-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="b78de-126">Пользователь1 не будет получать копии сообщений о собраниях и не сможет просматривать частные элементы в почтовом ящике user2's.</span><span class="sxs-lookup"><span data-stu-id="b78de-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="b78de-127">Приглашения на собрания будут отправляться как в Пользователь1, так и в Пользователь2.</span><span class="sxs-lookup"><span data-stu-id="b78de-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b78de-128">Код</span><span class="sxs-lookup"><span data-stu-id="b78de-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <AddDelegate>
      <Mailbox>
        <t:EmailAddress>user2@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user1@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndMe</DeliverMeetingRequests>
    </AddDelegate>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-response-example"></a><span data-ttu-id="b78de-129">Пример отклика AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b78de-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="b78de-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b78de-130">Description</span></span>

<span data-ttu-id="b78de-131">В приведенном ниже примере ответа **AddDelegate** показано, как успешно ответить на запрос **AddDelegate** .</span><span class="sxs-lookup"><span data-stu-id="b78de-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b78de-132">Код</span><span class="sxs-lookup"><span data-stu-id="b78de-132">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="b78de-133">Пример ответа на сообщение об ошибке AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b78de-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="b78de-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b78de-134">Description</span></span>

<span data-ttu-id="b78de-135">В следующем примере показан ответ на запрос на добавление делегата, который уже был добавлен в почтовый ящик субъекта.</span><span class="sxs-lookup"><span data-stu-id="b78de-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="b78de-136">Код</span><span class="sxs-lookup"><span data-stu-id="b78de-136">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b78de-137">Comments</span><span class="sxs-lookup"><span data-stu-id="b78de-137">Comments</span></span>

<span data-ttu-id="b78de-138">Если при попытке добавить делегата возвращается код ответа Еррорделегатеалреадексистс, используйте [операцию](getdelegate-operation.md) GetResponse для получения всех текущих разрешений для делегата, а затем используйте [операцию UpdateDelegate](updatedelegate-operation.md) для установки новых разрешений.</span><span class="sxs-lookup"><span data-stu-id="b78de-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b78de-139">См. также</span><span class="sxs-lookup"><span data-stu-id="b78de-139">See also</span></span>

- [<span data-ttu-id="b78de-140">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="b78de-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

