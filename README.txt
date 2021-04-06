---------------------------------------------------------------------------------
- README file: The Teradata Vantage SCRIPT Table Operator Plugin for R and Python
-
- Version: 1.0.2
-
- April 2021
-
- Copyright (c) 2021 Teradata
---------------------------------------------------------------------------------

The Teradata Vantage SCRIPT Table Operator (STO) plugin for R and Python allows
end users to leverage the STO object in the Vantage Advanced SQL Engine Database.
STO enables Database users to push R and Python scripts, execute them natively
in the Database nodes, and thus benefit from scaled performance through execution
of script instances across the Database processing units. The Teradata Vantage
SCRIPT Table Operator plugin facilitates pushing down and executing with the STO
your custom-built R or Python code from
(a) notebooks built in Dataiku DSS, or
(b) external script files stored in DSS managed folders.
The plugin also allows you to push down to the Database any supplementary files
that may be needed by your script, such as R or Python model files.

Note that Dataiku DSS itself also supports ANSI SQL push-down for most of their
data preprocessing Visual recipes.

The present plugin has been tested with Vantage 1.1 Release Candidate 9 and
Vantage 2.0.


I. System Requirements
----------------------

The following component versions are required for the present plugin:

1. Dataiku Data Science Studio version 8.0.2 - 8.0.6
2. Teradata Vantage 1.1 or 2.0
3. Teradata JDBC Driver 16.20 (minimum), Teradata JDBC Driver 17.00 (recommended)

For R and Python support in Teradata Vantage, one or both of the following are required:

1. 9687-2000-0120	R Interpreter and Add-on Pkg on Teradata Advanced SQL
2. 9687-2000-0122	Python Interpreter and Add-on Pkg on Teradata Advanced SQL

Finally, to use the STO on a target Advanced SQL Engine,
(a) the STO Database object must be enabled on the Advanced SQL Engine, and
(b) as a Database user, you need to have suitable privileges for the STO granted
by your Database Administrator.
For more details, see documentation and references.


II. Install / Upgrade Instructions
----------------------------------

To install the Teradata Vantage SCRIPT Table Operator plugin, perform the
following:

1. In DSS Settings page (accessible through the Admin Tools button),
   select the [Plugins] tab, then select the [ADVANCED] option.
2. Click on [Choose File] and browse to the location of the present plugin
   zip file in your local filesystem.
3. If a previous installation of the Teradata Vantage Analytic plugin
   exists, check "Is update".
4. Click on [UPLOAD] button.
5. When the upload succeeds, click on [Reload] button, or do a hard refresh
   (Ctrl + F5) on all open Dataiku browsers for the change to take effect.

Documentation for the present plugin exists in the folder "resource/documentation"
of the plugin zip file.


III. Limitations
----------------

1. The plugin currently only supports Advanced SQL Engine datasets as input and
   output.


IV. References
--------------

For additional information on the Teradata Vantage Vantage SCRIPT Table Operator
search for the following on docs.teradata.com:

1. "Teradata Vantage SQL Operators and User-Defined Functions"
2. "Teradata Vantage User Guide"
3. “R And Python Analytics with SCRIPT Table Operator” (sign-in needed)


V. Changelog
------------

What’s new:
- Updated documentation and support details.

Release          Date             Notes
Version 1.0.2    April 2021       Current; updated documentation.
Version 1.0.0    September 2019   Initial release.
