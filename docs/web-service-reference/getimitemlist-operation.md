---
title: Операция GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Найдите сведения о веб-служб Exchange GetImItemList операции.
ms.openlocfilehash: 3977b0ad31e819cd973ce261ba3152b3840003b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762816"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="45982-103">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="45982-103">GetImItemList operation</span></span>

<span data-ttu-id="45982-104">Найдите сведения о **GetImItemList** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="45982-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="45982-105">С помощью операции GetImItemList</span><span class="sxs-lookup"><span data-stu-id="45982-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="45982-106">Операция **GetImItemList** показано получение списка групп мгновенного обмена мгновенными сообщениями и обмена мгновенными Сообщениями контактные действующие лица в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="45982-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="45982-107">Операция **GetImItemList** не имеет каких-либо аргументов.</span><span class="sxs-lookup"><span data-stu-id="45982-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="45982-108">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="45982-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="45982-109">Заголовки SOAP GetImItemList операции</span><span class="sxs-lookup"><span data-stu-id="45982-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="45982-110">Операция **GetImItemList** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="45982-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="45982-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="45982-111">**Header name**</span></span>|<span data-ttu-id="45982-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="45982-112">**Element**</span></span>|<span data-ttu-id="45982-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="45982-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="45982-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="45982-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="45982-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="45982-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="45982-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="45982-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="45982-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="45982-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="45982-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="45982-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="45982-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="45982-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="45982-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="45982-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="45982-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="45982-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="45982-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="45982-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="45982-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="45982-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="45982-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="45982-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="45982-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="45982-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="45982-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="45982-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="45982-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="45982-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="45982-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="45982-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="45982-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="45982-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="45982-130">Пример запроса GetImItemList операции: запрашивать список элементов обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="45982-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="45982-131">Приведенный ниже запрос операции **GetImItemList** показано, как запросить список групп обмена мгновенными Сообщениями и обмена мгновенными Сообщениями контактов пользователей в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="45982-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="45982-132">Элемент **GetImItemList** это единственный элемент в тексте запроса SOAP.</span><span class="sxs-lookup"><span data-stu-id="45982-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="45982-133">Запрос SOAP body содержит следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="45982-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="45982-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="45982-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="45982-135">Успешные операции ответа GetImItemList</span><span class="sxs-lookup"><span data-stu-id="45982-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="45982-136">В следующем примере показано успешного ответа на запрос операции **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="45982-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="45982-137">Ответ содержит четыре группы обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="45982-137">The response contains four IM groups.</span></span> <span data-ttu-id="45982-138">Из трех групп обмена мгновенными Сообщениями — другие контакты, метка и "Избранное" — это группы по умолчанию в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="45982-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="45982-139">Группа MyCustomGroup2 — настраиваемой группы, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="45982-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="45982-140">Группы «другие контакты» и «метка не имеют члены.</span><span class="sxs-lookup"><span data-stu-id="45982-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="45982-141">Группа "Избранное" имеет одного элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="45982-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="45982-142">MyCustomGroup2 имеет два элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="45982-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="45982-143">Идентификаторы элементов, предоставляются таким образом, последующие запросы **GetItem** , могут выполняться для получения дополнительных сведений о контактах обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="45982-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="45982-144">В этом примере возвращаются два пользователей.</span><span class="sxs-lookup"><span data-stu-id="45982-144">This example returns two personas.</span></span> <span data-ttu-id="45982-145">Первый он представляет двумя элементами контактов: Вадим Smith "и" Tony Smith.</span><span class="sxs-lookup"><span data-stu-id="45982-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="45982-146">Объединенный контактные данные возвращаются в объекте **пользователя** .</span><span class="sxs-lookup"><span data-stu-id="45982-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="45982-147">Второй он представляет один контакт с отображаемым именем Terence Adams.</span><span class="sxs-lookup"><span data-stu-id="45982-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="45982-148">Идентификаторы хранилища Exchange, идентификаторы элементов, идентификаторы источника, идентификаторы папок и идентификаторы пользователя URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="45982-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="45982-149">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="45982-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="45982-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="45982-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="45982-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="45982-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="45982-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="45982-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="45982-153">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="45982-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="45982-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="45982-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="45982-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="45982-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="45982-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="45982-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="45982-157">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="45982-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="45982-158">Действующие лица</span><span class="sxs-lookup"><span data-stu-id="45982-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="45982-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="45982-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="45982-160">PersonaType</span><span class="sxs-lookup"><span data-stu-id="45982-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="45982-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="45982-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="45982-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="45982-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="45982-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="45982-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="45982-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="45982-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="45982-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="45982-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="45982-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="45982-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="45982-167">Фамилия</span><span class="sxs-lookup"><span data-stu-id="45982-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="45982-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="45982-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="45982-169">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="45982-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="45982-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="45982-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="45982-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="45982-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="45982-172">ImAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="45982-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="45982-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="45982-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="45982-174">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="45982-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="45982-175">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="45982-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="45982-176">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="45982-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="45982-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="45982-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="45982-178">IsWritable</span><span class="sxs-lookup"><span data-stu-id="45982-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="45982-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="45982-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="45982-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="45982-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="45982-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="45982-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="45982-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="45982-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="45982-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="45982-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="45982-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="45982-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="45982-185">GivenNames</span><span class="sxs-lookup"><span data-stu-id="45982-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="45982-186">Фамилии</span><span class="sxs-lookup"><span data-stu-id="45982-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="45982-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="45982-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="45982-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="45982-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="45982-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="45982-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="45982-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="45982-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="45982-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="45982-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="45982-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="45982-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="45982-193">Значение (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="45982-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="45982-194">Ошибка операции GetImItemList ответа</span><span class="sxs-lookup"><span data-stu-id="45982-194">GetImItemList operation error response</span></span>

<span data-ttu-id="45982-195">В следующем примере показано ошибочный ответ на запрос операции **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="45982-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="45982-196">Это ответ на запрос, который содержит версию неправильные запрошенный сервер в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="45982-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="45982-197">Эта ошибка ответа — это ошибки SOAP и не представлено в схеме веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="45982-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="45982-198">См. также</span><span class="sxs-lookup"><span data-stu-id="45982-198">See also</span></span>

- [<span data-ttu-id="45982-199">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="45982-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="45982-200">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="45982-200">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="45982-201">Операция GetImItems</span><span class="sxs-lookup"><span data-stu-id="45982-201">GetImItems operation</span></span>](getimitems-operation.md)
    

