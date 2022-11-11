# myUDTree

Universal Dependency Tree for Myanmar Language  
We plan to announce/release soon ...   
***Still uploading files and updating the README file ...     

y  
10 Nov 2022  

## Introduction
	
The myUDTree corpus is a Universal Dependency (UD) Corpus that extends previous work of the Myanmar UD parsing (Hnin Thu Zar Aye et al., 2018), including 11,000 sentences of dependency tree data. The extended myUDTree corpus contains 43,196 sentences in total.  

Universal Dependencies (UD) Corpus is a type of corpus that is annotated according to the grammar rule of the respective languages with Part-of-Speech (POS), morphological features, and syntactic dependencies. Before building myUDTree, we built a [Joint POS Tagging and Graph-based Dependency Parsing (jPTDP)](https://github.com/datquocnguyen/jPTDP) model, using the existing in-house version of Myanmar UD corpus in order to parse raw data with dependency information. After building the jPTDP model, we selected 20,000 Myanmar sentences from our developing parallel corpora (i.e., from Myanmar-Chinese and Myanmar-Korean language pairs), and 12,000 Myanmar sentences from the ASEN-MT corpus built by [NECTEC Research Center](https://www.nectec.or.th/en/) in Thailand, and these data are parsed by using our built jPTDP model to obtain dependency-tree data.  

The parsed data were manually checked and corrected using the [CoNLL-U Viewer tool](https://urd2.let.rug.nl/~kleiweg/conllu/). After that, the revised data and the parsed output of the original Myanmar UD corpus were integrated to obtain the myUDTree corpus which contains 43,169 sentences with dependency information. Fourteen (14) Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) and 14 dependency relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) are applied in the previous work of Myanmar UD Corpus, and CoNLL-U format is used as a dependency-tree data format. The same number of Universal Part-of-Speech tags and dependency relations were also applied in our extended myUDTree corpus version 1.0. The following dependency relations are the most primarily utilized in Myanmar dependency structure.
  
1.	root (root) 
2.	acl (clausal modifier of noun) 
3.	amod (adjectival modifier) 
4.	advmod (adverbial modifier) 
5.	case (case marking) 
6.	mark (marker) 
7.	compound (compound) 
8.	obl (oblique nominal) 
9.	obj (object)
10.	punct (punctuation)

----------

The compilation of the myUDTree corpus is as follows:  

Table 1. Corpus information of the myUDTree (version 1.0)  

|Unit|myPOS (ver. 1.0)|Ext-1: my-zh|	Ext-2: my-ko|	Ext-3: ASEAN-MT (my)| myUDTree (ver. 1.0)|
|:------------- |--------:| -----:|-----:|-----:|-----:|
|Sentences	|11,000	|10,000	|10,052	|12,144	|43,196|
|Words	| 239,598 | 103,909 | 106,864 | 114,134 | 564,505|
|Average Words/Sentence	| 21.78| 10.17|	10.64| 9.40| 	13.07|


## မိတ်ဆက် (Intoduction in Myanmar Language)

myUDTree corpus ဟာ ဆိုရင် (Hnin Thu Zar Aye et al., 2018) တည်ဆောက်ခဲ့တဲ့ Universal Dependency tree data စာကြောင်းရေ ၁၁,၀၀၀ corpus ကို အခြေခံပြီး graph-based model ဆောက် parsing လုပ်ပြီး ဒေတာကို သုံးဆကျော် တိုး extend လုပ်ထားတဲ့ UDTree Corpus အသစ် ဖြစ်ပါတယ်။ ယခု release လုပ်တဲ့ Myanmar UDTree Corpus ရဲ့ version 1.0 မှာဆိုရင် စာကြောင်း အရေအတွက်စုစုပေါင်း ၄၃,၁၉၆ ပါဝင်ပါတယ်။  

Universal Dependency (UD) corpus ဆိုသည်မှာ Part-of-Speech (POS) အပြင် mophological feature များနှင့် syntatic dependency များဖြင့် သက်ဆိုင်ရာ ဘာသာစကားရဲ့ grammar rule အရ annotated လုပ်ထားတဲ့ corpus အမျိုးအစားဖြစ်ပါတယ်။ myUDTree ကို မတည်ဆောက်ခင်မှာ dependency information များဖြင့် raw data များကို parsing လုပ်နိုင်ရန်အတွက် မူလရှိပြီးသား စာကြောင်းရေ တစ်သောင်းကျော်သာ ရှိတဲ့ Myanmar UD corpus အသုံးပြု၍ dependnecy parsing model တစ်ခုဖြစ်တဲ့ [Joint POS Tagging and Graph-based Dependency Parsing (jPTDP)](https://github.com/datquocnguyen/jPTDP) မော်ဒယ် ကို တည်ဆောက်ခဲ့ပါတယ်။ 

jPTDP မော်ဒယ်ကို တည်ဆောက်ပြီးတဲ့နောက်မှာ လက်ရှိမှာ machine translation သုတေသနအတွက် ပြင်ဆင်နေတဲ့ parallel corpora (i.e. Myanmar-Chinese and Myanmar-Korean) မှ Myanmar raw data စာကြောင်းရေ ၂၀,၀၀၀ နှင့် ထိုင်းနိုင်ငံ [NECTEC Research Center](https://www.nectec.or.th/en/) မှ တည်ဆောက်ထားသော ASEAN MT Corpus မှ Myanmar raw data စာကြောင်းရေ ၁၂,၀၀၀ တို့အား jPTDP model ဖြင့် dependency tree data များ ရရှိရန် parsing လုပ်ခဲ့ပါတယ်။ Parsed လုပ်ထားသော ဒေတာများကို CoNLL-U Viewer tool ကို အသုံးပြုပြီး manual အားဖြင့် အချိန်ယူ စစ်ဆေးပြီးပြင်ဆင်ထားပါတယ်။ အဲ့ဒီနောက်မှာ စစ်ဆေးပြင်ဆင်ထားသော dependency tree data များနှင့် မူလရှိပြီးသား Myanmar UD Corpus ကို parse လုပ်ထားတဲ့ output စာကြောင်းတွေနဲ့ပေါင်းလိုက်ပြီး စာကြောင်းရေ အရေအတွက် ၄၃,၁၆၉ နှင့် dependency tree information များ ပါဝင်သော myUDTree Corpus (version 1.0) ကို ဖွဲ့စည်းထားပါတယ်။

Myanmar UDTree Corpus (version 1.0) မှာ 14 Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) နှင့် 14 dependency relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) တို့ကို apply လုပ်ထားပြီး dependency tree data format အနေဖြင့် CoNLL-U format ကို အသုံးပြုထားပါတယ်။  

Myanmar dependency structure မှာ အများဆုံး အသုံးပြုတဲ့ dependency relation တွေကတော့ အောက်ဖော်ပြပါ relation များဖြစ်ကြပါတယ်။  

1.	root (root) 
2.	acl (clausal modifier of noun) 
3.	amod (adjectival modifier) 
4.	advmod (adverbial modifier) 
5.	case (case marking) 
6.	mark (marker) 
7.	compound (compound) 
8.	obl (oblique nominal) 
9.	obj (object)
10.	punct (punctuation)

------------


ဒေတာပမာဏ မတူတဲ့ myPOS ver. 1.0 နှင့် ver. 3.0 နှစ်မျိုးစလုံးကို အသုံးပြုပြီး experiment လုပ်ခဲ့တဲ့ dependency parsing model နှစ်ခု (i.e., [jPTDP](https://github.com/datquocnguyen/jPTDP) and [UniParse](https://github.com/danielvarab/uniparse)) အကြား မတူညီတဲ့ accuracy ရလဒ်တွေကို အောက်ပါ Table 2 မှာ ဖော်ပြထားပါတယ်။ Accuracy အနေနဲ့က UniParse က jPTDP ထက် UAS ရလဒ်မှာရော LAS ရလဒ်မှာပါ အနည်းငယ် သာလွန်တာကို ထင်ထင်ရှားရှား မြင်ကြရပါလိမ့်မယ်။  

Table 2. Comparison of accuracy values between dependency parsing models  

|Model|UAS <br/>(myPOS ver.1)|LAS <br/>(myPOS ver.1)|UAS <br/>(myPOS ver.3)|LAS <br/> (myPOS ver.3)|
|:----|--------:| -----:|-----:|-----:|
|jPTDP| 85.07%| 81.38%| 86.16%| 82.77%|
|UniParse| 85.67%| 82.72%| 86.27%| 83.36%|


Note: jPTDP Model က raw text data ကို parsing လုပ်ပေးနိုင်သော်လည်း UniParse model ကတော့ raw text data များကို parsing မလုပ်ပေးနိုင်ပါ။ အဲဒါကြောင့် ဒီ myUDTree repository မှာ training လုပ်ခဲ့တဲ့ JPTDP မော်ဒယ်နှစ်ခု (တစ်ခုက myPOS ver.1, နောက်တစ်ခုက myPOS ver.3 corpus ရဲ့ စာကြောင်းတွေကို သုံးခဲ့) ကိုပဲ ဆက်လက်လေ့လာချင်သူတွေအတွက် [Microsoft OneDrive link](https://1drv.ms/f/s!Ap_PSroRKvH0akzceRq0cJpNK4w) ကနေတဆင့် ရှဲလုပ်ပေးထားပါတယ်။  

## Introduction to CoNLL-U Viewer tool

CoNLL-U Viewer (https://urd2.let.rug.nl/~kleiweg/conllu/) ကို အသုံးပြုပြီး dependency tree structure တွေကို ကြည့်တာ ပုံတွေကို save လုပ်တာ လုပ်နိုင်ပါတယ်။ CoNLL-U Viewer website မှာ CoNLL-U Formart ဖြင့် သိမ်းဆည်းထားတဲ့ text file ကို upload လုပ်ပေးလိုက်ယုံပါပဲ။  


ဥပမာ အနေနဲ့ myUDTree (version 1.0) ထဲမှာ ပါဝင်တဲ့ အောက်ပါ စာကြောင်းငါးကြောင်းကို CoNLL-U Viewer ကို upload လုပ်လိုက်ရင် စာကြောင်း တစ်ကြောင်းချင်းစီအတွက် dependency relationship ပုံတွေကို output အနေနဲ့ ရလာပါလိမ့်မယ်။  

### Example sentence no.1

Input:  
```
1	ကျသင့်	_	VERB	_	_	2	acl	_	_
2	ငွေ	_	NOUN	_	_	4	obl	_	_
3	က	_	ADP	_	_	2	case	_	_
4	ဘယ်လောက်	_	ADJ	_	_	0	root	_	_
5	လဲ	_	PART	_	_	4	mark	_	_
6	။	_	PUNCT	_	_	4	punct	_	_
```

Output:  
<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence1.png" alt="dependency tree for example sentence no. 1" width="800"/>  
</p>  
<div align="center">
  Fig.1 Dependency tree for the example sentence no. 1: "ကျသင့်ငွေ က ဘယ်လောက်လဲ။"  
</div> 

<br />

### Example sentence no.2

Input:  
```
1	ချစ်မေတ္တာ	_	NOUN	_	_	2	compound	_	_
2	သင်္ကေတ	_	NOUN	_	_	6	obl	_	_
3	အနေနဲ့	_	PART	_	_	2	case	_	_
4	နှင်းဆီပန်း	_	NOUN	_	_	6	obl	_	_
5	ကို	_	ADP	_	_	4	case	_	_
6	ပို့ပေး	_	VERB	_	_	0	root	_	_
7	ခဲ့	_	PART	_	_	6	mark	_	_
8	တယ်	_	ADP	_	_	6	case	_	_
9	။	_	PUNCT	_	_	6	punct	_	_
```

Output:  
<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence2.png" alt="dependency tree for example sentence no. 2" width="800"/>  
</p>  
<div align="center">
  Fig.2 Dependency tree for the example sentence no. 2: "ချစ်မေတ္တာ သင်္ကေတ အနေနဲ့ နှင်းဆီပန်းကို ပို့ပေးခဲ့တယ်။"  
</div> 

<br />

### Example sentence no.3

Input:  
```
1	ထမင်း	_	NOUN	_	_	4	obl	_	_
2	ကို	_	ADP	_	_	1	case	_	_
3	နည်းနည်း	_	ADV	_	_	4	advmod	_	_
4	ရ	_	VERB	_	_	0	root	_	_
5	နိုင်	_	PART	_	_	4	mark	_	_
6	ပါ	_	PART	_	_	4	case	_	_
7	သလား	_	PART	_	_	4	mark	_	_
8	။	_	PUNCT	_	_	4	punct	_	_
```

Output:  
<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence3b.png" alt="dependency tree for example sentence no. 3" width="800"/>  
</p>  
<div align="center">
  Fig.3 Dependency tree for the example sentence no. 3: "ကိုရီးယား-မြန်မာ အဘိဓါန် တစ်အုပ်ဝယ်မလို့ပါ။"  
</div> 

<br />

### Example sentence no.4

Input:  
```
1	Country	_	NOUN	_	_	2	compound	_	_
2	code	_	NOUN	_	_	6	obl	_	_
3	ကို	_	ADP	_	_	2	case	_	_
4	လည်း	_	PART	_	_	2	case	_	_
5	တပါတည်း	_	ADV	_	_	6	advmod	_	_
6	တွဲထည့်	_	VERB	_	_	0	root	_	_
7	ပေး	_	PART	_	_	6	mark	_	_
8	ထား	_	PART	_	_	6	case	_	_
9	ပါ	_	PART	_	_	6	mark	_	_
10	သည်	_	ADP	_	_	6	case	_	_
11	။	_	PUNCT	_	_	6	punct	_	_
```

Output:  
<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence4.png" alt="dependency tree for example sentence no. 4" width="800"/>  
</p>  
<div align="center">
  Fig.4 Dependency tree for the example sentence no. 4: "Country code ကိုလည်း တပါတည်းတွဲထည့် ပေး ထားပါသည်။"  
</div> 

<br />

### Example sentence no.5

Input:  
```
1	မက်ဆင်ဂျာ	_	PROPN	_	_	7	compound	_	_
2	အာကာသယာဉ်	_	NOUN	_	_	1	obl	_	_
3	သည်	_	ADP	_	_	2	case	_	_
4	ဂြိုဟ်	_	NOUN	_	_	5	compound	_	_
5	အနီး	_	NOUN	_	_	7	obl	_	_
6	မှ	_	ADP	_	_	5	case	_	_
7	ဖြတ်	_	VERB	_	_	11	acl	_	_
8	၍	_	SCONJ	_	_	7	mark	_	_
9	တစ်	_	NUM	_	_	11	nummod	_	_
10	ကြိမ်	_	PART	_	_	9	case	_	_
11	ပျံသန်း	_	VERB	_	_	14	acl	_	_
12	ခဲ့	_	PART	_	_	11	mark	_	_
13	ပြီး	_	PART	_	_	11	case	_	_
14	ဖြစ်	_	VERB	_	_	0	root	_	_
15	သည်	_	ADP	_	_	14	case	_	_
16	။	_	PUNCT	_	_	14	punct	_	_
```

Output:  
<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence5.png" alt="dependency tree for example sentence no. 5" width="800"/>  
</p>  
<div align="center">
  Fig.5 Dependency tree for the example sentence no. 5: "မက်ဆင်ဂျာ အာကာသယာဉ်သည် ဂြိုဟ်အနီးမှ ဖြတ်၍ တစ်ကြိမ်ပျံသန်းခဲ့ပြီး ဖြစ်သည်။"  
</div> 

<br />

### Dependency relationship of each word

CoNLL-U Viewer tool ကို သုံးပြီးတော့ မြန်မာစာလုံး တစ်လုံးချင်းစီကို mouse pointer နဲ့ ထောက်ပေးလိုက်ရင်၊ အဲဒီ စာလုံး တစ်လုံးချင်းစီက ချိတ်ဆက်နေတဲ့ dependency relationship လမ်းကြောင်းတွေကို highlight လုပ်ပေးလို့ အသေးစိတ်လေ့လာချင်သူတွေအတွက်လည်း အသုံးဝင်ပါလိမ့်မယ်။  

အောက်ပါ ပုံက အထက်မှာပေးခဲ့တဲ့ ဥပမာစာကြောင်းနံပါတ် ၃ ရဲ့ output graph ကိုပဲ "အဘိဓါန်" ဆိုတဲ့ စာလုံးကို mouse pointer ထောက်ကြည့်ရင် မြင်ရမယ့် အပြာရောင်မြှားအထူနဲ့ ပြပေးမယ့် dependency relationship တွေဖြစ်ပါတယ်။  


<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/highlight-eg-sent3-point-word-dict.png" alt="Highlighting demo with sentence no.3" width="800"/>  
</p>  
<div align="center">
  Fig.6 Highlighting demo with example sentence no. 3 when you point the mouse pointer on the word "အဘိဓါန်"  
</div> 

<br />

## Parsing Raw Myanmar Sentences with jPTDP Models

ရှဲလုပ်ထားတဲ့ jPTDP မော်ဒယ်တွေကို သုံးပြီးတော့ raw မြန်မာစာ စာကြောင်း တွေကို ဘယ်လို UDTree parsing လုပ်ရသလဲ ဆိုတာကို အလွယ် ရှင်းပြရရင် ...   


## Citation

If you want to use myUDTree JPTDP models or myUDTree corpus in your research and we'd appreciate if you use the following reference:  

Zar Zar Hlaing, Ye Kyaw Thu, Thepchai Supnithi and Ponrudee Netisopakul, "Graph-based Dependency Parser Building for Myanmar Language", In Proceedings of the 17th International Joint Symposium on Artificial Intelligence and Natural Language Processing (iSAI-NLP 2022), Nov 5 to 7, 2022, Chiang Mai, Thailand, pp. xx-xx. [to appear], [[Slide]](https://github.com/ye-kyaw-thu/papers/blob/master/iSAI-NLP2022/9510_Graph-basedDependencyParserBuildingforMyanmarLanguage.pdf)  

## Lincense

Creative Commons Attribution-NonCommercial-Share Alike 4.0 International (CC BY-NC-SA 4.0) License  
[Details Info of License](https://creativecommons.org/licenses/by-nc-sa/4.0/)  

Contact email: yktnlp[at]gmail.com  

## Reference

1. The concept of Universal Dependencies (UD):  
https://universaldependencies.org/  

2. B. Prachya and S. Thepchai, "Technical Report for The Network-based ASEAN Language Translation Public Service Project", Online Materials of Network-based ASEAN Languages Translation Public Service for Members, 2013.

3. Hnin Thu Zar Aye, Win Pa Pa, and Ye Kyaw Thu, "Unsupervised Dependency Corpus Annotation for Myanmar Language", In Proceedings of The 21st Conference of the Oriental Chapter of the International Coordinating Committee on Speech Databases and Speech I/O Systems and Assessment (Oriental COCOSDA 2018), May 2018, Miyazaki, Japan  

4. CoNLL-Viewer Tool:  
https://urd2.let.rug.nl/~kleiweg/conllu/?fbclid=IwAR2Flucow_szmuB63-J2vuqSGiXXtCw8I_OUyHvxd4hZfs0oK0140x5oQtY  

5. Neural network models for joint POS tagging and dependency parsing (CoNLL 2017-2018):  
https://github.com/datquocnguyen/jPTDP?fbclid=IwAR2xUeHdT4tGMD0vQ7nor7aXjfuDtaFaoNjwgpuz8ye2xd5uG6laAUOCWho

6. Khin War War Htike, Ye Kyaw Thu, Zuping Zhang, Win Pa Pa, Yoshinori Sagisaka and Naoto Iwahashi, "Comparison of Six POS Tagging Methods on 10K Sentences Myanmar Language (Burmese) POS Tagged Corpus", at 18th International Conference on Computational Linguistics and Intelligent Text Processing (CICLing 2017), April 17~23, 2017, Budapest, Hungary.[[Draft paper]](https://github.com/ye-kyaw-thu/myPOS/blob/master/CICLING2017/myPOS-CICLing2017-paper.pdf), [[Poster]](https://github.com/ye-kyaw-thu/myPOS/blob/master/CICLING2017/10K-POS-tagging-CICLing2017.pdf)  

7. Zar Zar Hlaing, Ye Kyaw Thu, Myat Myo Nwe Wai, Thepchai Supnithi, Ponrudee Netisopakul, "Myanmar POS resource extension effects on automatic tagging methods", In Proceedings of the 15th International Joint Symposium on Artificial Intelligence and Natural Language Processing (iSAI-NLP 2020), Nov 18 to Nov 20, 2020, Bangkok, Thailand, pp. 189-194. [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9376835)    

8. A framework for graph-based dependency parsing:  
https://github.com/danielvarab/uniparse  


## To Do

- Recheck myUDTree ver.1  
- Active learning and Manual UDTree tagging for myUDTree corpus extension  
- DTree parsing experiments for Myanmar language





