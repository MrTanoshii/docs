---
menuTitle: actionListModules
Title: actionListModules
hidden: true
hookTitle: Allows you to add your own modules from a remote source in the modules list in the back office.
files:
 - src/Core/Module/ModuleRepository.php
locations:
 - back office
type: action
hookAliases:
hasExample: true
---

# Hook actionListModules {{< minver v="8.0" >}}

## Information

Hook locations:
- back office

Hook type: action

Located in:
- [src/Core/Module/ModuleRepository.php](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Core/Module/ModuleRepository.php)

## Call of the Hook in the origin file

```php
$modulesFromHook = $this->hookManager->exec('actionListModules', [], null, true);
$modulesFromHook = array_values($modulesFromHook ?? []);
```

## Example implementation

This hook has been implemented in the native [ps_distributionapiclient](https://github.com/PrestaShop/ps_distributionapiclient/tree/master) module