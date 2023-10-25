# BackGround XL (bg)
*formerly known as "[Landscape XL](https://civitai.com/models/160192)"*

Creating stunning, randomly generated landscapes as wallpaper (my main intention) or to use as backgrounds for your characters.

*The recommended "official" wildcard prompt will ***___NOT___*** work, as this requires ***__Dynamic Prompts__***!*

Keep in mind, the core intention was to create wallpapers for myself!
* 1720 x 720 === 3440 x 1440 (21:9)
* 1280 x 720 === 1920 x 1080 (16:9)

For characters / portrait, I would recomend:
* 768 x 1024
* 896 x 1152

To see screenshots generated with this DynPrompt, please see my CivitAi page: \
https://civitai.com/models/160192

-------------------------------------------------------------------------------------

### ___Requirements:___

* [Dynamic Prompts](https://github.com/adieyal/sd-dynamic-prompts)
	* Start WebUI
	* goto "Extension"
	* then "Install from URL"
	* enter / paste: ``https://github.com/adieyal/sd-dynamic-prompts.git``
	* hit "Install"
	* Reload UI

### ___Installation:___

* Simply put the contained folder "bg" into: 
	* ./extensions/sd-dynamic-prompts/wildcards
* So you get/have:
	* ./extensions/sd-dynamic-prompts/wildcards/bg
* After that, just make sure that you hit that "Refresh Wildcards" button \
	at the bottom of the "Wildcards Manager" tab.


-------------------------------------------------------------------------------------

## Basic Usage:

To create a complete randome image in whatever style your model favors:

	__bg/wallpaper__

My personal favorite is to force photos, however, some effects *might* change it to different styles.

	__bg/wallpaper__
	__bg/photo__

One of my favorites is: \
*however, art is already included in the wallpaper, but with a 1:4 chance*

	__bg/art__
	__bg/random__

## Negatives:

Of course you can use your own negatives, but I do have prepared them as well. \
That said, you might want to add "text" for the char negative, but since I know that some people like to use text in combination with characters, I did not "hardcode" it.

A general negative for wallpapers:

	__bg/neg__

And the specific one for the use with characters:

	__bg/char/neg__

## Use as character background:

For the use with characters, I'd recomend either:

	( your character description )
	__bg/char__
	__bg/anime__

Or go more.. specific:

	( your character description )
	__bg/char/aio__
	{ __bg/city/fantasy-char__ | __bg/city/scifi-char__ | __bg/city/modern-char__ |__bg/city/mystery-char__ }

If you find defining your character as difficult, \
or if it annoys you to write so many different (SFW + Skimpy/NSFW) prompts to get random characters / females, \
I have a solution for you.

* SD-DynPrompt-Char (WIP, unpublished yet)
	* [GitHub](https://github.com/sri-arjuna/SD-DynPrompt-Char)
	* [CivitAI]()

The latest / newest version of this readme, can be found at: \
https://github.com/sri-arjuna/SD-DynPrompt-BG




-------------------------------------------------------------------------------------

## Detailed Usage:

These are all options I've designed for you to use.

Please keep in mind that all "calls" have to look like:

	__bg/<call>__

### Styles

Two different approaches:

| Call (bg/)	| Description				|
|---------------|---------------------------|
| photos		| Should force photo-like images |
| anime			| Should force anime-like images, also relies heavy on the model used! |
| random 		| This produces various styles, from pixelart, to oilpainting, and many more. However, due to the "random" factor, some styles dont get applied as prominent as others - depends on the model used as well as other factors. |

If you want to use all styles, you can use the following:

	{ __bg/photo__ | __bg/anime__ | __bg/random__ }

While the following ones are used automaticly by the "city" files, you could also use them for other images of yours:

| Call (bg/)	| Description				|
|---------------|---------------------------|
| styles/aio-anime | Picks different effects and drawing artists of the genre. |
| styles/aio-fantasy 	| 	|
| styles/aio-mystery 	| 	|
| styles/aio-scifi 		| 	|
| styles/asorted 		| This contains some asorted styles, obviously.	|


### Background / Wallpaper:

| Call (bg/)	| Description				|
|---------------|---------------------------|
| city/fantasy 	| Shows a fantasy city, usualy as a "backdrop" in the landscape 		|
| city/modern 	| 		|
| city/mystery 	| 		|
| city/scifi 	| 		|
| nature/aio	| Prints a random landscape		|


### Character:

| Call (bg/)			| Description			|
|-----------------------|-----------------------|
| city/fantasy-char 	| Shows a fantasy city, chance to call its according ./building/ section 	|
| city/modern-char 		| 															|
| city/mystery-char 	| 	 														|
| city/scifi-char 		| 															|
| city/building/fantasy | inside/outside of a 'specific' building.					|
| city/building/modern 	| 															|
| city/building/mystery	| 															|
| city/building/scifi 	| 															|
| nature/char 			| Prints a random landscape which has human influence		|


___***Example:***___ \
Say you have my "Char" prompt and want a fantasy theme:

	__char/rp-sfw__
	__bg/char/aio__
	__bg/city/fantasy-char__


# Trigger words:

	__bg/wallpaper__
	__bg/art__
	__bg/city/aio__
	__bg/city/char__
	__bg/nature/aio__
	__bg/nature/char__
	__bg/char/io__
	__bg/neg__
	__bg/char/neg__

# More "optimized" trigger words:

	__bg/city/fantasy__
	__bg/city/modern__
	__bg/city/mystery__
	__bg/city/scifi__
