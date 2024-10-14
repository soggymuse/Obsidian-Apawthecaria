# Obsidian-Apawthecaria
Snippets and templates for setting up and playing the solo journalling RPG [Apawethecaria](https://blackwellwriter.itch.io/apawthecaria-a-poultice-pounder-adventure) in Obsidian.md.

## Flowcharts
[Apawthecaria](https://blackwellwriter.itch.io/apawthecaria-a-poultice-pounder-adventure) can be a bit confusing and involve a lot of back and forth between encounters and foraging and so on. 

**Note:** The screenshots show the flowcharts in my dark custom theme. If you copy them into your vault as .canvas files, they'll be the same colour as your theme. I plan to create light-mode versions at some point.

#### Making a Move
I made a flowchart to take you through all the different forks and decisions you need to make every time you make a move.

<a href="/APAW-Flowchart-Moving.png"><img src="/APAW-Flowchart-Moving.png" height="200px" /></a> <a href="/APAW-Flowchart-Moving-Light.png"><img src="/APAW-Flowchart-Moving-Light.png" height="200px" /></a>

_Click image to see bigger version_

It's available as an [Obsidian canvas](/APAW-Flowchart-Moving.canvas) to save directly into your vault, and as a (huge) [PNG](/APAW-Flowchart-Moving.png) for those of you who'd prefer to be able to view it elsewhere. (Now includes Soaring.)

#### Character Creation Flowchart
This part's not nearly as confusing, but I thought it still might come in handy to have a flowchart for it.

<a href="/APAW-Flowchart-CharacterCreation.png"><img src="/APAW-Flowchart-CharacterCreation.png" height="150px" /></a> <a href="/APAW-Flowchart-CharacterCreation-Light.png"><img src="/APAW-Flowchart-CharacterCreation-Light.png" height="150px" /></a>

_Click image to see bigger version_

It's also available as an [Obsidian canvas](/APAW-Flowchart-CharacterCreation.canvas) and a PNG in both [light](/APAW-Flowchart-CharacterCreation-Light.png) and [dark](/APAW-Flowchart-CharacterCreation.png) modes.

## Statblocks
I'm using statblocks from the [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin for things like character sheets and encounter cards.

You need a few things for these to work:
1. [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) installed and enabled
2. The **JSON** file for whichever statblock you want to use
3. The matching **template** (.md file) for whichever statblock you want to use.

The [CSS snippet](/APAW-Statblock.css) for the statblocks is *optional*. Mine make my statblocks match the main colours from the Apawthecaria map, but you can stick with the plugin's default or style your own. I wrote this snippet before I learned how to use theme variables, so you'll need to go through the **Set up Variables** section at the top and change all the colour hexes (e.g. <code>--statblock-background-color: #C0AD9B;</code>) to suit your theme.

### Non-player Character Sheet

<img src="/APAW-NPC-Statblock-Long.png" width="300px" />

*With extra line for "notes"*

<img src="/APAW-NPC-Statblock.png" width="300px" />

*Without line for notes*

The NPC statblock is short and designed for quick notes about characters you meet on the road. You can get the JSON for the statblock [here](/ApawthecariaNPC.json) (to import through the Fantasy Statblock plugin) and the markdown template [here](/FSB-APAW-NPC.md) (to save in your templates folder).

**Note:** I also use the NPC statblock for location cards (like for Odoak) to save on layouts. Just have the name, image, location, and description fields, and you'll get something like this:

<img src="/APAW-Location-Statblock.png" width="300px" />

*Image created with [NightCafe AI](https://creator.nightcafe.studio)*


### Ailment Cards

<img src="/APAW-AilmentCard.png" width="300px" />

This is a great way to copy the ailments from the PDF into Obsidian. You can link to tables that list [TAGs] for easier research for reagents. And you could have a rollable table that links to all the ailment cards in your vault so you can go right to the ailment when you come across a patient who's suffering from it.

The JSON for the statblock is [here](/ApawthecariaAilment.json) (to import through the Fantasy Statblock plugin) and the markdown template is [here](/FSB/APAW-Ailment.md) (to save in your templates folder).


### Coming Soon
I'll add more templates for them (and maybe the CSS, too) when I'm done fiddling. 
