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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761103"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="ca96f-103">Ссылки на сборку управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ca96f-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="ca96f-104">Найдите сведения о том, как ссылки на сборку управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca96f-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="ca96f-105">Управляемый API веб-служб Exchange предоставляет простой и полнофункциональных интерфейс для разработки и расширения приложений, использующих веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="ca96f-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="ca96f-106">С помощью Visual Studio или другой редактор кода, чтобы разрабатывать приложения управляемый API веб-служб Exchange, необходимо создать ссылку на сборку управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca96f-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="ca96f-107">Если вы еще не установили уже управляемый API веб-служб Exchange, необходимо [загрузить API-интерфейса](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="ca96f-107">If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ca96f-p102">[!Примечание]  Теперь управляемый API EWS доступен в виде проекта с открытым кодом на сайте [GitHub](https://github.com/officedev/ews-managed-api). С помощью библиотеки с открытым кодом вы можете: >  добавлять исправления ошибок и улучшения в API; >  получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске; >  получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах. >  Мы будем рады вашим [дополнениям](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="ca96f-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="ca96f-113">Создание ссылок на сборки</span><span class="sxs-lookup"><span data-stu-id="ca96f-113">Referencing the assembly</span></span>

<span data-ttu-id="ca96f-114">Чаще всего для добавления ссылки является использование Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="ca96f-114">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="ca96f-115">Мы знаем, что некоторые разработчиков предпочитают других редакторах, поэтому мы включая инструкции по использованию командной строки компилятора, а также инструкции по использованию Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="ca96f-115">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="ca96f-116">Пользователь может заметить, что ниже примерах кода имеют те же **с помощью** инструкции.</span><span class="sxs-lookup"><span data-stu-id="ca96f-116">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="ca96f-117">Различие между двумя методами — это, что компилятор командной строки необходимо указать расположение файла сборки.</span><span class="sxs-lookup"><span data-stu-id="ca96f-117">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="ca96f-118">Справочник по Visual Studio выполняет это автоматически в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="ca96f-118">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="ca96f-119">Чтобы добавить ссылку с помощью Visual Studio</span><span class="sxs-lookup"><span data-stu-id="ca96f-119">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="ca96f-120">Скопируйте файл Microsoft.Exchange.WebServices.dll и файл Microsoft.Exchange.WebServices.xml в папку по выбору.</span><span class="sxs-lookup"><span data-stu-id="ca96f-120">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="ca96f-121">По умолчанию файлы устанавливаются в `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, но могут сохранять файлы в любом месте на вашем компьютере.</span><span class="sxs-lookup"><span data-stu-id="ca96f-121">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="ca96f-122">В области обозреватель решений в Visual Studio выберите **ссылки**и затем выберите команду **Добавить ссылку**.</span><span class="sxs-lookup"><span data-stu-id="ca96f-122">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="ca96f-123">Откроется диалоговое окно Добавить ссылку.</span><span class="sxs-lookup"><span data-stu-id="ca96f-123">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="ca96f-124">В окне Добавить ссылку, перейдите на вкладку **Обзор** , перейдите к местоположению файла Microsoft.Exchange.WebServices.dll, выберите этот файл и нажмите кнопку « **ОК»**.</span><span class="sxs-lookup"><span data-stu-id="ca96f-124">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="ca96f-125">Чтобы использовать управляемый API EWS в приложении, добавьте оператор **using** для пространства имен **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="ca96f-125">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="ca96f-126">Чтобы добавить ссылку и выполните построение приложения с помощью командной строки компилятора</span><span class="sxs-lookup"><span data-stu-id="ca96f-126">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="ca96f-127">Поместите файл Microsoft.Exchange.WebServices.dll в папку по выбору.</span><span class="sxs-lookup"><span data-stu-id="ca96f-127">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice.</span></span> <span data-ttu-id="ca96f-128">Эта папка будет папку выходных данных для компилятора.</span><span class="sxs-lookup"><span data-stu-id="ca96f-128">This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="ca96f-129">В редакторе исходного кода добавьте оператор **using** в исходный код для пространства имен **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="ca96f-129">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="ca96f-130">Запуск командной строки компилятора для построения приложения.</span><span class="sxs-lookup"><span data-stu-id="ca96f-130">Run the command-line compiler to build the application.</span></span> <span data-ttu-id="ca96f-131">В следующей команде используется компилятора .NET Framework C# для создания приложений Windows, определенных в файле исходного кода «program.cs».</span><span class="sxs-lookup"><span data-stu-id="ca96f-131">The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs".</span></span> <span data-ttu-id="ca96f-132">Предполагается, что компилятор расположен в каталоге установки по умолчанию и, что файл Microsoft.Exchange.WebServices.dll находится в подкаталоге текущий каталог с именем «создать».</span><span class="sxs-lookup"><span data-stu-id="ca96f-132">It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="ca96f-133">См. также</span><span class="sxs-lookup"><span data-stu-id="ca96f-133">See also</span></span>

- [<span data-ttu-id="ca96f-134">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="ca96f-134">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="ca96f-135">Настройка среды разработки приложений Exchange</span><span class="sxs-lookup"><span data-stu-id="ca96f-135">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="ca96f-136">Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ca96f-136">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

