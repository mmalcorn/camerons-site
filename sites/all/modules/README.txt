Modules extend your site functionality beyond Drupal core.

WHAT TO PLACE IN THIS DIRECTORY?
--------------------------------

Placing downloaded and custom modules in this directory separates downloaded and
custom modules from Drupal core's modules. This allows Drupal core to be updated
without overwriting these files.

DOWNLOAD ADDITIONAL MODULES
---------------------------

Contributed modules from the Drupal community may be downloaded at
https://www.drupal.org/project/project_module.

ORGANIZING MODULES IN THIS DIRECTORY
------------------------------------

You may create subdirectories in this directory, to organize your added modules,
without breaking the site. Some common subdirectories include "contrib" for
contributed modules, and "custom" for custom modules. Note that if you move a
module to a subdirectory after it has been enabled, you may need to clear the
Drupal cache so it can be found. (Alternatively, you can disable the module
before moving it and then re-enable it after the move.)

MULTISITE CONFIGURATION
-----------------------

In multisite configurations, modules found in this directory are available to
all sites. Alternatively, the sites/your_site_name/modules directory pattern
may be used to restrict modules to a specific site instance.

MORE INFORMATION
----------------

Refer to the "Developing for Drupal" section of the README.txt in the Drupal
root directory for further information on extending Drupal with custom modules.

--------------------------------------
greeting.info file
------------------
Gives Drupal about information about the module, such as the name or the description
* Requires a "name", "description", and "package" which are displayed in the Modules Admin page where you can enable your module.
* "core" defines which version the module is compatible with.
* "files" is an array containing the relative paths to any external files to load.

--------------------------------------
greeting.module file
--------------------
Will contain core of the module
*Contains two arrays - one for functions, one for html
