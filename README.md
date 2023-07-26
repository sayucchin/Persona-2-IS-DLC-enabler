# Persona-2-IS-DLC-enabler
This mod will make the Imported Films menu item visible in the theater and make it possible to play DLC quests. It does not include the quest creator, Single Theater or Independent Film menu categories. If you have created a quest yourself in the Japanese version of the game (Single Theater quest) you will still not be able to play it with this mod. The Single Theater quests are saved in a different format and will not be recognized by the game. Apart from the Dark Shadow trilogy, the Imported Films were collaborations between Atlus and games media organizations in Japan to showcase the capabilities of the Quest Creator. We have not included the quests themselves nor any game ISOs in this mod, only patches for you to modify your own files. Please note that the quests are not necessarily canon and may contain offensive content. 

Patching instructions

Patch the ISO:
Drag your Innocent Sin ISO file to the patcher.exe, both North American and European releases will work. It will not overwrite your original ISO, it will create a new copy called P2IS_modded.iso in the same folder as the patcher.exe. You do not need to touch any of the individual patch files in the dist folder. 

Please note that if you are running an already decrypted and modified version of the game such as an HD mod or undub mod, the patcher may not work. It might be compatible with the undub mod but we make no guarantees. 

Once you have patched the ISO you have to be careful with the "Install Data" option in the config menu. That option saves data from the UMD onto the PSP's memory card but it is useless if you are already running a digital version of the game and will not speed up load times! It will instead potentially corrupt your game files and make it crash. Don't ever click it! 

Patch the DLC quests:
Obtain a copy of the original Japanese quests, they were distributed as freeware on the PlayStation Store but the servers have gone offline, you'll need to find an archived copy from elsewhere.

You should have a folder called NPJH50329 containing 9 files:
PARAM.PBP
quest01.EDAT
quest02.EDAT
quest03.EDAT
quest04.EDAT
quest05.EDAT
quest06.EDAT
quest07.EDAT
quest08.EDAT

Select all the quests.EDAT files and drag them onto the patcher.exe. The patcher will decrypt and translate the quests and place the output files in a new folder called "quests".

Place the files in the right directory:
Move the newly created quest.EDAT files from the quest folder over to the PSP/GAME folder. Remember to copy the original unmodified PARAM.PBP from the NPJH50329 folder over as well.

For the European version of Innocent Sin make a folder called ULES01557 and place the 9 files in there, that will let your European ISO file recognize the quests and play them. For the North American version, name the folder ULUS10584 instead. 

Directory pathways on original PSP:
Quests and param.pbp go here: PSP/GAME/ULES01557 or PSP/GAME/ULUS10584 
Put the modified ISO for the game in the GAME folder, not in the ULES/ULUS folder
-The psp has to be jailbroken for you to be able to add your own files to the memory card. 

The PSVita places the PSP directory in the pspemu folder:
ux0: pspemu/PSP/GAME/ULES01557 or ux0: pspemu/PSP/GAME/ULUS10584 for the quests + param
The ISO file should be placed in ux0: pspemu/PSP/ISO rather than the game folder
-The PSVita has to be jailbroken for you to be able to add your own files to the memory card.

PPSSPP copies the original PSP directory structure perfectly:
PPSSPP/PSP/GAME/ULES01557 or PPSSPP/PSP/GAME/ULUS10584 for the quests + param file
PPSSPP can load up an ISO from anywhere on your PC so you can keep it wherever you want and find it in the recently played screen. 

Bonus:
If you are interested in the bonus quest, then move the file quest09.EDAT from the bonus folder into the same folder as the other 8 quests and the param file. This is an exp farming quest. The Japanese version of Innocent Sin PSP came with a quest creator which Atlus hoped that the fanbase would use to generate infinite new Persona content. But it could also be exploited for fast exp farming which ended up being the main way people used the editor. This bonus quest is an example of those kinds of farming quests so that you can easily level up your entire party when you want,  without having to slowly grind Alice encounters under the factory. Please note that this bonus quest was not built using the editor, it was written manually. If you are having trouble navigating the dungeons in the quests you can check the walkthrough in the bonus folder. If you are still struggling then you should check out the maps available at https://w.atwiki.jp/persona2tsumi/pages/67.html

Credits:
Eiowlta: Programming
DarTisD: Programming
Sayucchi: Translation, Editing
Polyglot Sammy: Translation
Gabriulio: Translation
Apollo: Proofreading

The patcher uses code from PPSSPP in order to decrypt the eboot.bin and the EDAT files. Additionally, https://github.com/wmltogether/CriPakTools was used as a reference for the cpk code. xdelta3 is used for patching the files. The source files for this mod are available in patcher_src_zip.

