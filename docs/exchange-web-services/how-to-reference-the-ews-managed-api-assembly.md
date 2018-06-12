---
title: Ссылки на сборку управляемого интерфейса API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Найдите сведения о том, как ссылки на сборку управляемого интерфейса API веб-служб Exchange.
ms.openlocfilehash: af7b1ec449c24e7fa4db89abb30e5ebc9f8d329e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761103"
---
# <a name="reference-the-ews-managed-api-assembly"></a>Ссылки на сборку управляемого интерфейса API веб-служб Exchange

Найдите сведения о том, как ссылки на сборку управляемого интерфейса API веб-служб Exchange.
  
Управляемый API веб-служб Exchange предоставляет простой и полнофункциональных интерфейс для разработки и расширения приложений, использующих веб-служб Exchange (EWS). С помощью Visual Studio или другой редактор кода, чтобы разрабатывать приложения управляемый API веб-служб Exchange, необходимо создать ссылку на сборку управляемого интерфейса API веб-служб Exchange. Если вы еще не установили уже управляемый API веб-служб Exchange, необходимо [загрузить API-интерфейса](http://aka.ms/ews-managed-api-readme).
  
> [!NOTE]
>  [!Примечание]  Теперь управляемый API EWS доступен в виде проекта с открытым кодом на сайте [GitHub](https://github.com/officedev/ews-managed-api). С помощью библиотеки с открытым кодом вы можете: >  добавлять исправления ошибок и улучшения в API; >  получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске; >  получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах. >  Мы будем рады вашим [дополнениям](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) на сайте GitHub. 
  
## <a name="referencing-the-assembly"></a>Создание ссылок на сборки

Чаще всего для добавления ссылки является использование Visual Studio. Мы знаем, что некоторые разработчиков предпочитают других редакторах, поэтому мы включая инструкции по использованию командной строки компилятора, а также инструкции по использованию Visual Studio. Пользователь может заметить, что ниже примерах кода имеют те же **с помощью** инструкции. Различие между двумя методами — это, что компилятор командной строки необходимо указать расположение файла сборки. Справочник по Visual Studio выполняет это автоматически в фоновом режиме. 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Чтобы добавить ссылку с помощью Visual Studio

1. Скопируйте файл Microsoft.Exchange.WebServices.dll и файл Microsoft.Exchange.WebServices.xml в папку по выбору. По умолчанию файлы устанавливаются в `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, но могут сохранять файлы в любом месте на вашем компьютере.
    
2. В области обозреватель решений в Visual Studio выберите **ссылки**и затем выберите команду **Добавить ссылку**. Откроется диалоговое окно Добавить ссылку.
    
3. В окне Добавить ссылку, перейдите на вкладку **Обзор** , перейдите к местоположению файла Microsoft.Exchange.WebServices.dll, выберите этот файл и нажмите кнопку « **ОК»**. 
    
4. Чтобы использовать управляемый API EWS в приложении, добавьте оператор **using** для пространства имен **Microsoft.Exchange.WebServices.Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>Чтобы добавить ссылку и выполните построение приложения с помощью командной строки компилятора

1. Поместите файл Microsoft.Exchange.WebServices.dll в папку по выбору. Эта папка будет папку выходных данных для компилятора.
    
2. В редакторе исходного кода добавьте оператор **using** в исходный код для пространства имен **Microsoft.Exchange.WebServices.Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. Запуск командной строки компилятора для построения приложения. В следующей команде используется компилятора .NET Framework C# для создания приложений Windows, определенных в файле исходного кода «program.cs». Предполагается, что компилятор расположен в каталоге установки по умолчанию и, что файл Microsoft.Exchange.WebServices.dll находится в подкаталоге текущий каталог с именем «создать».
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>См. также

- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md)    
- [Настройка среды разработки приложений Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

