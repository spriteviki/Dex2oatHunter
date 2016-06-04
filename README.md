# Dex2oatHunter

Dex2oatHunter aims at unpacking hardened dex file automatically.

Dex2oatHunter is based on the source code of Android runtime. It is composed of modified ART runtime. You can use the modified runtime to replace the original content in Android source codes (Android 4.4). The modification is mainly in "art/dex2oat/dex2oat.cc" (ART).

###Usage:

If you want to unpack an app, you need to install the app and start it . You can observe the log using "logcat" to determine whether the unpacking procedure is finished. Once done, the generated "xxx_class.dex" file is the wanted result which is located in the app's data directory.


###File description:

"demo.mp4" is the demonstration video of unpacking a hardened app by 360 and legu.

"test_legu.apk,test_qihoo.apk" are the samples used in the video.

"art/dex2oat/dex2oat.cc" is the modified file for dex2oat.

"image" 7z files contain the system image files used in the video.


If you use this code, please cite the following paper. Thanks!


#####Comment: 

I have tested the samples from 360 and Legu in May under ART. The result may be changed to multiple dex files and the dex file("../classes.dex_XXX.dex") is valid.
