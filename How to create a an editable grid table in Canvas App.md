/* Using the sequence function and collection to create an editable table to capture data in an excel like format inside Canvas Apps */

Insert a ComboxBox/Dropdown Control 
/*Change Item property into :*/  Sequence('Desired Number')
/*Change the Combox OnChange property to create a variable with the sequence function :*/ ClearCollect({Grid, Sequence(Self.Selected.Value))
Insert a Vertical gallery 
Insert and Input Controls required into the gallery 
/* Change Gallery Item Property to the varibale */ Items = Grid
/* Use the ForAll function to extract all data entry*/

![image](https://github.com/GeeksDam/PowerApps/assets/98710158/039c24e6-3975-4937-90d4-5199a3836c46)
