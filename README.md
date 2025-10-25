# Translation of SEGA AGES 2500 Series Vol. 26: Dynamite Deka
### A.K.A. the PS2 port of Die Hard Arcade
###### By way of emulator-assisted texture replacement

<p align="center">
  <img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreigxonqweyhzyvddrrj64tewwo2bd2w7fzu6h6dcf2a3jarnxuplpe@jpeg" width="400"/> <img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreifyzw6j6nv65fpub5bixlfco5ssxkakwnvhb5dkkwgdmc6pvpmjle@jpeg" width="400"/>
  <img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreicyyzx3s5x3fdhbboniay3dhskgypnxki6p2bapsjxsxv4fulfdry@jpeg" width="400"/> <img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreicjuf7szodatdsns5ffmq2cqxnva3bnkmfeictoews7n4cdreckfy@jpeg" width="400"/>
</p>

Because of Die Hard Arcade's nature of being developed as a (very loose) adaptation of American IP first before being adapted into an original title, all things related to the main scenario were already in English, including the main weapon icon banners used in the Arcade/Saturn game - the only change in adapting Die Hard Arcade to Dynamite Deka was the iconography, changing the QTE prompts to Japanese Kana, and some added subtitles with *very* loose translations of the (still) English dialogue.

However, when Deka 1 was remade for the SEGA AGES series on PS2 (maintaining all the changes of the original Dynamite Deka release, only with some slightly tweaked typography), they also took the time to add several new features, including:
- An extensive gallery of original assets and marketing material for the original release
- A full graphical refresh of the game bringing the aesthetic closer to, and in many cases beyond that of *Dynamite Deka 2,* A.K.A. *Dynamite Cop!*
  - *...alongside* a true-to-Saturn mode (aptly titled *SEGASATURN MODE* with original artwork and bright models reminiscent of the Saturn/ST-V hardware (without texture wobble)
- Replaces the original *Deep Scan* subgame for a virtual recreation of Sega's electro-mechanical [*Periscope*](https://en.wikipedia.org/wiki/Periscope_(arcade_game)), complete with a fully modeled original cabinet!
- Several new modes of play built around the *DYNAMITEDEKA* mode that are exclusive to this port

While this extra content largely pulls from the base game, it also features many new weapons freshly made for the PS2 game with their own Japanese typography in contrast to the main arms. All of this content makes for the single *best* version of Die Hard Arcade/Dynamite Deka 1 available... as well as a *very jarring* mix of Japanese and original English assets in a game that's otherwise completely legible and easy to pick-up-and-play for English-speaking audiences, save for the QTE prompts.
___
<img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreifw5c7nostajymun3fae4qrmilhclruxypno7yhc2dkzjy6nvffta@jpeg" align="right" width="512"> This repo serves as a Texture Replacement Pack for SA26:Deka1, for use with *[PCSX2](https://github.com/PCSX2/pcsx2)* v2.0 or newer.

**At the moment, this is *not* a proper translation hack for Deka1, and will not work on original hardware as it is,** but can be played on devices that can run basic PS2 games (as low as a Retroid Pocket 4, and will run on virtually any x86_64 PC that PCSX2 supports these days). The hope here is that this project will serve as a potential resource for any aspiring brainier individuals that wants to take a crack at hacking these changes directly into the game.

#### As of now, this texture pack covers the following:
- Iconography depicting "Dynamite Deka" has been reverted to "DIE HARD Arcade" when possible - currently the title screen and rolling demo, save for the title menu (which uses a partially unique art with the logo baked in).
- All dialogue in the main scenario & attract mode have the Japanese translations replaced with direct transcriptions of the English script.
  - At least three of these subtitles - all of which happen to be consecutive across the end of Stage 4 and the boss of Stage 5 - are extra squished in comparison to the others due to the size of the original texture they accompanied. The Japanese script, in many cases, tends to be as wordy if not wordier than the English dialogue, but in these cases they are comically truncated down to fewer words (So somehow, the line *"Ah, so the cat has found the mouse"* turned into just *"Little girl"*), and these instances have a smaller texture size to accomodate. This is where a hack would be preferable. 
  - For whatever reason, the attract mode line from the radio chatter "We'll have to get her out, as soon as possible. Over." is not subbed at all, meanwhile the lines "Roger, we've got a bad situation down there." and "We've got a band of terrorists..." are merged into one text blob in the Japanese subs. These are true to the original NTSC-J Saturn/ST-V version, which this port directly lifts from.
  - Main scenario dialogue is shared across all modes, including *DYNAMITEDEKA* sub modes and the *SEGASATURN* mode, so they will all be translated the same.
- In-game button prompts "PUSH PUNCH/KICK/JUMP" are reverted back to English.
- Menu button prompts are translated into English, which covers the *Gallery* submenu in the options and *Periscope* mode.
- Congratulatory screens upon completion of a mode are a work-in-progress - currently only the screen detailing how to unlock *DEADLINE* mode is translated.
- The weapon icons for the new arms added to the sub modes are partially translated, with redone and retraced assets for at least twelve of the added weapons made from scratch to match the existing Die Hard Arcade banners as closely as possible.
- The banners for the Gallery items are currently *not* translated, but should be for completion's sake.

### Installation
Download a copy of this repository, either directly via `git` or by clicking GitHub's green *"Code"* icon, then *"Download ZIP"*. Extract/move the root folder, which should be `SLPM-62717`, to wherever you set PCSX2 to look for texture dumps/replacements; by default, it should be `PCSX2/textures` for portable/Windows builds, and `~/.config/PCSX2/textures` for Linux Repos/AppImage builds.

### Notes
Remember that when modifiying textures for PS2 emulation, *they are all vertically flipped* and must remain as such when exporting to the working texture pack. Same goes for the textures, which only scales to an Alpha value of 128 which will appear half-transparent in most editing programs - the working/src assets are scaled to 0-255, and will need to be unscaled back to 128, either by merging all layers down to one and then setting to half-opacity by hand, or by way of [PCSX2's Python script](https://github.com/PCSX2/pcsx2/blob/master/tools/texture_dump_alpha_scaler.py).

This repo uses project files for Krita, which is my preferred image editing utility, but can be exported to other formats.

The Weapon grid background used as a base for all weapon UI assets is provided in `replacementsSrc/Weapons/_wpnBG_template.kra` and should be used as the baseline for all assets - refer to the other working files for the text.

Original Japanese asset dumps should be kept as a disabled layer in all src project files for reference.

<img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreiarnpz3zurrg2m32msap3rr2x4tpengnxbyidnz5ie72whiawmotq@jpeg" align="right"> Whenever possible, the original weapon outline should be restored/redrawn as its own layer, and the text should be layered on top of that as a modifiable Vector layer in as close to the original position/scale as is reasonable for the new English text, except in cases where the translated name is bigger - else, follow the template of the existing Die Hard Arcade weapon banners, since they are the look we're aiming to achieve consistency with.

It's a good thing to note that more than a few added Deka weapons are actually directly referencing real world objects or trade names, such as [Maglite](https://en.wikipedia.org/wiki/Maglite) and [Česká zbrojovka](https://en.wikipedia.org/wiki/%C4%8Cesk%C3%A1_zbrojovka_Uhersk%C3%BD_Brod), and others like `d166f2fb2cd5d004-138b579cd327df0-00001dd3` are clearly a cheeky reference to other IP with a slightly different name; both cases should be preserved as much as possible.

On the other hand, others like `29ba9e08b1be22a2-8454bf5ed9f409ce-00001dd3` are objects that I'm not even sure what they translate to, as machine translation just gives garbage results - in these cases, some creative liberty is taken just as a placeholder, but should be corrected by someone that actually knows what it is.

Currently, all fonts are some stretched, squished, or emboldened variant of bog standard Arial, since it *sorta kinda* matches the original Die Hard Arcade banner fonts and prompts, and happens to fit in pretty okay with the existing English typeface used in the menus. Someone more design savvy might want to opt for a better/more fitting font instead?

<img src="https://cdn.bsky.app/img/feed_fullsize/plain/did:plc:jl65duvyqgjqafpa5oxa52fv/bafkreib5ow3uc7w2qq4vmb6nrdhpm55g3zxvlduqg4ytuv7erol5n2bjxq@jpeg" width="512" align="right"/> Yes, the website the game links to is down, but anyone playing games of this vintage (which are ports of an even *older* arcade title) should *probably* know what the Internet Archive is by this point. However, the codes don't seem to register on the current archived copies when I checked.
