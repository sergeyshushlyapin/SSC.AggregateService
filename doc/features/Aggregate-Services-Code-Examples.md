# Aggregate Services Code Examples

**Code Examples** can be found in the [SSC.AggregateService project][1] on GitHub.

The `src\CustomeService.Sample` project contains the SSC Aggregate Services sample code and associated configuration files.
    
The sample code is intended to bootstrap your learning and understanding of the new *ASP.NET Web API* and *Dependency Injection* features delivered in Sitecore 8.2.

## [Attribute Routing][2] in ASP.NET Web API 2 

```
src\CustomService.Sample\Controllers\SimpleWepApiController.cs
```

## [Dependency Injection][3] configuration via code.

Makes use of a class derived from `Sitecore.DependencyInjection.IServicesConfigurator` and a configuration include file:

```
src\CustomService.Sample\DependencyInjection\CustomServiceConfigurator.cs
      
src\CustomService.Sample\App_Config\Include\CustomService.Sample.config

src\CustomService.Sample\Extensions\ServiceCollectionExtensions.cs
```

## [OData][4] based Web API Aggregate Services

```
src\CustomService.Sample\Controllers\TodoListController.cs
src\CustomService.Sample\Model\Todo.cs
src\CustomService.Sample\Data\TodoRepository.cs
src\CustomService.Sample\OData\AdminServiceDescriptor.cs 
```

## Using [ODataConventionModelBuilder][5] to create complex EDM models in Aggregate Services

```
src\CustomService.Sample\Controllers\CustomersController.cs
src\CustomService.Sample\Controllers\OrdersController.cs
src\CustomService.Sample\OData\Edm\CustomServiceEdmBuilder.cs
src\CustomService.Sample\OData\CustomServiceDescriptor.cs        
```


 [1]: https://github.com/kevinobee/SSC.AggregateService/
 [2]: https://www.asp.net/web-api/overview/web-api-routing-and-actions/attribute-routing-in-web-api-2
 [3]: https://msdn.microsoft.com/en-us/magazine/mt707534/
 [4]: http://www.odata.org/documentation/
 [5]: https://msdn.microsoft.com/en-us/library/system.web.http.odata.builder.odataconventionmodelbuilder/
