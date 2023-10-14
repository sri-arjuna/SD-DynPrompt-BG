Creating stunning, randomly generated landscapes to use as backgrounds for your characters, as wallpaper (my main intention) or whatever.

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
