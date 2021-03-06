---
-api-id: P:Windows.UI.Input.Preview.Injection.InjectedInputMouseInfo.MouseOptions
-api-type: winrt property
---

<!-- Property syntax
public Windows.UI.Input.Preview.Injection.InjectedInputMouseOptions MouseOptions { get;  set; }
-->

# Windows.UI.Input.Preview.Injection.InjectedInputMouseInfo.MouseOptions

## -description
Gets or sets the various options, or modifiers, used to simulate mouse input.

> [!NOTE]
> The APIs in this namespace require the inputInjectionBrokered [restricted capability](https://docs.microsoft.com/windows/uwp/packaging/app-capability-declarations#special-and-restricted-capabilities).

## -property-value
The options, or modifiers, for the mouse input.

## -remarks
Using input injection requires the following be added to the Package.appxmanifest:

- To `<Package>`
    - `xmlns:rescap="http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities"`
    - `IgnorableNamespaces="rescap"`
- To `<Capabilities>`
    - `<rescap:Capability Name="inputInjectionBrokered" />`


## -examples

## -see-also
