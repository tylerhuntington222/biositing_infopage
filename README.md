# Biositing Tool

This webtool was developed by the Lawrence Berkeley National Lab.                                                                    

The webtool can be found free of charge at: [https://biositing-tool-heroku.herokuapp.com/](https://biositing-tool-heroku.herokuapp.com/)


## Background


## Data
- **Wastewater treatment plants (WWTP) with anaerobic digestion**
- **Facilities with anaerobic digestion onsite other than WWTP**
- **Combustion plants**.
- **Manure locations**.
- **Manure (non points)**
- **Municipal solid waste locations**
- **Crop locations**
- **Processor residue (non points)**
- **District energy systems**
- **Mixed use developments (non points)**
- **Process heating and cooling locations**


## Webtool
The webtool is connected to the python algorithm through Flask. The frontend is a javascript based webtool. The user can interact with the webpage and create certain events that are logged and passed to the python module. Specifically, the user can:
- Select the **year** of the analysis from a drop-down menu.
- Set the **background layer** as biomass availability or thermal consumption density from a drop-down menu.
- Select whether the **facility** of interest is an Anaerobic Digestion or a Therochemical facility from a drop-down menu. This filters the biomass data by moisture and only shows the relevant portions based on the facility selection.
- Select from a drop-down menu whether the **biomass amounts** will be shown as gross amounts or technical amounts.
- Set the radius for the search **buffer** in which the analysis will be performed.
- **Click** on any point data on the map to get more information.
- **Click** on the map, to given the signal of the query point location, from where the algorithmic process is going to initiate. This will show the available biomass locations and amounts that fall within the predefined buffer zone.
- **Download** the data in a csv format for the entire county or the selected biomass that is inside the predefined buffer.
- **Report** whether there are errors in the data to us and we will work to the best of our abilities to confirm and fix any issues.

The outputs of the algorithmic process are going to appear on the screen after the computation is done. The outputs consist of the locations of all available biomass that are within the buffer zone from the clicked location. By clicking on any point the user can get more information on the nature and amounts of the biomass.