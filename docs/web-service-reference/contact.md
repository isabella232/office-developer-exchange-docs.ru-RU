---
title: Контакт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Элемент Contact представляет элемент контакта в хранилище Exchange.
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44445652"
---
# <a name="contact"></a>Контакт

Элемент **Contact** представляет элемент контакта в хранилище Exchange. 
  
```XML
<Contact>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 **контактитемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[Сохранитьmimecontent](mimecontent.md) <br/> |Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения для элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объектов ответа.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень конфиденциальности элемента.  <br/> |
|[Body](body.md) <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер элемента в байтах. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[инреплито](inreplyto.md) <br/> |Представляет идентификатор элемента, который является ответом на этот элемент.  <br/> |
|[Отправлено](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.  <br/> |
|[Черновик](isdraft.md) <br/> |Указывает, был ли элемент еще не отправлен.  <br/> |
|[исфромме](isfromme.md) <br/> |Указывает, отправил ли пользователь элемент самому себе или самому себе.  <br/> |
|[исресенд](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[исунмодифиед](isunmodified.md) <br/> |Указывает, был ли изменен элемент.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.  <br/> |
|[датетимесент](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания определенного элемента в почтовом ящике.  <br/> |
|[респонсеобжектс](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.  <br/> |
|[реминдердуеби](reminderdueby.md) <br/> |Представляет дату и время возникновения события. Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[реминдериссет](reminderisset.md) <br/> |Указывает, задано ли напоминание для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события при отображении напоминания.  <br/> |
|[дисплайкк](displaycc.md) <br/> |Представляет отображаемую строку, используемую для содержимого строки "копия". Это объединенная строка всех отображаемых имен получателей копии.  <br/> |
|[дисплайто](displayto.md) <br/> |Представляет отображаемую строку, используемую для содержимого строки "Кому". Это объединенная строка для отображаемых имен получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет язык и региональные параметры для определенного элемента в почтовом ящике.  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[ластмодифиеднаме](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя для изменения элемента.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[Связанный](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[вебклиентреадформкуеристринг](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[вебклиентедитформкуеристринг](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.  <br/> |
|[FileAs](fileas.md) <br/> |Представляет способ хранения контакта в папке "Контакты".  <br/> |
|[филеасмаппинг](fileasmapping.md) <br/> |Определяет, как создавать отображаемые сведения о контакте.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Определяет отображаемое имя контакта.  <br/> |
|[GivenName](givenname.md) <br/> |Содержит имя контакта.  <br/> |
|[Initials](initials.md) <br/> |Представляет инициалы контакта.  <br/> |
|[MiddleName](middlename.md) <br/> |Представляет отчество контакта.  <br/> |
|[Прозвищ](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[комплетенаме](completename.md) <br/> |Представляет полное имя контакта.  <br/> |
|[CompanyName](companyname.md) <br/> |Представляет название компании, связанное с контактом.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адресов электронной почты контакта.  <br/> |
|[фисикаладдрессес](physicaladdresses.md) <br/> |Содержит коллекцию физических адресов, связанных с контактом.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию телефонных номеров контакта.  <br/> |
|[AssistantName](assistantname.md) <br/> |Представляет помощника для контакта.  <br/> |
|[Birthday](birthday.md) <br/> |Представляет дату рождения контакта.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Представляет домашнюю страницу контакта (веб-адрес).  <br/> |
|[Children](children.md) <br/> |Содержит имена потомков контакта.  <br/> |
|[Companies](companies.md) <br/> |Представляет коллекцию компаний, связанных с контактом.  <br/> |
|[контактсаурце](contactsource.md) <br/> |Указывает, находится ли контакт в хранилище Exchange или службе каталогов Active Directory.  <br/> |
|[Department](department.md) <br/> |Представляет подразделение контакта на рабочем месте.  <br/> |
|[Generation](generation.md) <br/> |Представляет сокращенное название, которое соответствует полному имени контакта.  <br/> |
|[Адреса](imaddresses.md) <br/> |Представляет коллекцию адресов обмена мгновенными сообщениями для контакта.  <br/> |
|[JobTitle](jobtitle.md) <br/> |Представляет должность контакта.  <br/> |
|[Manager](manager.md) <br/> |Представляет руководителя контакта.  <br/> |
|[Mileage](mileage.md) <br/> |Представляет расстояние для элемента контакта.  <br/> |
|[OfficeLocation](officelocation.md) <br/> |Представляет расположение контакта в офисе.  <br/> |
|[посталаддрессиндекс](postaladdressindex.md) <br/> |Представляет типы отображения для физических адресов.  <br/> |
|[Profession](profession.md) <br/> |Представляет профессия контакта.  <br/> |
|[спаусенаме](spousename.md) <br/> |Представляет имя супруга/партнера контакта.  <br/> |
|[ФИО](surname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[веддинганниверсари](weddinganniversary.md) <br/> |Содержит годовщину свадьбы контакта.  <br/> |
|[HasPicture](haspicture.md) <br/> |Указывает, имеет ли элемент контакта вложенный файл, представляющий изображение контакта.  <br/> |
|[фонетикфуллнаме](phoneticfullname.md) <br/> |Содержит полное имя контакта, включая имя и фамилию, введенное в фонетическое имя.  <br/> |
|[фонетикфирстнаме](phoneticfirstname.md) <br/> |Содержит имя контакта, написанное в фонетическом формате.  <br/> |
|[фонетикластнаме](phoneticlastname.md) <br/> |Содержит фамилию контакта с написанием фонетического имени.  <br/> |
|[Alias](alias.md) <br/> |Содержит псевдоним электронной почты контакта.  <br/> |
|[Примечания (контакт)](notes-contact.md) <br/> |Содержит дополнительную контактную информацию.  <br/> |
|[фотография](photo.md); <br/> |Содержит значение, которое кодирует фотографию контакта.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Содержит значение, которое кодирует сертификат SMIME контакта.  <br/> |
|[мсексчанжецертификате](msexchangecertificate.md) <br/> |Содержит значение, которое кодирует сертификат Microsoft Exchange контакта.  <br/> |
|[директорид](directoryid.md) <br/> |Содержит идентификатор каталога контакта.  <br/> |
|[манажермаилбокс](managermailbox.md) <br/> |Содержит данные SMTP, определяющие почтовый ящик руководителя контакта.  <br/> |
|[DirectReports](directreports.md) <br/> |Содержит сведения об SMTP, которые определяют прямые отчеты о контакте.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[аджацентмитингс](adjacentmeetings.md) <br/> |Описывает все элементы календаря, смежные с временем собрания.  <br/> |
|[аппендтоитемфиелд](appendtoitemfield.md) <br/> |Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуют с временем собрания  <br/> |
|[Create (Итемсинк)](create-itemsync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[Resolution](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
|[сетитемфиелд](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).  <br/> |
|[Обновление (Итемсинк)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание контактов (веб-службы Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Удаление контактов](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

