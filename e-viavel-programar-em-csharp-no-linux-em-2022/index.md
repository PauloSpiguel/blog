## Introdução

C# e Linux, um casamento complicado? A um bom tempo atrás, era apenas possível desenvolver, sem dor de cabeça, para o ambiente .Net somente no Windows, com algumas ressalvas com a “falecida” IDE MonoDevelop (https://www.monodevelop.com/) para ajudar o pinguim.

Bom, um pouco de história: em 2016, a Microsoft anunciava o .Net Core, uma reimplementação do famoso e amado, por uns odiados, Framework de sua autoria, dessa vez disponível para, além do Windows, o macOS e Linux. Claro, nem tudo são flores e é impossível fazer uma reimplementação de um gigantesco Framework igualmente completo como o seu “pai” do dia para a noite e distribuir por ai aos SO’s de maior relevância do mercado, mesmo que de forma gratuita e open source.

No ano de 2020, a versão 5 do .Net foi disponibilizada como estável, tanto SDK como para run time, o que marcou a unificação de uma baita confusão de versões do .Net, deixando para trás o .Net Framework (aquele exclusivo para Windows), .Net Core (versões iniciais do .Net open source) e a criação do padrão “.Net Standard.” Mas, agora retomando o rumo da venta. É viável programar em C# no Linux em 2022? Bom, a resposta é dupla: sim e não.

## Explicando

**Por que sim?**

Com o amadurecimento da ferramenta ao passar dos anos e, um gigante apoio, da JetBrains com a IDE Rider, desenvolver com C#, especialmente para a Web, Console applications, Worker Services e Unit Tests, hoje possuímos uma baita ferramenta completa, apesar de salgada, para desenvolver com comodidade no Linux (até mesmo no Mac, além do Visual Studio for Mac, e no Windows, caso não queira o Visual Studio). Para os que ainda duvidam, deem uma olhada no meu mais recente e maduro projeto de APS Net feito 100% no Linux: [A basic Snack Store MVC project.](https://github.com/JGMelon22/Snacks_Web_MVC_SqlServer)

![ImagemRider](https://user-images.githubusercontent.com/73988556/151468561-fbaa27be-625f-47c2-ac71-80a7a7f826d2.png)

**Por que não?**

Alguns podem estranhar que eu não comentei sobre o editor de textos, muito confundido com IDE, Visual Studio Code. O Visual Studio Code, apesar de ficar bem redondinho para codificar em C# com algumas extensões, especialmente as da imagem a baixo, acaba pecando por ser limitado em alguns aspectos, sendo os mais chatinho a falta de facilidade para auxiliar a geração de itens do Scaffolding ASP .NET Core - Usando os recursos do Scaffolding, a necessidade de usar a implementação “curada” da Microsoft do Visual Studio Code (o que complica aos que usam distros como o Solus, pois a versão disponível nos repositório é a VSCode-oss) (GitHub - microsoft/vscode: Visual Studio Code) e a falta, por hora, de uma alternativa ao WinForms, caso você queira desenvolver para computadores locais, mas não curte nem um pouco se aventurar na web com um tico de JavaScript, CSS, Html e Bootstrap.

![ImagemExtensoes](https://user-images.githubusercontent.com/73988556/151468654-aca6cd7a-8142-472e-883f-477c03648519.png)

![ImagemVSCode](https://user-images.githubusercontent.com/73988556/151468658-fb5319ac-a8d3-4c7f-b0be-1313e407c70b.png)

## Fazendo uma breve tangência: 

há esperança de um dia surgir uma alternativa ao WinForms, para Mac (e talvez Linux)? Sim, jovem Padawan e esse sonho pode estar cada vez mais perto devido ao MAUI, um acrônimo para Multi-platform App UI, que além de possibilitar reusar o mesmo código para desktop, permitirá portar o programa em questão para mobile (IOS e Android), aposentando o legado Xamarin Forms. A notícia triste é que o MAIU foi adiado para Q2 de 2022 (.NET MAUI: Preview 8 Available, But GA Postponed to Q2 2022).

Mas existem boas alternativas já disponíveis como o [AvaloniaUI](https://avaloniaui.net/) e o [UNO Plataform](https://platform.uno/), ambos visando o desenvolvimento multiplataforma, mas com um toque de XAML (na unha).
 
 ## Conclusão

Bom, caso você opte pelo desenvolvimento web, ASP Net, desenvolver em C# no Linux, até o presente o momento, será uma experiência bastante agradável. Mas, caso você precise desenvolver aplicações locais usando WinForms, eu sinto em informar que somente pelo Windows mesmo, visto que o WinForms, assim como o Visual Basic For Application, depende de componentes do Windows para funcionar [Design Windows Forms | JetBrains Rider](https://www.jetbrains.com/help/rider/Working_with_Windows_Forms.html), você precisará usar o SO da Microsoft (ou via máquina virtual ou dual boot). 

## Continue lendo:

[Visual Studio Code - Instalação e costumização](https://balta.io/blog/visual-studio-code-instalacao-customizacao)

[WSL - Windows Subsystem for Linux](https://balta.io/blog/wsl)

[Plataform Specific no .NET](https://balta.io/blog/dotnet-platform-specific)
