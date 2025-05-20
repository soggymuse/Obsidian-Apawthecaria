# Obsidian-Apawthecaria
Snippets and templates for setting up and playing the solo journalling RPG [Apawethecaria](https://blackwellwriter.itch.io/apawthecaria-a-poultice-pounder-adventure) in Obsidian.md.

## Boheme Theme

<img width="1280" alt="Screenshot 2025-04-14 at 07 06 31" src="https://github.com/user-attachments/assets/cc203270-cc7f-4847-8877-e030545f8903" />

Boheme is an _untested_ brown and gold theme made for my Apawthecaria playthrough. It makes heavy use of javalent's Fantasy Statblocks plugin.

## Flowcharts **1.0**
[Apawthecaria](https://blackwellwriter.itch.io/apawthecaria-a-poultice-pounder-adventure) can be a bit confusing and involve a lot of back and forth between encounters and foraging and so on. I've made several attempts to chart out the play loop, updating as I come to understand the game better. The following is from v1.0 but there is a more up-to-date version [here](/ApawthecariaFlowcharts).

**Note:** The screenshots show the flowcharts in my dark custom theme. If you copy them into your vault as .canvas files, they'll be the same colour as your theme. I plan to create light-mode versions at some point.

#### Making a Move
I made a flowchart to take you through all the different forks and decisions you need to make every time you make a move.

<a href="/Flowcharts1.0/APAW-Flowchart-Moving-Light.png"><img src="https://github.com/soggymuse/Obsidian-Apawthecaria/blob/main/Flowcharts1.0/APAW-Flowchart-CharacterCreation-Light.png?raw=true" height="200px" /></a>

_Click image to see bigger version_

It's available as an [Obsidian canvas](/Flowcharts1.0/APAW-Flowchart-Moving.canvas) to save directly into your vault, and as a (huge) [PNG](/Flowcharts1.0/APAW-Flowchart-Moving.png) for those of you who'd prefer to be able to view it elsewhere. (Now includes Soaring.)

#### Character Creation Flowchart
This part's not nearly as confusing, but I thought it still might come in handy to have a flowchart for it.

<a href="/Flowcharts1.0/APAW-Flowchart-CharacterCreation.png"><img src="/Flowcharts1.0/APAW-Flowchart-CharacterCreation.png" height="150px" /></a> <a href="/Flowcharts1.0/APAW-Flowchart-CharacterCreation-Light.png"><img src="/Flowcharts1.0/APAW-Flowchart-CharacterCreation-Light.png" height="150px" /></a>

_Click image to see bigger version_

It's also available as an [Obsidian canvas](/APAW-Flowchart-CharacterCreation.canvas) and a PNG in both [light](/APAW-Flowchart-CharacterCreation-Light.png) and [dark](/APAW-Flowchart-CharacterCreation.png) modes.

## Statblocks
I was using statblocks from the [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin for things like character sheets and encounter cards.

You need a few things for these templates to work:
1. [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) installed and enabled
2. The **JSON** file for whichever statblock you want to use
3. The matching **template** (.md file) for whichever statblock you want to use.

The [CSS snippet](/FantasyStatblocks/APAW-Statblock.css) for the statblocks is *optional*. Mine make my statblocks match the main colours from the Apawthecaria map, but you can stick with the plugin's default or style your own. I wrote this snippet before I learned how to use theme variables, so you'll need to go through the **Set up Variables** section at the top and change all the colour hexes (e.g. <code>--statblock-background-color: #C0AD9B;</code>) to suit your theme.

### Non-player Character Sheet

<img src="/FantasyStatblocks/APAW-NPC-Statblock-Long.png" width="300px" />

*With extra line for "notes"*

<img src="/FantasyStatblocks/APAW-NPC-Statblock.png" width="300px" />

*Without line for notes*

The NPC statblock is short and designed for quick notes about characters you meet on the road. You can get the JSON for the statblock [here](/FantasyStatblocks/ApawthecariaNPC.json) (to import through the Fantasy Statblock plugin) and the markdown template [here](/FantasyStatblocks/FSB-APAW-NPC.md) (to save in your templates folder).

**Note:** I also use the NPC statblock for location cards (like for Odoak) to save on layouts. Just have the name, image, location, and description fields, and you'll get something like this:

<img src="/FantasyStatblocks/APAW-Location-Statblock.png" width="300px" />

*Image created with [NightCafe AI](https://creator.nightcafe.studio)*


### Ailment Cards

<img src="/FantasyStatblocks/APAW-AilmentCard.png" width="300px" />

This is a great way to copy the ailments from the PDF into Obsidian. You can link to tables that list [TAGs] for easier research for reagents. And you could have a rollable table that links to all the ailment cards in your vault so you can go right to the ailment when you come across a patient who's suffering from it.

The JSON for the statblock is [here](/FantasyStatblocks/ApawthecariaAilment.json) (to import through the Fantasy Statblock plugin) and the markdown template is [here](/FantasyStatblocks/FSB-APAW-Ailment.md) (to save in your templates folder).

## Dataview Templates

I use Dataview for my Sourcebook content now; they're much more pliable and useful than statblocks.

These templates use the YAML frontmatter functionality built-in to Obsidian to set the information, along with a Dataview template to use it. You can then use another Dataview template to index and filter all ailments in your vault. 

You'll need the [Dataview](https://blacksmithgu.github.io/obsidian-dataview/) plugin to make them work as intended. You'll also need my `snippets.css` file if you want your templates to look like mine.

### Templates Explained

I use three different custom callouts for all the templates in my vault: `[!ailment]` `[!reagent]` and `[!recipe]`. , `[!ailment]` is really just a standard callout with no icon so you could use any of the default callouts instead, whereas `[!reagent]` adds a border and `[!recipe]` has two columns for ingredients and instructions.

**Note:** Not all fields are used in all templates.

|Field|Description|
|---|---|
|Game|Useful if you have home-brewed content or content you've "borrowed" from other games that you might need to filter out.|
|Level|"1 - Novice" to "4 - Dire" helps you filter out ailments you can't handle yet. I also use "1" to "4" to sort my equipment.|
|Card|`A` to `K` lets you sort your indices or filter content according to the card you drew.|
|Timer|The time you have to treat an ailment.|
|Attributes|Used for ailment [TAGs], skills like APPLY/COOK, Familiar bonuses, etc.|
|Season|Lets you filter content by the season it's available. I also use this field to indicate rarity modifiers (e.g. Spring BR+3).|
|Description|The description provided in the Sourcebook.|
|Consequences|A list of potential outcomes and consequences.|
|Campaign|Name/date stamp (e.g. "Miska03") which journey you're on so you can review your journal and remember what happened when. I also use this field to mark when I got equipment.|
|Treatment|Link to the recipe(s) you used to treat this ailment.|
|Payment|A quick overview of how much RP and how many trinkets you gained. I use this to summarise and make sure I haven't added too much to my inventory at the end of a journey.|
|Location|Where content is available. I use this to filter reagents and make sure I'm not buying equipment I don't have access to yet. Also used for rarity modifiers (e.g. Forest BR+3).|
|Ailment|Used in recipes to link to the ailment it's for.|
|Type|Very versatile. I use it to indicate if equipment is a basic/advanced tool, if a location is a city/settlement, if a reagent is plant/earth/insect, if an encounter is social/travel/foraging, etc.|
|image|If you want an image in your note, put it here (e.g. "Dunleith.jpg") and the template will insert it. This way, you can also use images in indices.|
|Patient|Name of patient you treated. I only create NPC notes for recurring characters now so I don't link them here, but I do like to add what kind of animal they are in brackets after their name.|
|Guild|Kind of redundant because you could add this to Attributes and I may be merging them, but I currently use it to show which Guild an NPC belongs to.|
|Cost|How many trinkets/hours something costs. I just use the number so I can use the same field for trinkets (equipment and reagents) and hours (knitting projects).|
|Weight|I have vague thoughts about converting the Sourcebook's way of indicating weight (I use ⬡ ◔ ◕ ⬢ because they're available in the emoji finder on MacOS).|
|BaseRarity|The base rarity of a reagent.|
|Potency|The potency rating of a reagent.|

## Coming Soon

Dataview templates for indices.
