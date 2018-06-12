---
title: Пользователь
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b115c990-3a2d-4536-9af3-ac1fd06d00dc
description: Элемент пользователя определяет набор данных пользователя, возвращаемых запросом GetPersona.
ms.openlocfilehash: 15af72eb0e25e424aa7293ce0cbc2dd31e76abda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834736"
---
# <a name="persona"></a><span data-ttu-id="b95a4-103">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b95a4-103">Persona</span></span>

<span data-ttu-id="b95a4-104">Элемент **пользователя** определяет набор данных пользователя, возвращаемых запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b95a4-104">The **Persona** element specifies a set of persona data returned by a **GetPersona** request.</span></span> 
  
```XML
<Persona>
   <PersonaId/>
   <PersonaType/>
   <PersonaObjectStatus/>
   <CreationTime/>
   <Bodies/>
   <DisplayNameFirstLastSortKey/>
   <DisplayNameLastFirstSortKey/>
   <CompanyNameSortKey/>
   <HomeCitySortKey/>
   <WorkCitySortKey/>
   <DisplayNameFirstLastHeader/>
   <DisplayNameLastFirstHeader/>
   <FileAsHeader/>
   <DisplayName/>
   <DisplayNameFirstLast/>
   <DisplayNameLastFirst/>
   <FileAs/>
   <FileAsId/>
   <DisplayNamePrefix/>
   <GivenName/>
   <MiddleName/>
   <Surname/>
   <Generation/>
   <Nickname/>
   <YomiCompanyName/>
   <YomiFirstName/>
   <YomiLastName/>
   <Title/>
   <Department/>
   <CompanyName/>
   <Location/>
   <EmailAddress/>
   <EmailAddresses/>
   <PhoneNumber/>
   <ImAddress/>
   <HomeCity/>
   <WorkCity/>
   <RelevanceScore/>
   <FolderIds/>
   <Attributions/>
   <DisplayNames/>
   <FileAses/>
   <FileAsIds/>
   <DisplayNamePrefixes/>
   <GivenNames/>
   <MiddleNames/>
   <Surnames/>
   <Generations/>
   <Nicknames/>
   <Initials/>
   <YomiCompanyNames/>
   <YomiFirstNames/>
   <YomiLastNames/>
   <BusinessPhoneNumbers/>
   <BusinessPhoneNumbers2/>
   <HomePhones/>
   <HomePhones2/>
   <MobilePhones/>
   <MobilePhones2/>
   <AssistantPhoneNumbers/>
   <CallbackPhones/>
   <CarPhones/>
   <HomeFaxes/>
   <OrganizationMainPhones/>
   <OtherFaxes/>
   <OtherTelephones/>
   <OtherPhones2/>
   <Pagers/>
   <RadioPhones/>
   <TelexNumbers/>
   <TTYTDDPhoneNumbers/>
   <WorkFaxes/>
   <Emails1/>
   <Emails2/>
   <Emails3/>
   <BusinessHomePages/>
   <PersonalHomePages/>
   <OfficeLocations/>
   <ImAddresses/>
   <ImAddresses2/>
   <ImAddresses3/>
   <BusinessAddresses/>
   <HomeAddresses/>
   <OtherAddresses/>
   <Titles/>
   <Departments/>
   <CompanyNames/>
   <Managers/>
   <AssistantNames/>
   <Professions/>
   <SpouseNames/>
   <Children/>
   <Schools/>
   <Hobbies/>
   <WeddingAnniversaries/>
   <Birthdays/>
   <Locations/>
   <ExtendedProperties/>
</Persona>

```

 <span data-ttu-id="b95a4-105">**PersonaType**</span><span class="sxs-lookup"><span data-stu-id="b95a4-105">**PersonaType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b95a4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b95a4-106">Attributes and elements</span></span>

<span data-ttu-id="b95a4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b95a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b95a4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b95a4-108">Attributes</span></span>

<span data-ttu-id="b95a4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b95a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b95a4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b95a4-110">Child elements</span></span>

<span data-ttu-id="b95a4-111">[PersonaId](personaid.md) | [PersonaType](personatype.md) | [PersonaObjectStatus](personaobjectstatus.md) | [CreationTime](creationtime.md) | [текст сообщений](bodies.md) | [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md) | [DisplayNameLastFirstSortKey ](displaynamelastfirstsortkey.md)  |  [CompanyNameSortKey](companynamesortkey.md) | [HomeCitySortKey](homecitysortkey.md) | [WorkCitySortKey](workcitysortkey.md) | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md) | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md)  |  [FileAsHeader](fileasheader.md) | [DisplayName (string)](displayname-string.md) | [DisplayNameFirstLast](displaynamefirstlast.md) | [DisplayNameLastFirst](displaynamelastfirst.md) | [FileAs](fileas.md) | [FileAsId](fileasid.md)  |  [DisplayNamePrefix](displaynameprefix.md)  |  [GivenName](givenname.md) | [Отчество](middlename.md) | [Фамилия](surname.md) | [создания](generation.md) | [псевдонимов](nickname.md) | [YomiCompanyName](yomicompanyname.md) | [YomiFirstName ](yomifirstname.md)  |  [YomiLastName](yomilastname.md) | [заголовок](title.md) | [отдел](department.md) | [CompanyName](companyname.md) | [расположение](location.md) | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  |  [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)  |  [PhoneNumber](phonenumber.md) | [ImAddress (String)](imaddress-string.md) | [HomeCity](homecity.md) | [WorkCity](workcity.md) | [RelevanceScore](relevancescore.md) | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md)  |  [Атрибуты (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) | [DisplayNames](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames ](givennames.md)  |  [MiddleNames](middlenames.md) | [фамилии](surnames.md) | [поколения](generations.md) | [псевдонимы](nicknames.md) | [инициалы (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md)  |  [ YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones ](homephones.md)  |  [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md)  |  [CarPhones](carphones.md)  |  [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [пейджеры ](pagers.md)  |  [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md) | [Emails1](emails1.md) | [Emails2 ](emails2.md)  |  [Emails3](emails3.md) | [BusinessHomePages](businesshomepages.md) | [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | (ImAddresses[) ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md)  |  [ OtherAddresses](otheraddresses.md) | [заголовков](titles.md) | [отделы](departments.md) | [CompanyNames](companynames.md) | [руководители](managers.md) | [AssistantNames](assistantnames.md)  |  [ Профессиях](professions.md) | [SpouseNames](spousenames.md) | [дочерние элементы (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md) | [школы](schools.md) | [занятиях](hobbies.md)  |  [ WeddingAnniversaries](weddinganniversaries.md) | [рождения](birthdays.md) | [расположения](locations.md) | [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)</span><span class="sxs-lookup"><span data-stu-id="b95a4-111">[PersonaId](personaid.md) | [PersonaType](personatype.md) | [PersonaObjectStatus](personaobjectstatus.md) | [CreationTime](creationtime.md) | [Bodies](bodies.md) | [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md) | [DisplayNameLastFirstSortKey](displaynamelastfirstsortkey.md) | [CompanyNameSortKey](companynamesortkey.md) | [HomeCitySortKey](homecitysortkey.md) | [WorkCitySortKey](workcitysortkey.md) | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md) | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md) | [FileAsHeader](fileasheader.md) | [DisplayName (string)](displayname-string.md) | [DisplayNameFirstLast](displaynamefirstlast.md) | [DisplayNameLastFirst](displaynamelastfirst.md) | [FileAs](fileas.md) | [FileAsId](fileasid.md) | [DisplayNamePrefix](displaynameprefix.md) | [GivenName](givenname.md) | [MiddleName](middlename.md) | [Surname](surname.md) | [Generation](generation.md) | [Nickname](nickname.md) | [YomiCompanyName](yomicompanyname.md) | [YomiFirstName](yomifirstname.md) | [YomiLastName](yomilastname.md) | [Title](title.md) | [Department](department.md) | [CompanyName](companyname.md) | [Location](location.md) | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md) | [PhoneNumber](phonenumber.md) | [ImAddress (String)](imaddress-string.md) | [HomeCity](homecity.md) | [WorkCity](workcity.md) | [RelevanceScore](relevancescore.md) | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md) | [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) | [DisplayNames](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames](givennames.md) | [MiddleNames](middlenames.md) | [Surnames](surnames.md) | [Generations](generations.md) | [Nicknames](nicknames.md) | [Initials (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md) | [YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md) | [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md) | [CarPhones](carphones.md) | [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [Pagers](pagers.md) | [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md) | [Emails1](emails1.md) | [Emails2](emails2.md) | [Emails3](emails3.md) | [BusinessHomePages](businesshomepages.md) | [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | [ImAddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md) | [Titles](titles.md) | [Departments](departments.md) | [CompanyNames](companynames.md) | [Managers](managers.md) | [AssistantNames](assistantnames.md) | [Professions](professions.md) | [SpouseNames](spousenames.md) | [Children (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md) | [Schools](schools.md) | [Hobbies](hobbies.md) | [WeddingAnniversaries](weddinganniversaries.md) | [Birthdays](birthdays.md) | [Locations](locations.md) | [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b95a4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b95a4-112">Parent elements</span></span>

<span data-ttu-id="b95a4-113">[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md) | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md) | [GetPersonaResponseMessage](getpersonaresponsemessage.md) | [людей](people.md) | [пользователей](personas-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="b95a4-113">[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md) | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md) | [GetPersonaResponseMessage](getpersonaresponsemessage.md) | [People](people.md) | [Personas](personas-ex15websvcsotherref.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b95a4-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="b95a4-114">Remarks</span></span>

<span data-ttu-id="b95a4-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b95a4-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b95a4-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b95a4-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b95a4-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b95a4-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b95a4-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b95a4-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b95a4-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b95a4-119">Schema name</span></span>  <br/> |<span data-ttu-id="b95a4-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b95a4-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b95a4-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b95a4-121">Validation file</span></span>  <br/> |<span data-ttu-id="b95a4-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b95a4-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b95a4-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b95a4-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b95a4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b95a4-124">false</span></span>  <br/> |
   

