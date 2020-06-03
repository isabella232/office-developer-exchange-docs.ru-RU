---
title: Операция GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Поиск сведений о GetDiscoverySearchConfigurationной операции EWS.
ms.openlocfilehash: 4db435988a9954b921e7851986b6f92ffedbad94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461025"
---
# <a name="getdiscoverysearchconfiguration-operation"></a>Операция GetDiscoverySearchConfiguration

Поиск сведений о **GetDiscoverySearchConfigurationной** операции EWS. 
  
Операция **GetDiscoverySearchConfiguration** возвращает сведения о конфигурации для удержаний на месте, сохраненных поисков и почтовых ящиков, которые включены для поиска обнаружения. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a>Использование операции GetDiscoverySearchConfiguration

Операция **GetDiscoverySearchConfiguration** предоставляет сведения о конфигурации для поиска при обнаружении. Запросы могут содержать один или несколько из следующих аргументов: 
  
1. [Сеарчид](searchid.md) — определяет сохраненный поисковый запрос на обнаружение. Если этот аргумент отправляется в запросе, значения других аргументов игнорируются. 
    
2. [Експандграупмембершип](expandgroupmembership.md) — указывает, развернут ли в ответе членство в группе. Значение **true** указывает, что членство в группе развернуто, и в ответе возвращаются все доступные для поиска почтовые ящики. Значение **false** указывает, что в ответе возвращается только группа. 
    
3. [Инплацехолдконфигуратиононли](inplaceholdconfigurationonly.md) — указывает, возвращаются ли все доступные для поиска почтовые ящики в дополнение к конфигурации хранения на месте. Значение **true** указывает, что возвращаются только конфигурации хранения на месте. Значение **false** указывает, что все идентификаторы почтовых ящиков, доступные для поиска, возвращаются в дополнение к идентификаторам хранения на месте. Если этот элемент отсутствует, то поведением по умолчанию является эквивалент значения **false**. 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a>Заголовки SOAP операции GetDiscoverySearchConfiguration

Операция **GetDiscoverySearchConfiguration** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a>Пример запроса операции GetDiscoverySearchConfiguration: получение конфигурации поиска при обнаружении для сохраненного поиска

В следующем примере запроса операции **GetDiscoverySearchConfiguration** показано, как запросить конфигурацию сохраненного поиска с именем "мидисксеарчфор — сбровн". Аргументы для элементов [експандграупмембершип](expandgroupmembership.md) и [инплацехолдконфигуратиононли](inplaceholdconfigurationonly.md) игнорируются. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)
    
- [сеарчид](searchid.md)
    
- [експандграупмембершип](expandgroupmembership.md)
    
- [инплацехолдконфигуратиононли](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a>Успешный отклик операции GetDiscoverySearchConfiguration: запрос на один сохраненный поиск

В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения конфигурации сохраненного поиска с именем "мидисксеарчфор — сбровн". 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [жетдисковерисеарчконфигуратионреспонсе](getdiscoverysearchconfigurationresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)
    
- [дисковерисеарчконфигуратион](discoverysearchconfiguration.md)
    
- [сеарчид](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [сеарчаблемаилбоксес](searchablemailboxes.md)
    
- [сеарчаблемаилбокс](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (строка)](primarysmtpaddress-string.md)
    
- [исекстерналмаилбокс](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [исмембершипграуп](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a>Успешный отклик операции GetDiscoverySearchConfiguration: запрос удержания на месте

В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения только удержаний на месте. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [жетдисковерисеарчконфигуратионреспонсе](getdiscoverysearchconfigurationresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)
    
- [дисковерисеарчконфигуратион](discoverysearchconfiguration.md)
    
- [сеарчид](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [InPlaceHoldIdentity](inplaceholdidentity.md)
    
- [манажедбйорганизатион](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a>Успешный отклик операции GetDiscoverySearchConfiguration: запрос для всех сохраненных конфигураций поиска для обнаружения

В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения всех сохраненных поисков обнаружения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [жетдисковерисеарчконфигуратионреспонсе](getdiscoverysearchconfigurationresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)
    
- [дисковерисеарчконфигуратион](discoverysearchconfiguration.md)
    
- [сеарчид](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [сеарчаблемаилбоксес](searchablemailboxes.md)
    
- [сеарчаблемаилбокс](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (строка)](primarysmtpaddress-string.md)
    
- [исекстерналмаилбокс](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [исмембершипграуп](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a>Ответ об ошибке операции GetDiscoverySearchConfiguration

В следующем примере показан ответ об ошибке для запроса операции **GetDiscoverySearchConfiguration** . Это ответ на запрос на получение сохраненного поиска, не найденного на сервере. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жетдисковерисеарчконфигуратионреспонсе](getdiscoverysearchconfigurationresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchMailboxes](searchmailboxes.md)
    
- [GetHoldOnMailboxes](getholdonmailboxes.md)
    
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)
    

