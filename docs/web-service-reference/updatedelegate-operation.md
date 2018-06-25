---
title: Операция UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: 03f618ac-ad1a-4772-9b81-c5bb0f12d6ab
description: Операция UpdateDelegate обновляет делегированных разрешений на почтовый ящик участника.
ms.openlocfilehash: 9f69d784617d10d8902a260bbf6639703dd33b6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840317"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="38a6b-103">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="38a6b-103">UpdateDelegate operation</span></span>

<span data-ttu-id="38a6b-104">Операция **UpdateDelegate** обновляет делегированных разрешений на почтовый ящик участника.</span><span class="sxs-lookup"><span data-stu-id="38a6b-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="38a6b-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="38a6b-105">SOAP Headers</span></span>

<span data-ttu-id="38a6b-106">Операция **UpdateDelegate** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="38a6b-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="38a6b-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="38a6b-107">**Header**</span></span>|<span data-ttu-id="38a6b-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38a6b-108">**Element**</span></span>|<span data-ttu-id="38a6b-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38a6b-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38a6b-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="38a6b-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="38a6b-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="38a6b-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="38a6b-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="38a6b-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="38a6b-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="38a6b-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="38a6b-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="38a6b-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="38a6b-115">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="38a6b-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="38a6b-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="38a6b-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="38a6b-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="38a6b-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="38a6b-118">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="38a6b-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="38a6b-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="38a6b-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="38a6b-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="38a6b-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="38a6b-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="38a6b-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="38a6b-122">Пример запроса UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="38a6b-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="38a6b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="38a6b-123">Description</span></span>

<span data-ttu-id="38a6b-124">Приведенный ниже запрос **UpdateDelegate** показано, как обновить делегированных разрешений для учетной записи пользователя user1.</span><span class="sxs-lookup"><span data-stu-id="38a6b-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="38a6b-125">Пользователь2 получает нет разрешений на уровне папки задач и предоставляется разрешение на просмотр частных элементов.</span><span class="sxs-lookup"><span data-stu-id="38a6b-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="38a6b-126">User3 предоставляется разрешения для папки журнала.</span><span class="sxs-lookup"><span data-stu-id="38a6b-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="38a6b-127">Приглашения на собрания, передаются в делегаты и сведения о запросе на отправляется User1.</span><span class="sxs-lookup"><span data-stu-id="38a6b-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38a6b-128">Программа</span><span class="sxs-lookup"><span data-stu-id="38a6b-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ViewPrivateItems>true</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user3@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:JournalFolderPermissionLevel>Reviewer</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndSendInformationToMe</DeliverMeetingRequests>
    </UpdateDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="38a6b-129">Комментарии</span><span class="sxs-lookup"><span data-stu-id="38a6b-129">Comments</span></span>

<span data-ttu-id="38a6b-130">Запрос [UpdateDelegate](updatedelegate.md) не требует применения обновления к делегатам.</span><span class="sxs-lookup"><span data-stu-id="38a6b-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="38a6b-131">Клиенты могут изменить только значение параметра **DeliverMeetingMessage** .</span><span class="sxs-lookup"><span data-stu-id="38a6b-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="38a6b-132">Пример ответа UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="38a6b-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="38a6b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="38a6b-133">Description</span></span>

<span data-ttu-id="38a6b-134">В следующем примере показано успешные ответ на операцию **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="38a6b-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38a6b-135">Программа</span><span class="sxs-lookup"><span data-stu-id="38a6b-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1117</t:SID>
              <t:PrimarySmtpAddress>User2@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User2</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>true</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
              <t:PrimarySmtpAddress>User3@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User3</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="38a6b-136">Пример ответа об ошибке UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="38a6b-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="38a6b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="38a6b-137">Description</span></span>

<span data-ttu-id="38a6b-138">В следующем примере показано ошибочный ответ на запрос **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="38a6b-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="38a6b-139">Произошла ошибка, так как делегат не существует в списке делегата участника.</span><span class="sxs-lookup"><span data-stu-id="38a6b-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38a6b-140">Программа</span><span class="sxs-lookup"><span data-stu-id="38a6b-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="38a6b-141">См. также</span><span class="sxs-lookup"><span data-stu-id="38a6b-141">See also</span></span>



- [<span data-ttu-id="38a6b-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38a6b-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

