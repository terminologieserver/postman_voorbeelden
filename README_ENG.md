# postman
Examples for using the FHIR API, documented as a Postman collection. Import the JSON file in this map in Postman and create an *environment* with the variables *username* and *password*.

## Import
Importing the JSON file can be done by clicking on the button at the top of the left column.  

   ![Instellingen collection](screenshots/import_json.png)
   
The collection with examples will appear in the left column as __Voorbeelden Nationale Terminologieserver [incl authenticatie]__.

## Adding username and password
There are two ways to add the username and password to the collection:
- Collection variables
- Environment variables

The __collection__ as downloadable in this repository contains a __prerequest script__ that retrieves the username and password from the variables. For this, it first checks for the variables in the __collection__, and if these are empty or not present it will search in the __environment__. Below you will find an explanation for both methods.

If you wish to create multiple collections with different requests it could be useful to define the login details on the environment level. This way your login details will be the same for all collections. If you only have one collection for the National Terminology Server then defining the login details on this collection level will be more secure. That way it will not be accidentally used in other collections.


### Adding variables to the __collection__ level
- In the left bar click on _collectie_ __Voorbeelden Nationale Terminologieserver [incl authenticatie]__. This will open the settings of the _collection_.

    ![Instellingen collection](screenshots/openen_variabelen_collection.png)

- Click on the tab __Variables__. Enter your username and password in the correct row. Please ensure that you enter your username and password in the column __current value__, or they will not become active. Finally, click on __Save__ to save your changes.
    
    ![Instellingen collection](screenshots/wijzigen_variabelen_collection.png)
    
    ![Opslaan collection](screenshots/opslaan_variabelen_collection.png)


### Adding variables to the __environment__ level
- Click on the eye-icon, as displayed in the following screenshot

    ![Instellingen environment](screenshots/aanmaken_environment.png)
- Click on __Add__

    ![Toevoegen environment](screenshots/toevoegen_environment.png)
- Create two variables: __username__ and __password__. You can also name the environment by clicking on the pencil icon next to '_New Environment_'. Please ensure that you enter your username and password in the column __current value__, or they will not become active. Finally, click on __Save__ to save your changes.

    ![Aanpassen environment](screenshots/aanpassen_environment.png)
- Activate the correct environment by selecting it in the dropdown menu in the top right of the screen.

    ![Activeren environment](screenshots/activeren_environment.png)

- By clicking on the eye icon, as visible in the screenshot, the active environment variables will be displayed. These should match your recently entered login details. 

    ![Controleren environment](screenshots/controleren_actieve_environment.png)

# Adding new _requests_
It is possible to add new requests to the __collection__ yourself. As long as the request falls under the folder __Voorbeelden Nationale Terminologieserver [incl authenticatie]__ the authentication will occur automatically.

