(Readme automatically translated, please submit PR with any mistakes you may notice.)

# Site Template for ActiveVFP in IIS

Welcome to the Site Template repository for ActiveVFP in IIS! In this repository, you'll find the necessary files and folders to configure and run ActiveVFP projects in Internet Information Services (IIS).

## About ActiveVFP
ActiveVFP (AVFP) is a completely free and open-source project for creating web applications with the Visual Foxpro programming language and database _(and other databases like MSSQL or MySQL)._ It provides an easy-to-use framework in pure Fox code to utilize a **multithreaded VFP dll** _(vfp mtdll)_ called from **ASP.NET**. If you're considering web programming with FoxPro, using FoxPro in the cloud, or converting desktop VFP to web or mobile using Android, iPhone, or iPad, this tool is for you.

## About the Template

ActiveVFP is a framework that enables web application development using Visual FoxPro. This template provides the base structure for configuring and running ActiveVFP projects in the IIS environment. Below is a detailed description of the contents of each folder and file in this template.

## Folder and File Structure

- **activevfp.dll** and **activevfp.dll.manifest**: These files are ActiveVFP modules necessary for its operation.

- **/bin**
  - **activevfp_dotnetproxy.dll**: Library that provides .NET capabilities for ActiveVFP.
  - **App_Code.dll**: Library containing shared application code.
  - **AspManifestHelpers.dll**: Library to help with ASP manifests.

- **/css**
  - **jquery-ui-1.8.7.css**, **jquery-ui.css**, **jquery.mobile-1.0rc1.min.css**, **Site.css** and **styles.css**: CSS files for site design and styling.
  - **Web.Config**: Configuration file for styles and CSS.

- **/html**
  - **default.avfp**: HTML template for the site's main page.

- **/prg**
  - **/handlers**
    - **/lib**
      - **resthelper.prg**: REST handler for auxiliary functions.
    - **resthandler.prg**: Main REST handler.

  - **/rest/controllers**
    - **/jsondb**
      - **configuration.json**: JSON database configuration for REST.
      - **examples.avfp**, **jsondb.avfp**, **reference.avfp**, **test.avfp**: JSON controllers for REST.
      - **jsondb.prg**: Main controller for handling JSON requests.

  - **main.prg**: Main application startup file.
  - **pages.prg**: File that handles pages and their content.
  - **/plugins**
    - **layouts.prg**: Plugin for managing page layouts.

- **/reports**
  - **clsheap.prg**, **print2pdf.prg**: Files related to report generation and handling.
  - **runfrx.exe**: Executable for generating reports.

- **/javascript**: JavaScript files for site functionality.
  - **jquery.js**, **jquery-ui.min.js**, **jquery.validate.min.js**, **ui.jqgrid.js**, among others.

- **/data**
  - **/newfeats**: Data files related to new features.

- **/docs**: Documentation related to the site and ActiveVFP.
  - **docs.htm**, **IIS_Setup_in_10_steps!.htm**: HTML documentation.

- **/images**: Images used in site design.
  - Various images used in CSS and HTML files.

- Root files:
  - `activevfp.dll`: The main ActiveVFP library for running Visual FoxPro code in IIS.
  - `activevfp.dll.manifest`: Manifest file that provides information about the `activevfp.dll` library.
  - `gxps.exe` and `runfrx.exe`: Utilities for generating and executing Visual FoxPro reports.
  - `Web.Config`: IIS configuration file for the site, defines how requests are handled and other configurations.
  - `webapp.manifest`: Another manifest file related to the web application.

## License

This project is distributed under the MIT License. See the LICENSE file for more details.

## Usage with MagicMenu

You can use the MagicMenu tool to simplify the process of creating and configuring sites using this template. MagicMenu automates the download and use of these same templates, allowing you to focus on developing your application.

- You can download and create sites manually using the files and folders provided in this repository.
- You can also use the MagicMenu tool for a more automated and user-friendly experience.
  
For more information about MagicMenu, visit the repository: [MagicMenu on GitHub](https://github.com/Irwin1985/MagicMenu).

## Windows Feature Activation and IIS Configuration

To ensure that IIS works correctly with ActiveVFP, follow these steps:
 - Open "Control Panel" -> "Programs" -> "Programs and Features" -> "Turn Windows features on or off".
 - Check the "Internet Information Services" box and its sub-features.
 - Make sure to select "CGI" and "ISAPI Filters" in the "World Wide Web Services" -> "Application Development Features" section.
 - Complete the process and restart your system if prompted.

## Support and Community

- If you have questions or need help with ActiveVFP, visit the [ActiveVFP Forum](https://groups.google.com/g/activevfp).
- In the absence of official documentation, the forum is an excellent resource for getting help and sharing knowledge.

## Contributions

Feel free to contribute and improve this template! If you have suggestions, improvements, or corrections, don't hesitate to make a pull request!

## Important Notes

- Make sure to comply with ActiveVFP requirements and recommended configurations for IIS.
- Consult ActiveVFP documentation and IIS resources for more information.
- Remember that security and maintenance are fundamental for successful deployment.

---

We hope this template helps you configure and run your ActiveVFP projects in IIS. If you have questions or need help, don't hesitate to contact us.
