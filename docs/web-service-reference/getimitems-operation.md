---
title: Операция GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Поиск сведений о GetImItemsной операции EWS.
ms.openlocfilehash: 960f4683dd478b0e5f8cf18fa8d1593b7433a249
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456047"
---
# <a name="getimitems-operation"></a><span data-ttu-id="36fd1-103">Операция GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-103">GetImItems operation</span></span>

<span data-ttu-id="36fd1-104">Поиск сведений о **GetImItemsной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="36fd1-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="36fd1-105">Операция **GetImItems** получает сведения о группах обмена мгновенными сообщениями и пользователях контактов для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="36fd1-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="36fd1-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36fd1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="36fd1-107">Использование операции GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-107">Using the GetImItems operation</span></span>

<span data-ttu-id="36fd1-108">Операция **GetImItems** принимает идентификаторы элементов Group и Contact и возвращает набор сведений о группах и контактах.</span><span class="sxs-lookup"><span data-stu-id="36fd1-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="36fd1-109">Наборы свойств, возвращаемые в ответе, идентифицируются с помощью расширенных свойств, нескольких идентификаторов контакта, идентификаторов групп и определений расширенных свойств в качестве аргументов.</span><span class="sxs-lookup"><span data-stu-id="36fd1-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="36fd1-110">Заголовки SOAP операции GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="36fd1-111">Операция **GetImItems** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="36fd1-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="36fd1-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="36fd1-112">**Header name**</span></span>|<span data-ttu-id="36fd1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36fd1-113">**Element**</span></span>|<span data-ttu-id="36fd1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36fd1-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="36fd1-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="36fd1-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="36fd1-116">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="36fd1-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="36fd1-117">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="36fd1-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="36fd1-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="36fd1-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="36fd1-119">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="36fd1-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="36fd1-120">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="36fd1-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="36fd1-121">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="36fd1-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="36fd1-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="36fd1-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="36fd1-123">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="36fd1-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="36fd1-124">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="36fd1-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="36fd1-125">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="36fd1-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="36fd1-126">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="36fd1-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="36fd1-127">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="36fd1-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="36fd1-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="36fd1-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="36fd1-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="36fd1-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="36fd1-130">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="36fd1-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="36fd1-131">Пример запроса операции GetImItems: получение подробных сведений о контактах и группах для обмена мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="36fd1-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="36fd1-132">В следующем примере запроса операции **GetImItems** показано, как запросить подробные сведения о контактах и группах для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="36fd1-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="36fd1-133">Операция **GetImItems** может запросить один или несколько сведений о контакте или группе.</span><span class="sxs-lookup"><span data-stu-id="36fd1-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="36fd1-134">Вы также можете использовать расширенные свойства для получения настраиваемых свойств для групп и контактов.</span><span class="sxs-lookup"><span data-stu-id="36fd1-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="36fd1-135">Если запрошенное расширенное свойство не существует для элемента, то ответ будет игнорировать запрошенное свойство и возвращать ответ для набора свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="36fd1-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="36fd1-136">В этом примере показано, как получить отображаемое имя с помощью расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="36fd1-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="36fd1-137">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="36fd1-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="36fd1-138">Обратите внимание, что для этой операции в службе игнорируются ключи изменений.</span><span class="sxs-lookup"><span data-stu-id="36fd1-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="36fd1-139">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36fd1-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="36fd1-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="36fd1-141">контактидс</span><span class="sxs-lookup"><span data-stu-id="36fd1-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="36fd1-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="36fd1-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="36fd1-143">граупидс</span><span class="sxs-lookup"><span data-stu-id="36fd1-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="36fd1-144">Екстендедпропертиес (Нонемптяррайофекстендедфиелдурис)</span><span class="sxs-lookup"><span data-stu-id="36fd1-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="36fd1-145">ExtendedProperty (Пастоекстендедфиелдтипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="36fd1-146">Успешный отклик операции GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="36fd1-147">В следующем примере показан успешный ответ на запрос **GetImItems** для получения контакта и группы для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="36fd1-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="36fd1-148">Отображаемое имя запрашивается в расширенном свойстве.</span><span class="sxs-lookup"><span data-stu-id="36fd1-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="36fd1-149">Контакты для обмена мгновенными сообщениями возвращаются в виде пользователя.</span><span class="sxs-lookup"><span data-stu-id="36fd1-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
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
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="36fd1-150">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36fd1-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="36fd1-151">жетимитемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="36fd1-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="36fd1-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="36fd1-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="36fd1-153">имитемлист</span><span class="sxs-lookup"><span data-stu-id="36fd1-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="36fd1-154">Groups (Аррайофимграуптипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="36fd1-155">Группа</span><span class="sxs-lookup"><span data-stu-id="36fd1-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="36fd1-156">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="36fd1-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="36fd1-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="36fd1-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="36fd1-158">ексчанжестореид</span><span class="sxs-lookup"><span data-stu-id="36fd1-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="36fd1-159">мемберкоррелатионкэй</span><span class="sxs-lookup"><span data-stu-id="36fd1-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="36fd1-160">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="36fd1-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="36fd1-161">Екстендедпропертиес (Нонемптяррайофекстендедфиелдурис)</span><span class="sxs-lookup"><span data-stu-id="36fd1-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="36fd1-162">ExtendedProperty (Пастоекстендедфиелдтипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="36fd1-163">Фиктивные пользователи</span><span class="sxs-lookup"><span data-stu-id="36fd1-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="36fd1-164">персонаид</span><span class="sxs-lookup"><span data-stu-id="36fd1-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="36fd1-165">персонатипе</span><span class="sxs-lookup"><span data-stu-id="36fd1-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="36fd1-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="36fd1-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="36fd1-167">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="36fd1-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="36fd1-168">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="36fd1-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="36fd1-169">FileAs</span><span class="sxs-lookup"><span data-stu-id="36fd1-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="36fd1-170">[Филеасид](fileasid.md) филеасид</span><span class="sxs-lookup"><span data-stu-id="36fd1-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="36fd1-171">Адрес (String)</span><span class="sxs-lookup"><span data-stu-id="36fd1-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="36fd1-172">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="36fd1-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="36fd1-173">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="36fd1-174">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="36fd1-175">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="36fd1-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="36fd1-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="36fd1-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="36fd1-177">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="36fd1-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="36fd1-178">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="36fd1-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="36fd1-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="36fd1-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="36fd1-180">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="36fd1-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="36fd1-181">филеасидс</span><span class="sxs-lookup"><span data-stu-id="36fd1-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="36fd1-182">Адреса</span><span class="sxs-lookup"><span data-stu-id="36fd1-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="36fd1-183">Значение (Екстендедпропертитипе)</span><span class="sxs-lookup"><span data-stu-id="36fd1-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="36fd1-184">Ответ об ошибке операции GetImItems</span><span class="sxs-lookup"><span data-stu-id="36fd1-184">GetImItems operation error response</span></span>

<span data-ttu-id="36fd1-185">Операция **GetImItems** не проверяет идентификаторы и не возвращает ожидаемый ответ об ошибке **ерроринвалидимконтактид** или **ерроринвалидимграупид** , если службе предоставлен недопустимый идентификатор контакта или группы.</span><span class="sxs-lookup"><span data-stu-id="36fd1-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="36fd1-186">См. также</span><span class="sxs-lookup"><span data-stu-id="36fd1-186">See also</span></span>

- [<span data-ttu-id="36fd1-187">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="36fd1-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="36fd1-188">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="36fd1-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

