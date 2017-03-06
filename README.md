OOSass
===

A scaffold for sass/scss based projects.

You can extend it as you need.

**Base**

The base directory is reserved for Sass code for base elements, normalize stylesheet, custom reset code and base typography declarations.

**Fonts**

The fonts directory is reserved for custom fonts source files.

**Helpers**

The modules directory is reserved for Sass code that doesn't cause Sass to actually output CSS, things like mixin declarations, functions, variables, placeholder selectors.


**Layout**

The partials directory is where the meat of my CSS is constructed. Break stylesheets into (header, sidebar, and footer components and a few others), or break into much finer categories (typography, buttons, textboxes, selectboxes, etc…).
The views directory is where page specific styles are constructed and partials combined or (if needed) modified and adapted to their container.


**Vendor**
The vendor directory is for third-party CSS. This is handy when using prepackaged components developed by other people (or for your own components that are maintained in another project).
jQuery UI and a color picker are examples of CSS that you might want to place in the vendor directory. 

**Folder Structure**

```
sass/
|
|-- base/                  # Base
|   |-- _base.scss         # Set of commons elements
|   |-- _normalize.scss    # Normalize style
|   |-- _reset.scss        # Custom reset style
|   |-- _typography.scss   # Typography settings and declarations
|   ...
|
|-- fonts/                 # Custom fonts source files
|   ...
|
|-- helpers/               # Helpers
|   |-- _functions.scss    # Global Functions
|   |-- _mixins.scss       # Global Mixins
|   |-- _variables.scss    # Global Variables
|   ...
|
|-- layout/                # Layout
|   |-- _view/             # Stylesheet for specific view
|   |-- _footer.scss       # Header specific stylesheet
|   |-- _header.scss       # Footer specific stylesheet
|   |-- _sidebar.scss      # Sidebar specific stylesheet
|   ...
|
|-- vendor/                # Vendor
|   |-- _colorpicker.scss  # Color picker specific stylesheet
|   |-- _jqueryui.scss     # jQuery UI specific stylesheet
|   ...
|
`-- main.scss              # Primary Sass file
````