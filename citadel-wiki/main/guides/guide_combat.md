Updated to citadel/master (coder talk for latest) 3/7/2020 - kev

If someone wants to clean this up please do because there is a reason I do not write/edit wikis/write in general/I hate writing

With it kept in mind that I am a CODER and most definitely not a WRITER, apologies in advance if you don't know what the heck I'm talking about.

SOMEONE PLEASE ATTACH IMAGES BECAUSE NEW PLAYERS NEED THOSE!

**Expect all of this to be mostly accurate but keep in mind that code changes happen fast, infact as of time of writing there's several changes to the below in the works.**

## General

Citadel station operates off some '''quirky''' mechanics you won't see anywhere else.

This is just a list of quick things on what the seriously-different-things are.

**Stamina Combat**
: Most "combat" actions take stamina to do. Everything from firing a gun (not a lot of course), bashing someone with an item/stabbing someone/etc (melee attacks, stamina usage depends usually on how big the item is and isn't going to scale consistently with damage, keep that in mind), throwing things (a decent amount) or people (quite a lot!) and other actions. Your stamina is shown by the lightning bolt on your HUD on the right side. The less it is, the less you have. If there's a flashing exclamation mark you're in stamcrit. More on that later. Your main stamina health pool does NOT regenerate while in combat mode. Try to use it sparingly.

**Stamina Buffer**
: You also have a stamina buffer (denoted by the white 'gauge'-like outline outside of the lightning bolt). In general, actions YOU take (like beating someone, shooting someone, throwing things, shoving yourself off the ground among other things) will take from this buffer before using your stamina "health".This regenerates constantly and you don't need to be out of combat mode.
**Combat Mode**
: Hotkey bound to C, also a button on screen. Generally something you want to be on while in combat, you do reduced melee damage without it, you get hit for more damage in melee without it, you can't do some specific things (like shoving yourself off the ground) without it, your gun is inaccurate without it, etc etc.

**Sprint**
: Citadel has a sprinting feature. You get a small buffer of sprint that you can use, afterwards it'll do direct damage to your main stamina health (as opposed to your stamina buffer). You move a bit faster while in sprint (and due to strange mechanics in game this is most effective if you were already fast). This is based on TILES MOVED rather than TIME. This means you lose more buffer/stamina while sprinting the faster you're actually going.

**Stamcrit(ted)**
: If you run out of stamina you get stamcritted. There's soft, and hard stamina critical (stamcrit) at 100 and 140 respectively. If you're in '''soft''' stamcrit, you in general can not attack or do outgoing hostile actions like firing guns using melee and similar things. You can use things like spells if you have them though. You can still move in this state but can not crawl under people or shove yourself off the ground (or get off the ground at all). If you are in '''hard''' stamcrit, you can't do anything but use spells and other things that don't require.. well.. stamina or hands to use. You're just stuck on the ground and hard-stunned like how it works in other servers. People can still shake you up with varying effectiveness in either soft or hard stamcrit (it'll generally regenerate some stamina for you if they shake while in hard stamcrit)

## Combat Mode

**Combat mode in general is needed to be relevant in combat. Not having it on will give your character a lot of debuffs (weaknesses).**
* Any nonhumanoid (so anyone who isn't /mob/living/carbon/human in code, so almost everyone but you unless you are a non-human) is in effect always in combat mode. <s>The game was rigged from the start</s> Luckily for you, only cyborgs get actually increased damage if you aren't in combat mode (citation needed).
* All of the below stack with any other multipliers/buffs/debuffs.
* **Not having combat mode on decreases your outgoing (inflicted on others) melee damage from item attacks by 50%.** (I say this specifically because this is different than the assumed inverse of this statement)
* **Not having combat mode on increases your incoming melee damage from item attacks by humans/silicons by 50%.**
* That's a total of 150% damage if you are not in combat mode, from someone in combat mode. This means you can kill people far quicker and easier if they are either not in combat mode, or hard-stamcritted, and in general surprise attacks are more powerful because most people won't have it on all the time.
* **Not having combat mode on will make guns have random angular dispersion (non coders/nerds: this is inaccuracy).**
* This applies to punching too. 
* **Your stamina health pool does not regenerate while combat mode is on.** Your stamina and sprint buffers, however, will.
* **You will always face towards your cursor while combat mode is on, and you are able to use your right click mouse button.** By default, right click is the same as left click except for certain actions like shoving instead of disarming in unarmed-disarm-intent-attacking, stunbatons disarming instead of knockdown + stamina damage, tasers alt-firing, energy weapons switching modes instead of firing, etc etc. 
* See: Sprinting/jogging/walking section for "direction you face vs direction you run".
* **You can clickdrag items from your inventory to things as a human if you are in combat mode to instantly draw that item and use it on the thing you dragged it to** if it is in your inventory, reachable by you, and your selected hand is free. This is pretty powerful if you do it flash-->cyborg, as they won't have time to disarm you, same with batons and similar. In reality, no one will do this even if they know this is a thing.

*<s>No one wanted to know this, but turning on combat mode disables vore mode.</s> Yeah for uhh, those who are into that stuff.

## Stamina

* You have a stamina health pool separate from damage. Both of them are taken into account for calculating how fast you move (slower = more damaged), but you cannot be stamcritted from physical/health damage, nor can you be critted (so dying from health loss) from stamina damage.
* Combat mode is off if you have are hard-stamcrit. This is bad for you as seen above by its effects.
* Stamina critical (stamcrit) comes in two flavors. Soft, and hard stamcrit. Soft makes you unable to fight back (much, there's still stuff that can work for you) but you can for the most part still walk around (or crawl if you get knocked down since you can't get back up while in soft) and do things. Hard makes you hard-stunned, with a darkened "filter" so people can see you are hard-stamcrit, turns your combat mode off.

## Sprinting(/jogging/walking)

* Sprinting has a cost. This is based on tiles instead of time. The further you go while in sprint, the more of this cost you will incur.
* Cost goes into the sprint buffer (the bar above the sprint button) before your stamina health pool, not buffer. If you sprint too much you will be easier to stamcrit. Manage your sprint and stamina.
* If you sprint off a table, you will trip off and fall. Ouch!
* If you sprint you will slip on wet floors no matter what (wet, not lubed/iced, those you always slip on as long as gravity is on/there). If you are jogging, you only slip if your stamina is below 80%. If you are walking, you never slip. On water-wetted floors.
* Sprint buffer regenerates even if you are currently sprinting and helps offset the stamina damage you take if you sprint while it is empty. Obviously, it's not going to in effect regenerate if you keep sprinting while it's empty.
* The sprint buffer regenerates while in combat mode.

## Shoving
**You might have experienced this if you played on /tg/.**

* Pushes someone back.
* If they directly hit a wall, they get knocked down. Same if they hit a table (although they'll go on the table). If they hit a person, both the people get knocked down.
* Shoving someone twice in quick succession will forcefully disarm their gun (any /obj/item/gun in the code this won't work on flamethrowers and such). 
* Shoving someone also applies a brief slowdown. This is just happening to be what the above checks for in the code, so they're effectively the same duration. Pushing again will not refresh this duration, unfortunately, only re-apply it if it had already ran out.

## Punching

Don't do this. It uses a ton of stamina for a crappy randomized amount of damage. You will almost never realistically be in a situation where you don't have a better weapon. This is only nice for fistfights, not for murder.

## Disarms

This is still the stupid random-number-generator (aka luck) based feature like it was on /tg/ before they got smart and removed it. Unfortunately for us, we still are stuck with it.

* This works best if you have combat mode on and they don't. People who have combat mode on have a higher chance of disarming, and have even higher of a chance if the target isn't in combat mode. If you disarm someone without combat mode active while having it active it will be a near-guarunteed disarm.
* This is a random chance. Sometimes, you will instantly disarm someone with a dual-bladed energy sword, unarmed and in combat mode. Sometimes, you will never get it. This is a bad mechanic but can save your life if you're feeling lucky, as it works on all items, not just guns.
* In reality you have a decent chance of disarming if you're in combat mode so it's better to try to disarm than to do nothing or punch.

## Grabbing
Grabbing/pulling is the same thing.

* Aggressive or up grabs are the equivalent of an indefinite hard stun until they resist out of it.
* They can not resist out of it if they are laying down. Ouch.
* You can throw people if you have them aggressively or up grabbed.

## Crawling/resting
**On Citadel, much like most /tg/code derived servers, you can crawl around at a slow speed while on the ground.**

While you are on the ground, you do less outgoing damage (damage you inflict) in melee (in general, and I keep emphasizing this because there is a lot of code that doesn't care, like stunbaton stuns isn't going to be affected). This stacks with combat mode buffs/debuffs.

Bullets won't hit you while you are on the ground unless it's special (like fireballs will always hit things they fly near to) or the person clicks directly on you. This can be useful if you also have a gun, as you aren't affected by accuracy losses as long as you keep in the same direction and have combat mode on, and they have to dodge your bullets unless they lay down too and have to click directly on you. However, if you're actively resting, your projectiles won't be capable of passing through windows, tables, grilles, and other objects that your projectiles would otherwise be able to shoot through.

You can crawl under other people at a delay. You won't immediately just slide under them. This doesn't work if you are in stamcritted.

If you are on the ground, you cannot disarm people. They can disarm you and shove you, though.

Getting up off of the ground is slower the less stamina you have, at a quite unfair curve, meaning you are at a significant disadvantage as long as you have less than full stamina. Shove yourself up with combat mode, help intent right click on yourself. This will use your entire stamina buffer and use your stamina health if you don't have enough

**An advantage to crawling and resting is that your stamina health (not buffer) regenerates faster while on the ground.**

## Miscellaneous things you probably didn't know or realize that weren't or were poorly covered above

* If you are pulling or otherwise gripping someone, your disarms will have a higher chance of working (but at that point why not just grab again to upgrade to aggressive, which is a hard stun?)
* You run slower while not facing the same direction as your movement. This is really only relevant while in combat mode because you always face your cursor and without it you'll automatically be the same direction as your movement.
* Some items just flat out have better damage-to-stamina ratios than others. See: Welding torches. Those do 15 burn damage but just don't use a lot of stamina. Same with stuff like the nullrods, energy swords (to an extent anyways, it still uses quite a bit), etc etc.
* There's no downside to only having combat mode on while in actual melee combat (as in close enough to hit/be hit) if you're not using guns. There's no timers here. Squeeze every last drop of stamina regeneration out if you can.
* As of right now at the time of writing, guns are inaccurate if you change directions, even if you have combat mode on. This means keep your character facing the same direction to not suffer losses and only change directions with combat mode if you need to. 
* Things like shotguns that are loaded with buckshot and similar "this isn't accurate" things don't matter if they're inaccurate. Why bother being in combat mode/facing the same direction if it is always inaccurate and it doesn't matter?
* Most of you don't examine things. Stunbatons on disarm mode and on combat mode right click strike disarm people. Hybrid tasers shoot slowing tasers on right click too. The latter isn't too useful at the time of writing, the former will probably save your life.
* The stamina buffer helps you during the calculation for slowdown due to stamina damage. It doesn't seem significant but it can help you. A lot.

## Miscellaneous things that you won't care about
* Lag is a thing. When you click someone, that doesn't mean you hit them until the server gets the message that "I want to hit that person" and the server goes "Alright, are you currently next to them", both in layman's terms. 
* This means that if you click someone while sprinting while next to them, you'll have a chance of missing if you're lagging due to you being out of range by the time the server checks for this **proximity**
* This means that for optimal hitting at high speed/sprint, you need to click just before you get into range and hope that you can get out of range before they can do the same for you.
* This means that since none of us are robots with timing of atomic precision, this is the exact reason SS13 combat is called **clickspam** combat. There's still tricks to this along with how fast the game actually processes your clicks (click too fast and your clicks won't be as effective per click), of course.
* Melee attacks hit as long as they are/were in range when the server receives your click. Ranged gun attacks tend to only work if they're still there when your projectile hits. This won't matter. Until you are fighting a slaughter demon and realize that the faster melee processing speed is the reason you can melee them with a higher window of timing than using a gun. Same applies for greyshits running around on meth, you'll want to hit them with a hard hitting melee attack if you can't ranged them (obviously this is risky, don't listen to me and complain you died.)



* And since this isn't in the rules, '''keep in mind that no matter how hard you try or how much equipment and benefits you have, sometimes you just lose'''. Combat is never something you can always win, there will always be luck involved. The players that are the best in combat will still die to unforeseen factors or flat out bad luck. Do not be discouraged if you "lose". There is no losing other than giving up. Have a fun time, it's a game, and remember that combat isn't everything.

