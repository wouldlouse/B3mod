# Burghers, barley and bloomeries

This mod has a few key design goals:

- **To recentre the game from Europe**

    Europa Universalis IV is eurocentric by design as are most of its mods.
    This is a valid design choice;
    the game is fun and some argue that history was eurocentric during the time frame of EUIV.

    When the great divergence began and its extent is subject to debate[^divergence], but this is besides the point.
    Recentring the game from Europe would involve getting rid of ahistorical constraints from non European states (e.g. reworking institutions such as feudalism and renaissance).
    To rebalance the game, pops will be added and estates will be fleshed out to make industrialisation more dynamic and give the player more agency, which will improve gameplay both outside and inside of Europe.

[^divergence]: See [Frankema, E. (2024)](https://doi.org/10.1111/joes.12609).

- **To flesh out internal conflicts**

    In EUIV, states grow big and fast.
    It is rare for a state to collapse without the intervention of a bespoke mechanic (such as decadency for the Ottomans or the mandate of heaven for China).
    General mechanics for internal challenges to expansion exist but are not used as the game is balanced to favour playing "wide" and not punish expansion.
    As a result, players tend to stop playing after the 1500s, once no other states are strong enough to challenge the player.

    The estate mechanics in game give classes within the state some agency.
    Players do not face serious challenges from the estates however.
    Currently they exist to give the player early game buffs which they revoke for absolutism in the mid game.

    A combination of low governing capacity with harsh penalties and new estate mechanics to model class conflict will be used to challenge the player.
    Low governing capacity will force the player to keep subject states and makes expansion less useful in increasing state power.
    Estates will demand conflicting rights from the state, such as burghers demanding freedom from taxation and harassment from nobles while nobles demand the crushing of communes and reinstating noble control of towns.

    To increase "state power", the player will need to increase their governing capacity by building courts, paving roads and employing more bureaucrats.
    Additionally, playing estates off one another will open opportunities to strip rights from them and give the state more breathing room.

- **To represent historical diversity more accurately**

    Currently, cultural and religious minorities on a provincial level are not modelled in EU4.
    To model them, pops will be added.
    Pops are either urban or rural (the production and military dev of a province renamed) and will be represented as a province level variable.

    Cultures are put into exclusive groups of similar cultures.
    For example, the Catalan culture is part of the Iberian group and so isn't part of any other group.
    Despite Occitan culture being similar to Catalan culture, as Occitan is part of the French group these cultures are as alien to each other in game as Catalan is of Japanese.

    Culture will be replaced with language, the common language of the province.
    Languages fit the exclusive paradigm better than cultures, though there will still be edge cases.
    As minority languages cannot be represented on a provincial level using this system, "unaccepted" languages (languages the bureaucracy does not support) will only contribute to increased governing capacity and autonomy.

- **To represent population growth and decline**

    Development will be replaced by pops and wealth in the province.
    The pops in the province will increase passively, the rate depending on the terrain, prosperity and wealth.
    Low province loot, devastation and occupation will decrease the pops in a province.
    This makes war costly, especially multiple wars over the same region.
    Wars like the thirty years war and the Ming-Qing transition will depopulate areas rapidly.
    This also incentivises building forts all over the hinterland.

## Usage
Clone the repository into your mod folder[^modfolder], copy `description.mod` from inside the cloned repo into the mod folder and rename the file to `B3mod.mod`.

[^modfolder]: Usually `%HOMEPATH%\Documents\Paradox Interactive\Europa Universalis IV\mod` on Windows.
