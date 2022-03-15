MainController.java

0.5 Constructor
Creating and populating our viewer fixtures here instead of initialize?

0.6 initialize
Initialize for the Tournament controller will display the following column headers per tourna-
ment Params: URL location, ResourceBundle resources

1. location = jar:ViewerControllerTest/build/libs/ViewerControllerTest-1.0-SNAPSHOT.jar!/com/test/viewercontrollertest/Viewer.fxml

The location used to resolve relative paths for the root object, or null if the location is not known.

2. resources = null css file is currently empty

The resources used to localize the root object, or null if the root object was not
localized.

list.setCellFactory Sets new ListCell’s created with the new cell factory. @override update()

0.7 loadStages

Every scene needs to load an fxml file. Images, icons and css files can also added to a scene.

load() FXMLLoader load() −>
resources fxml file −> 
controller constructor −>
initialize −>
back to load() set scene 
−> show()

Exceptions thrown launch −> start. 

Data Access Object
Database
Model
Service

Exceptions
1. java.lang.RuntimeException ”A bound value cannot be set.” When your stage is trying to show your
loaded scenes. At this point, null checks from FXML load() should not be a reason for this exception.
