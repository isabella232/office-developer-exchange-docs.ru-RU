---
title: Операция GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Поиск сведений о GetImItemListной операции EWS.
ms.openlocfilehash: aabe84054b93e7de8af6145942493a0224932e45
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456068"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="5b1e9-103">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-103">GetImItemList operation</span></span>

<span data-ttu-id="5b1e9-104">Поиск сведений о **GetImItemListной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="5b1e9-105">Использование операции GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="5b1e9-106">Операция **GetImItemList** извлекает список групп мгновенных сообщений и пользователей контактов для обмена мгновенными сообщениями в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="5b1e9-107">Операция **GetImItemList** не имеет аргументов.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="5b1e9-108">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="5b1e9-109">Заголовки SOAP операции GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="5b1e9-110">Операция **GetImItemList** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5b1e9-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-111">**Header name**</span></span>|<span data-ttu-id="5b1e9-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-112">**Element**</span></span>|<span data-ttu-id="5b1e9-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5b1e9-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5b1e9-115">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="5b1e9-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5b1e9-116">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5b1e9-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b1e9-118">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5b1e9-119">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="5b1e9-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5b1e9-120">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5b1e9-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b1e9-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5b1e9-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="5b1e9-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5b1e9-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5b1e9-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b1e9-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="5b1e9-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5b1e9-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="5b1e9-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5b1e9-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5b1e9-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="5b1e9-130">Пример запроса операции GetImItemList: запрос списка элементов для обмена мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="5b1e9-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="5b1e9-131">В следующем примере запроса операции **GetImItemList** показано, как запросить список групп IM и пользователей контактов для обмена мгновенными сообщениями в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="5b1e9-132">Элемент **GetImItemList** является единственным параметром element в теле SOAP.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5b1e9-133">Текст SOAP запроса содержит следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="5b1e9-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="5b1e9-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="5b1e9-135">Успешный отклик операции GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="5b1e9-136">В следующем примере показан успешный ответ на запрос операции **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="5b1e9-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="5b1e9-137">Ответ содержит четыре группы для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-137">The response contains four IM groups.</span></span> <span data-ttu-id="5b1e9-138">Три группы для обмена мгновенными сообщениями — другие контакты, размеченные Теги и Избранное — это группы по умолчанию в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="5b1e9-139">Группа MyCustomGroup2 — это пользовательская группа, созданная пользователем.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="5b1e9-140">Другие контакты и группы с тегами не имеют членов.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="5b1e9-141">Группа "Избранное" имеет одного участника контакта.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="5b1e9-142">У MyCustomGroup2 есть два контакта.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="5b1e9-143">Идентификаторы элементов предоставляются таким образом, что для получения дополнительных сведений о контактах для обмена мгновенными сообщениями можно выполнить последующие запросы **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="5b1e9-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="5b1e9-144">В этом примере возвращаются два пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-144">This example returns two personas.</span></span> <span data-ttu-id="5b1e9-145">Первый персонаж представляет два элемента контактов: Ансони Смит и Tony Смит.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="5b1e9-146">В объекте **персоны** возвращается Объединенная Контактная информация.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="5b1e9-147">Второй персонаж представляет один контакт с отображаемым именем Теренце Adams.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5b1e9-148">Идентификаторы хранилища Exchange, идентификаторы элементов, идентификаторы источников, идентификаторы папок и идентификаторы пользователей были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Other Contacts</DisplayName>
                  <GroupType>IPM.DistList.MOC.OtherContacts</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLThQoTbWAAAAAAQUAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Tagged</DisplayName>
                  <GroupType>IPM.DistList.MOC.Tagged</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJAAQTAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Favorites</DisplayName>
                  <GroupType>IPM.DistList.MOC.Favorites</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTAAAAAQSAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1MjJtt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
               <ImGroup>
                  <DisplayName>MyCustomGroup2</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjKAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1Matt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                     <ItemId Id="AAMkAGQ1MjJjMTBkTbWAAAAAAveAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4YkZmRkYQAQAFgxE1nBcqRGgYWWorM9/+s=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-12T22:14:36Z</CreationTime>
                  <DisplayName>Anthony Smith</DisplayName>
                  <DisplayNameFirstLast>Anthony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Smith Anthony</DisplayNameLastFirst>
                  <FileAs>Smith, Anthony</FileAs>
                  <FileAsId>LastCommaFirst</FileAsId>
                  <GivenName>Anthony</GivenName>
                  <Surname>Smith</Surname>
                  <EmailAddress>
                     <Name>tsmith@contoso.com</Name>
                     <EmailAddress>tsmith@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>tsmith@contoso.com</Name>
                        <EmailAddress>tsmith@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AQMkAGQ1MjIAYzEwZC03OGNlLTQ5Bq239uFChNtYAAAIvDAAAAA==" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAADB3" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>false</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AQMkAGQ1MjIAYzEMikE3AQBtF8oI7iVOQatt/bhQoTbWAAADEAAAAA==" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                     <Attribution>
                        <Id>1</Id>
                        <SourceId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04/bhQoTbWAAAAAAveAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAym" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Qatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Anthony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAses>
                     <StringAttributedValue>
                        <Value>Smith, Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAses>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>LastCommaFirst</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <GivenNames>
                     <StringAttributedValue>
                        <Value>Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </GivenNames>
                  <Surnames>
                     <StringAttributedValue>
                        <Value>Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </Surnames>
                  <HomePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550110</Number>
                           <Type>Home</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </HomePhones>
                  <MobilePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550120</Number>
                           <Type>Mobile</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </MobilePhones>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>tsmith@contoso.com</Name>
                           <EmailAddress>tsmith@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLkYQAQAJ3EkhEEXN5KufGbSYJanZk=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-05T23:06:58Z</CreationTime>
                  <DisplayName>Terence Adams</DisplayName>
                  <DisplayNameFirstLast>Terence Adams</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Terence Adams</DisplayNameLastFirst>
                  <FileAsId>None</FileAsId>
                  <EmailAddress>
                     <Name>Terence Adams</Name>
                     <EmailAddress>tadams@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>Terence Adams</Name>
                        <EmailAddress>tadams@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tadams@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkAGQ1MjVOQatt/bhQoTbWAAAA7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAyg" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2rBtF8oI7iVOQatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Terence Adams</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>Terence Adams</Name>
                           <EmailAddress>tadams@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tadams@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5b1e9-149">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5b1e9-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b1e9-150">жетимитемлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="5b1e9-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="5b1e9-151">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5b1e9-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5b1e9-152">имитемлист</span><span class="sxs-lookup"><span data-stu-id="5b1e9-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="5b1e9-153">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5b1e9-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="5b1e9-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="5b1e9-155">ексчанжестореид</span><span class="sxs-lookup"><span data-stu-id="5b1e9-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="5b1e9-156">мемберкоррелатионкэй</span><span class="sxs-lookup"><span data-stu-id="5b1e9-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="5b1e9-157">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5b1e9-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5b1e9-158">Фиктивные пользователи</span><span class="sxs-lookup"><span data-stu-id="5b1e9-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5b1e9-159">персонаид</span><span class="sxs-lookup"><span data-stu-id="5b1e9-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="5b1e9-160">персонатипе</span><span class="sxs-lookup"><span data-stu-id="5b1e9-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="5b1e9-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="5b1e9-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="5b1e9-162">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="5b1e9-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="5b1e9-163">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="5b1e9-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="5b1e9-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="5b1e9-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="5b1e9-165">филеасид</span><span class="sxs-lookup"><span data-stu-id="5b1e9-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="5b1e9-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="5b1e9-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="5b1e9-167">ФИО</span><span class="sxs-lookup"><span data-stu-id="5b1e9-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="5b1e9-168">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="5b1e9-169">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="5b1e9-170">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="5b1e9-171">EmailAddresses (Аррайофемаиладдрессестипе)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="5b1e9-172">Адрес (String)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="5b1e9-173">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="5b1e9-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="5b1e9-174">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="5b1e9-175">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="5b1e9-176">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="5b1e9-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="5b1e9-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="5b1e9-178">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="5b1e9-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="5b1e9-179">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="5b1e9-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="5b1e9-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="5b1e9-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="5b1e9-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="5b1e9-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5b1e9-182">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="5b1e9-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="5b1e9-183">филеасес</span><span class="sxs-lookup"><span data-stu-id="5b1e9-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="5b1e9-184">филеасидс</span><span class="sxs-lookup"><span data-stu-id="5b1e9-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="5b1e9-185">гивеннамес</span><span class="sxs-lookup"><span data-stu-id="5b1e9-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="5b1e9-186">Фамилии</span><span class="sxs-lookup"><span data-stu-id="5b1e9-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="5b1e9-187">хомефонес</span><span class="sxs-lookup"><span data-stu-id="5b1e9-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="5b1e9-188">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="5b1e9-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="5b1e9-189">мобилефонес</span><span class="sxs-lookup"><span data-stu-id="5b1e9-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="5b1e9-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="5b1e9-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="5b1e9-191">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="5b1e9-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="5b1e9-192">Адреса</span><span class="sxs-lookup"><span data-stu-id="5b1e9-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="5b1e9-193">Значение (Екстендедпропертитипе)</span><span class="sxs-lookup"><span data-stu-id="5b1e9-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="5b1e9-194">Ответ об ошибке операции GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b1e9-194">GetImItemList operation error response</span></span>

<span data-ttu-id="5b1e9-195">В следующем примере показан ответ об ошибке для запроса операции **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="5b1e9-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="5b1e9-196">Это ответ на запрос, который содержит неверную версию запрошенного сервера в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="5b1e9-197">Этот ошибочный ответ является причиной сбоя SOAP и не представлен в схеме EWS.</span><span class="sxs-lookup"><span data-stu-id="5b1e9-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5b1e9-198">См. также</span><span class="sxs-lookup"><span data-stu-id="5b1e9-198">See also</span></span>

- [<span data-ttu-id="5b1e9-199">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="5b1e9-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="5b1e9-200">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="5b1e9-200">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="5b1e9-201">Операция GetImItems</span><span class="sxs-lookup"><span data-stu-id="5b1e9-201">GetImItems operation</span></span>](getimitems-operation.md)
    

