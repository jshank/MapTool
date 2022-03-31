# RPTools Macros

## Bulk Assignable Damage
Select any number of JMR's monster tokens and this macro will replace the default damage amounts with clickable links. Highlight a target character and click the link to bring up the Takehara damage assignment screen.

## Renumber and Color Tokens
Select a group of tokens and activate this macro to rename them and append a number to each, started at the index of your choice. The macro will also assign a unique color halo to each token. Edit the macro to modify the colors or naming convension. 

## JMR Upgrade Monster Macros
This macro will search another map for tokens matching a specific naming pattern and then replace the macros on the current map with those. The original intent was to update JMR's Monster Tokens with new macros without losing the original details (other than the macros). This one has some fun features:

- Initial warning with abort on cancel
- Allow a map to be selected from a dropdown populated with all maps
- Replace macro logic based on a specific macrogroup (safer)
- Select target tokens based on a regular expression
- Easy inline commenting
- Colorized output based on success
- Example output when this macro is run:

```
Searching for Wolf...
Found! Replacing all macros.
 
Searching for Okre...
not found on source map, skipping.
 
Finished. Replaced macros on 9/10 Monster tokens. Check output for missing tokens
```

## JMR Rechargable Attacks
An example of a rechargable attack using Young Green Dragon's Poison Breath. The first click uses up the charge, changes the button name/color. The next click rolls for a recharge. If successful, the button is returned to the original state.