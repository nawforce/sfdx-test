# Test for Error parsing file (sfdx-cli/7.144.2)

To run:

    sfdx force:source:push -f

Actual Output: 

    *** Deploying with SOAP API v53.0 ***
    Deploy ID: 0AfB000000e7xelKAA

    === Component Failures [1]
    Type   Name          Problem
    Error  CustomLabels  Error parsing file: Unexpected element {http://soap.sforce.com/2006/04/metadata}p during simple type deserialization (8:19)

    ERROR running force:source:deploy:  Deploy failed.

Expected Output: 

    File should deploy sucessfully as it does with force:source:legacy:push.