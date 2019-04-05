<!-- default file list -->
*Files to look at*:

* [MainPage.xaml](./CS/MainPage.xaml) (VB: [MainPage.xaml](./VB/MainPage.xaml))
* [MainPage.xaml.cs](./CS/MainPage.xaml.cs) (VB: [MainPage.xaml.vb](./VB/MainPage.xaml.vb))
* [MainViewModel.cs](./CS/MainViewModel.cs) (VB: [MainViewModel.vb](./VB/MainViewModel.vb))
* [RichEditEx.cs](./CS/RichEditEx.cs) (VB: [RichEditEx.vb](./VB/RichEditEx.vb))
* [ThemeFriendlyNameConverter.cs](./CS/ThemeFriendlyNameConverter.cs) (VB: [ThemeFriendlyNameConverter.vb](./VB/ThemeFriendlyNameConverter.vb))
* [CustomColorScheme.cs](./CS/Themes/CustomColorScheme.cs) (VB: [CustomColorScheme.vb](./VB/Themes/CustomColorScheme.vb))
* [generic.xaml](./CS/Themes/generic.xaml) (VB: [generic.xaml](./VB/Themes/generic.xaml))
<!-- default file list end -->
# How to define a custom Color Scheme for Windows 10 XAML controls


<br>This example illustrates how to implement a custom Color Scheme and use it in your application. In the current implementation, the application supports two themes (Generic and Custom), which can be changed by using the corresponding ComboBox. <br><br>The <strong>Custom </strong>color scheme is defined as a separate GenericColorScheme class descendant with the corresponding color changes in the overridden <strong>Initialization</strong> method. To register this theme use the static <strong>ThemeManager.RegisterColorScheme</strong> method: <br><br>


```xaml
ThemeManager.RegisterColorScheme(new CustomColorScheme("Custom"));
```


<br>All colors available for overriding are listed in separate files within the installation folder with our controls: <DevExpress Installation Folder><strong><u>\Components\System\UAP\ColorThemes<br><br></u></strong>If you wish to do this in an older version, refer to the following example: <a href="https://www.devexpress.com/Support/Center/p/T404909">T404909 - How to define a custom Color Scheme for Windows 10 XAML controls</a>. 

<br/>


