---
title: Начало работы с клиентскими приложениями, использующими управляемый API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Разработка простого почтового клиентского приложения Hello World для Exchange с помощью управляемого API EWS.
ms.openlocfilehash: b4254ab80b4dfc2c8fadf90c79d57517c3a0bb16
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353989"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a>Начало работы с клиентскими приложениями, использующими управляемый API EWS

Разработка простого почтового клиентского приложения Hello World для Exchange с помощью управляемого API EWS. 
  
[Управляемый API EWS](http://aka.ms/ews-managed-api-readme) предоставляет интуитивно понятную и простую в использовании объектную модель для отправки и получения сообщений веб-служб от клиентских приложений, приложений порталов и приложений-служб. Управляемый API EWS предоставляет вам доступ почти ко всем сведениям, хранящимся в Exchange Online, Exchange Online в составе Office 365 или почтовом ящике сервера Exchange. Вы можете использовать сведения из этой статьи при разработке своего первого клиентского приложения, использующего управляемый API EWS. 
  
> [!NOTE]
> Управляемое API EWS теперь доступно в качестве проекта с открытым кодом на [GitHub](https://github.com/officedev/ews-managed-api). Вы можете использовать библиотеку открытого кода, чтобы: 
> - добавлять исправления ошибок и улучшения в API; 
> - получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске; 
> - получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах. 
>
>  Мы будем рады вашему [вкладу](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) в GitHub. 
  
## <a name="youll-need-an-exchange-server"></a>Вам потребуется сервер Exchange Server
<a name="NeedExchange"> </a>

Если у вас уже есть учетная запись почтового ящика Exchange, вы можете пропустить этот раздел. В противном случае у вас есть следующие варианты настройки почтового ящика Exchange для вашего первого клиентского приложения EWS:
  
- Заведите [сайт разработчиков Office 365](http://msdn.microsoft.com/ru-RU/library/office/fp179924.aspx) (рекомендуется). Это самый быстрый способ настройки почтового ящика Exchange. 
    
- Скачайте [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Убедившись, что вы можете отправлять и получать сообщения из Exchange, вы будете готовы настроить среду разработки. Вы можете использовать веб-клиент Exchange [Outlook Web App](http://technet.microsoft.com/ru-RU/library/jj657718%28v=exchg.150%29.aspx), чтобы убедиться, что вы можете отправлять сообщения. 
  
## <a name="set-up-your-development-environment"></a>Настройка среды разработки
<a name="Setup"> </a>

Убедитесь, что у вас есть доступ к следующим ресурсам:
  
- Любая версия [Visual Studio](http://www.visualstudio.com/ru-RU/downloads/download-visual-studio-vs.aspx), поддерживающая .NET Framework 4. Хотя на самом деле вам не требуется Visual Studio, ведь вы можете использовать любой компилятор C#, мы рекомендуем использовать его. 
    
- [Управляемый API EWS](http://aka.ms/ews-managed-api-readme). Вы можете использовать 64- или 32-разрядную версию в зависимости от вашей системы. Используйте для установки папку по умолчанию. 
    
## <a name="create-your-first-ews-managed-api-application"></a>Создание первого приложения, использующего управляемый API EWS
<a name="Create"> </a>

В этом руководстве предполагается, что у вас настроен сайт разработчиков Office 365. Если вы скачали и установили Exchange, потребуется [установить действительный сертификат](http://technet.microsoft.com/ru-RU/library/bb310769%28v=exchg.141%29.aspx) на сервере Exchange или [реализовать обратный вызов проверки сертификатов](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) для самозаверяющего сертификата, предоставляемого по умолчанию. Обратите внимание, что эти действия могут слегка отличаться в зависимости от используемой версии Visual Studio. 
  
### <a name="step-1-create-a-project-in-visual-studio"></a>Этап 1. Создание проекта в Visual Studio

1. В Visual Studio выберите в меню **Файл** пункт **Создать**, а затем  **Проект**. Откроется диалоговое окно **Новый проект**. 
    
2. Создайте **Консольное приложение C#**. В панели **Шаблоны** выберите **Visual C#**, а затем  **Консольное приложение**. 
    
3. Назовите проект HelloWorld, а затем нажмите кнопку **ОК**.
    
Visual Studio создаст проект и откроет окно документа с кодом Program.cs.

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a>Этап 2. Добавление ссылки на управляемый API EWS

1. Если окно **обозревателя решений** уже открыто, пропустите этот этап и переходите к этапу 2. Чтобы открыть **обозреватель решений**, в меню **Вид** выберите пункт **Обозреватель решений**. 
    
2. В **обозревателе решений** выберите проект **HelloWorld**, откройте контекстное меню (правая кнопка мыши) раздела **Ссылки** и выберите команду **Добавить ссылку**. Откроется диалоговое окно управления ссылками проекта. 
    
3. Выберите команду **Обзор**. Перейдите в папку, где установлена DLL-библиотека управляемого API EWS. По умолчанию программа установки выбирает следующий путь: C:\Program Files\Microsoft\Exchange\Web Services\<версия>\. Путь может зависеть от того, скачали вы 32- или 64-разрядную версию файла Microsoft.Exchange.WebServices.dll. Выберите **Microsoft.Exchange.WebServices.dll** и нажмите кнопку **ОК** или **Добавить**. В проект будет добавлена ссылка на управляемый API EWS. 
    
4. Если вы используете Управляемый API EWS 2.0, измените проект HelloWorld, чтобы он ссылался на .NET Framework 4. Другие версии управляемого API EWS могут использовать другую целевую версию .NET Framework.
    
5. Убедитесь, что вы используете правильную целевую версию .NET Framework. Откройте контекстное меню (правая кнопка мыши) проекта **HelloWorld** в **обозревателе решений** и выберите пункт **Свойства**. Убедитесь, что в раскрывающемся списке **Целевая рабочая среда** выбран пункт **.NET Framework 4**. 
    
Теперь, когда у вас есть настройка проекта и вы создали ссылку на управляемое API EWS, то вы готовы создать свое первое приложение. Для простоты работы добавьте код в файл Program.cs. Ознакомьтесь со статьей [Ссылка на сборку управляемого API EWS](how-to-reference-the-ews-managed-api-assembly.md) для получения дополнительной информации о ссылках на управляемое API EWS. На следующем этапе вы будете разрабатывать базовый код, чтобы создавать большинство клиентских приложений управляемого API EWS. 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a>Этап 3. Настройка проверки перенаправления URL-адресов для автообнаружения

- Добавьте приведенный ниже метод обратного вызова для проверки перенаправления после метода **Main(string[] args)**. Он проверяет, представляют ли перенаправленные URL-адреса, возвращенные функцией [автообнаружения](autodiscover-for-exchange.md), конечную точку HTTPS. 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

Этот проверяющий метод обратного вызова будет передан объекту **ExchangeService** на этапе 4. Это необходимо, чтобы ваше приложение доверяло и следовало перенаправлению функции автообнаружения  результат перенаправления функции автообнаружения предоставляет конечную точку EWS для вашего приложения. 

### <a name="step-4-prepare-the-exchangeservice-object"></a>Этап 4. Подготовка объекта ExchangeService

1. Добавьте ссылку на директиву **using** в управляемый API EWS. Добавьте следующий код после директивы **using** в начале файла Program.cs. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. В методе **Main** создайте экземпляр объекта [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в нужной версией службы. В этом примере используется самая ранняя версия схемы EWS. 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. Если вы ссылаетесь на локальный сервер Exchange и ваш клиент присоединен к домену, переходите к этапу 4. Если ваш клиент ссылается на почтовый ящик Exchange Online или сайта разработчиков Office 365, необходимо передавать учетные данные в явной форме. Добавьте следующий код после создания экземпляра объекта **ExchangeService** и задайте данные учетной записи почтового ящика. Имя пользователя должно быть именем участника-пользователя. Переходите к этапу 5. 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. Присоединенные к доменам клиенты, которые ссылаются на локальный сервер Exchange, могут использовать заданные по умолчанию учетные данные пользователя, выполнившего вход, при условии, что учетные данные связаны с почтовым ящиком. Добавьте следующий код после создания экземпляра объекта **ExchangeService**. 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   Если ваш клиент ссылается на почтовый ящик Exchange Online или сайта разработчиков Office 365, убедитесь, что для параметра [UseDefaultCredentials](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) задано значение **false**, установленное по умолчанию. Ваш клиент готов совершить первый вызов службы автообнаружения, чтобы получить URL-адрес службы для вызовов службы EWS.
    
5. Метод **AutodiscoverUrl** объекта **ExchangeService** совершает серию вызовов службы автообнаружения, чтобы получить URL-адрес службы. Если вызов этого метода совершен успешно, для свойства URL объекта **ExchangeService** будет задано значение URL-адреса службы. Передайте адрес электронной почты пользователя и **RedirectionUrlValidationCallback** методу **AutodiscoverUrl**. Добавьте приведенный ниже код после указания учетных данных на этапе 3 или 4. Измените  `user1@contoso.com` на ваш адрес электронной почты, чтобы служба автообнаружения нашла конечную точку EWS. 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

На этом этапе ваш клиент настроен для вызовов EWS для доступа к данным почтового ящика. Если вы сейчас запустите свой код, то сможете проверить, что метод вызова **AutodiscoverUrl** отработал, проверив содержимое свойства [ExchangeService.Url](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). Если это свойство содержит URL-адрес, то ваш вызов был удачным! Это означает, что ваше приложение успешно прошло проверку подлинности службой и обнаружило конечную точку EWS для почтового ящика. Теперь вы готовы выполнить первый вызов EWS. Ознакомьтесь со статьей [Настройка URL-адреса службы EWS с помощью управляемого API EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) для получения дополнительной информации о настройке URL-адреса EWS. 

### <a name="step-6-create-your-first-hello-world-email-message"></a>Этап 6. Создание первого сообщения электронной почты Hello World

1. После вызова метода **AutodiscoverUrl** создайте новый экземпляр объекта **EmailMessage** и передайте созданный ранее объект службы. 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   Теперь у вас есть сообщение электронной почты, в котором задана привязка к службе. Вызовы, совершенные из объекта **EmailMessage**, будут адресованы службе. 
    
2. Теперь задайте получателя сообщения. Для этого замените  `user1@contoso.com` на ваш SMTP-адрес. 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. Задайте тему и основной текст сообщения.
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. Теперь вы готовы отправить первое сообщение электронной почты с помощью службы управляемого API EWS. Метод **Send** вызовет службу и отправит сообщение электронной почты для доставки. Ознакомьтесь со статьей [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) для получения дополнительной информации о других методах, которые можно использовать для взаимодействия с Exchange. 
    
   ```cs
    email.Send();
   ```

5. Вы готовы запустить свое приложение Hello World. В Visual Studio нажмите клавишу **F5**. Откроется пустое окно консоли. В окно консоли не будет появляться никакого текста, пока приложение проходит проверку подлинности, следует перенаправлению службы автообнаружения, а затем совершает первый вызов для создания сообщения электронной почты, которое вы отправляете себе. Если вы хотите увидеть совершаемые вызовы, добавьте две приведенные ниже строки кода перед вызовом метода **AutodiscoverUrl**. Затем нажмите клавишу F5. [Запросы и ответы EWS будут трассированы](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) в окне консоли. 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

Теперь у вас есть работоспособное приложение, использующее управляемый API EWS. Для вашего удобства в следующем примере показан весь код, добавленный в файл Program.cs для создания приложения Hello World.

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a>Дальнейшие действия
<a name="Next"> </a>

Если вы готовы усовершенствовать свое первое клиентское приложение с использованием управляемого API EWS, изучите следующие ресурсы:
  
- [Exchange 2013: базовые примеры кода](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)   
- [Папки и элементы](folders-and-items-in-ews-in-exchange.md)    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
Если с приложением возникли проблемы, [попробуйте опубликовать вопрос или комментарий на форуме](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (и не забудьте прочитать первое сообщение). 
  
## <a name="in-this-section"></a>В этой статье
<a name="Next"> </a>

- [Ссылка на сборку управляемого API EWS](how-to-reference-the-ews-managed-api-assembly.md)   
- [Настройка URL-адреса службы EWS с помощью управляемого API EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)   
- [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a>См. также

- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)   
- [Трассировка запросов и ответов для устранения неполадок в приложениях управляемого API EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

