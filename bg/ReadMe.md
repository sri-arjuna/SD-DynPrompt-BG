# BackGround XL (bg)
*formerly known as "[Landscape XL](https://civitai.com/models/160192)"*

Creating stunning, randomly generated landscapes as wallpaper (my main intention) or to use as backgrounds for your characters.

*The recommended "official" wildcard prompt will ***___NOT___*** work, as this requires ***__Dynamic Prompts__***!*

Keep in mind, the core intention was to create wallpapers for myself!
* 1720 x 720 === 3440 x 1440 (21:9)
* 1280 x 720 === 1920 x 1080 (16:9)

For characters / portrait, I would recomend:
* 512 x 1024
* 896 x 1152

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
* So get/have:
	* ./extensions/sd-dynamic-prompts/wildcards/bg
* After that, just make sure that you hit that "Refresh Wildcards" button \
	at the bottom of the "Wildcards Manager" tab.


-------------------------------------------------------------------------------------

## Basic Usage:

To create a complete randome image in whatever style your model favors:

	__bg/wallpaper__

You can also set it to a certain style, or go complete random:

	__bg/wallpaper__
	{ __bg/photo__ | __bg/anime__ | __bg/random__ }

One of my favorites is:

	__bg/art__
	__bg/random__

## Use as character background

For the use with characters, I'd recomend either:

	__bg/char__
	__bg/anime__
	( your character description )

Or go more.. specific:

	__bg/char/aio__
	{ __bg/city/fantasy-char__ | __bg/city/scifi-char__ | __bg/city/modern-char__ |__bg/city/mystery-char__ }
	( your character description )

If you find defining your character as difficult, \
or if it annoys you to write so many different (SFW + Skimpy/NSFW) prompts to get random characters / females, \
I have a solution for you.

* SD-DynPrompt-Char 
	* [GitHub](https://github.com/sri-arjuna/SD-DynPrompt-Char)
	* [CivitAI]()



-------------------------------------------------------------------------------------

## Detailed Usage:

These are all options I've designed for you to use.

Please keep in mind that all "calls" have to look like:

	__bg/<call>__

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
| city/modern-char 		| 		|
| city/mystery-char 	| 	 	|
| city/scifi-char 		| 		|
| city/building/fantasy | inside/outside of a 'specific' building.					|
| city/building/modern 	| 															|
| city/building/mystery	| 															|
| city/building/scifi 	| 															|
| nature/char 			| Prints a random landscape which has human influence		|


___***Example:***___ \
Say you have my "Char" prompt and want a fantasy theme:

	__bg/char/aio__
	__bg/city/fantasy-char__
	__char/fantasy-sfw__

-----------------------------------------------------------





Currently updating in progress, text/images might not yet reflect what you get.

> 	This will NOT work with the "official wildcards" extension!
	See below for requirements!

*I tried to implement variations from natural aestetics, over futuristic scenery to mystical fantasy scenes.*

Works well with all checkpoints I had tested. Probably any/all checkpoint available, to different extends though.
However, I've gotten the best results using the 3 recomended resources below.


# Usage:

All pictures were made using this prompt to create stunning photo-like wallpapers.

	__landscape/aio__
	((photo raw))

or 

	__landscape/aio__
	__landscape/render-photo__















If you want to use a character of any kind, I highly recommend to use the following preset:

	__landscape/aio-char__

	__your-char-prompt__

	__landscape/render-photo__

For the example char images shown, I've used:

	__landscape/aio-char__

	{ __fake/act-custom__ | __fake/act-custom__ wearing a {elegant|gala|traditional} dress }, 

	__landscape/render-photo__ , __landscape/render-char__


# Optional:

If you feel lucky, instead of "photo", you can use the following to get one of of over 12'000 possible style combinations in total!

	__landscape/render-random__

For the negative prompt - specificly if you want to use for your character or whatever, I highly recomend to use at the very least:

	text, watermark

If you want to create wallpapers, I recomend to use my negative preset:

	text, __landscape/render-neg__ 

Likewise if you want to specificly promote your character, you can use:

	text, __landscape/render-neg-char__ 


# Requirements:

* [Dynamic Prompts](https://github.com/adieyal/sd-dynamic-prompts)
	* Start WebUI
	* goto "Extension"
	* then "Install from URL"
	* enter / paste: ``https://github.com/adieyal/sd-dynamic-prompts.git``
	* hit "Install"
	* Reload UI


# Installation:

Simply put the contained folder "landscape" into: 

	WebUI_DIR""./extensions/sd-dynamic-prompts/wildcards

So get/have:

	WebUI_DIR""./extensions/sd-dynamic-prompts/wildcards/landscape

After that, just make sure that you hit that "Refresh Wildcards" button 
at the bottom of the "Wildcards Manager" tab.

--------------------------------------------------------

### Notes:

* While the main intention is/was to generate wallpapers for my deskopt that I like, it therefor has a certain "bias" towards sci-fi + high fantasy visuals.
* That said, I also like photos of natural aestetics, art if you will, very much.
* So I tried to provide an equal variation of those 3, this will be the most likely reason for updates
