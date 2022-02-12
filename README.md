# LangDetect_Kab_Files
Adding support for Kabyle language (ISO 639-2 code “kab”)

I have added the language profile "kab" (obtained with the command java -jar langdetect.jar --genprofile)

Profile created using a Wikipedia export from kabwiki-20220120-abstract.xml.gz from wikipedia dumps site: https://dumps.wikimedia.org/kabwiki/20220120/

Installation (how to use "kab" in language detection):
1. Install "LangDetect" using https://github.com/Mimino666/langdetect
2. Add profile "Kab" file store here in this repository to the "LangDetect" installation folder
3 Testing: Run command "Python detect_lang.py"


Details for generating "kab" language profile (you only need to do this in case you want te regenerate another "kab" profile)

Steps provided here: https://code.google.com/archive/p/language-detection/wikis/Tools.wiki

Downloaded  langdetect.jar

Download and use new jsonic version (>1.2.5)  from http://www.java2s.com/Code/Jar/j/Downloadjsonic125jar.htm
(to fix error Exception in thread "main" java.lang.NoClassDefFoundError: net/arnx/jsonic/JSONException)

Run command java -jar lib/langdetect.jar --genprofile -d [directory path] [language codes]

Make sure that [directory path] contains only the file kabwiki-20220120-abstract.xml.gz  and nothing else.
Under [directory path], you need to have a subfolder named “profiles” that will store the generated language profile “kab”

Misc Troubeshooting: https://github.com/Mimino666/langdetect/issues/5

Note: 
In linux, you need to copy the profile generated “kab” into installation folder of LangDetect folder such as : .../lib/python3.7/site-packages/langdetect/profiles


