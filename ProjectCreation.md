# Creating a Project

## Completed once per computer
### Step 1. Import Preferences
1. Open Preferences by clicking on the gear icon in the top right hand corner below the search bar
2. Press the `Load...` button at the bottom of the window.
3. Navigate to the electric_boogaloo repository and open `UWRTPreferences.DXPPrf`
4. Press `Import` to begin the import process
5. Restart Altium when the import completes

### Step 2. Set Altium default locations
1. Re-open the preferences window
2. Go to `System -> Default Locations`
3. For `Document Path`, set that to the location of the electric_boogaloo repository
4. For the `Library Path`, set that to the Library folder in the electric_boogaloo repository
5. For the `OutputJob Path`, set that to a file not in the electric_boogaloo repository
6. Restart Altium to apply these default locations, if it prompts to create the OutputJobs folder, press yes

### Step 3. Add the UWRT_Project_Template
1. Re-open the preferences window
2. Go to `Data Management -> Templates`
3. At the bottom of the window, click the brows button for the `Local Templates folder`
4. Navigate to the `UWRT_Template_Project` folder in the electric_boogaloo repository
5. Hit Apply
6. Ensure that `UWRT_Template_Project` appears in the templates list
7. Go to the Defaults tab
8. Hit `Add...` then `From File` then `Schematic`
9. Navigate to the `UWRT_Template_Project` and select the `Sch_Sheet_Template` file
10. Hit Apply and OK

## Completed once per project
### Step 1. Create the new Project
1. Go to `File` then `New...` then `Project`
2. **Select `UWRT_Project_Template` as the project template**
3. Set the an appropriate project name. *It cannot contain spaces, it must use underscores*
4. Select the appropriate location for the project in the electric_boogaloo repository
5. Click `Create`

### Step 2. Rename and delete unused files
1. Rename `Sch_Sheet_Template.SchDoc` to `ProjectName_SheetName.SchDoc`
2. If more schematic sheets are needed, they should follow the `ProjectName_SheetName.SchDoc` naming convention
3. Rename `Sch_Notes_Template.SchDoc` to `ProjectName_Notes.SchDoc`
4. Rename the `Pcb_#layer_Template.PcbDoc` to `ProjectName.PcbDoc` for the layer number your board will be
5. Delete the other `Pcb_#layer_Template.PcbDoc` since that will not be used

### Step 3. Configure project specific parameters
1. Go to the `Project` menu, then click the `Project Options` button.
2. Click on the `Parameters` tab
3. Set the `ProjectTitle` to the title of the project (this can contain spaces)
6. Ensure `TeamLead` is set to the current electrical team lead
4. Leave `DateOfDesignReview` as it is for now, but it should be updated when the board gets its design review
5. Leave the `BoardRevision` at 1.0 unless otherwise stated

### Step 4. Configure sheet specific parameters
**Note: These steps must be performed for *each* schematic sheet made**
1. Open the sheet you want to set the parameters for
2. Ensure that there is nothing selected in the schematic sheet (just click in blank space to deselect anything)
3. Open the `Properties` panel. If you cannot find this, click on the `Panels` button in the bottom right corner, and select `Properties`
4. Click on the `Parameters` tab near the top of the properties panel
5. Update the `Date` parameter to the current date. You should see this be reflected in the Title Block in the bottom right of the sheet
6. Update the `Author` parameter to your name
7. Update the `Title` parameter to the sheet title. This is the title for what part of the board is going to be defined on this specific sheet

### Step 5. Configure Libraries for Project
1. Open any schematic document
2. Open the `Components` panel. If you cannot find it it will be under the `Panels` button in the bottom right corner
3. Click on the button with a three lines icon at the top of the components panel. *(Note: If only text appears reporting no components are installed, there should be a button in that message to browse for the library files)*
4. Click on `File-Based Libraries Preferences`
5. Click the `Add Library...` button
6. Navigate to the `electric_boogaloo` repository, in the `Libraries` subfolder
7. If nothing appears, make sure to change the `Integrated Libraries` filetype to `All Project Libraries`
8. Select all the libraries in the `Libraries` folder
9. Press `Open` then all of the libraries should appear in the list
10. Press `Close`
11. All the libraries should all appear in the dropdown menu next to the three line button.
12. Similarly, in the `Projects` menu a `Libraries` folder should appear, and inside there all of the libraries should be there as well

## Congratulations! You now have a new project. Have Fun Designing!