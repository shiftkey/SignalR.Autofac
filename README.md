# LICENSE
MIT License <http://www.opensource.org/licenses/mit-license.php>

## Get it on NuGet!
SignalR.Autofac is an extension for integrating the Autofac Inversion of Control container into a SignalR server:


To get started, install the package into a new or existing web application:

    Install-Package SignalR.Autofac

## Registration
Open the App_Start/AutofacSignalR.cs file and register the components your service needs:

    private static void RegisterServices(ContainerBuilder builder)
    {
         builder.RegisterType<SomeClass>().AsImplementedInterfaces();
		 builder.RegisterType<Anotherclass>().AsImplementedInterfaces();
    }

And that's it!