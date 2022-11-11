# myUDTree

Universal Dependency Tree for Myanmar Language  
We plan to announce/release soon ...   

y  
10 Nov 2022  

## Introduction
	
The myUDTree corpus is a Universal Dependency (UD) Corpus that extends the Myanmar UD Corpus (Hnin Thu Zar Aye et al., 2018) including 11,000 sentences of Dependency Tree Data. The extended myUDTree Corpus contains 43,196 sentences in total.  

Universal Dependencies (UD) Corpus is a type of Corpus that is annotated according to the Grammar Rule of the respective languages with Part-of-Speech, Morphological Features, and Syntactic Dependencies. Before building myUDTree, we built a Dependency Parsing Model, a Joint POS Tagging and Graph-based Dependency Parsing (jPTDP) model, using the existing Myanmar UD corpus in order to parse Raw Data with Dependency Information. After building the jPTDP model, we selected 20,000 Myanmar sentences from our developing parallel corpora (i.e., Myanmar-Chinese and Myanmar-Korean), and 12,000 Myanmar sentences from the ASEN MT Corpus built by NECTEC Research Center in Thailand, and these data are parsed by using our built jPTDP model to obtain dependency-tree data.  

The parsed data were manually checked and corrected using the CoNLL-U Viewer tool. After that, the revised data and the parsed output of the original Myanmar UD corpus were integrated to obtain the myUDTree corpus which contains 43,169 sentences with dependency information. Fourteen (14) Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) and 14 dependency relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) are applied in the original version of Myanmar UD Corpus, and CoNLL-U format is used as a dependency-tree data format. The same number of Universal Part-of-Speech tags and Dependency Relations were also applied in our extended myUDTree corpus. The following dependency relations are the most primarily utilized in Myanmar Dependency Structure.
  
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

|Unit|myPOS (ver. 1.0)|Ext-1: my-zh|	Ext-2: my-ko|	Ext-3: ASEAN-MT (my)| myUDTree|
|:------------- |--------:| -----:|-----:|-----:|-----:|
|Sentences	|11,000	|10,000	|10,052	|12,144	|43,196|
|Words	| 239,598 | 103,909 | 106,864 | 114,134 | 564,505|
|Average Words/Sentence	| 21.78| 10.17|	10.64| 9.40| 	13.07|


## မိတ်ဆက် (Intoduction in Myanmar Language)

myUDTree corpus ဟာ ဆိုရင် (Hnin Thu Zar Aye et al., 2018) တည်ဆောက်ခဲ့တဲ့ Universal Dependency Tree Data စာကြောင်းရေ ၁၁,၀၀၀ Corpus ကို အခြေခံပြီး graph-based model ဆောက် parsing လုပ်ပြီး ဒေတာကို သုံးဆကျော် တိုး extend လုပ်ထားတဲ့ UDTree Corpus အသစ် ဖြစ်ပါတယ်။ Myanmar UDTree Corpus ရဲ့ version 1.0 မှာဆိုရင် စာကြောင်း အရေအတွက်စုစုပေါင်း ၄၃,၁၉၆ ပါဝင်ပါတယ်။  

Universal Dependencies (UD) Corpus ဆိုသည်မှာ Part-of-Speech အပြင် Mophological Feature များနှင့် Syntatic Dependencie များဖြင့် သက်ဆိုင်ရာ ဘာသာစကားရဲ့ Grammar Rule အရ Annotated လုပ်ထားတဲ့ Corpus အမျိုးအစားဖြစ်ပါတယ်။ myUDTree ကို မတည်ဆောက်ခင်မှာ Dependency Information များဖြင့် Raw Data များကို Parsed လုပ်နိုင်ရန်အတွက် မူလရှိပြီးသား စာကြောင်းရေ တစ်သောင်းကျော်သာ ရှိတဲ့ Myanmar UD corpus အသုံးပြု၍ Dependnecy Parsing Model တစ်ခုဖြစ်တဲ့ Joint POS Tagging and Graph-based Dependency Parsing (jPTDP) မော်ဒယ် ကို တည်ဆောက်ခဲ့ပါတယ်။ 

jPTDP မော်ဒယ်ကို တည်ဆောက်ပြီးတဲ့နောက်မှာ လက်ရှိမှာ ပြင်ဆင်နေသာ Parallel Corpora (i.e. Myanmar-Chinese and Myanmar-Korean) မှ Myanmar Raw Data စာကြောင်းရေ ၂၀,၀၀၀ နှင့် ထိုင်းနိုင်ငံ NECTEC Research Centerမှ တည်ဆောက်ထားသော ASEN MT Corpus မှ Myanmar Raw Data စာကြောင်းရေ ၁၂,၀၀၀ တို့ကို jPTDP မော်ဒယ်ကို အသုံးပြု၍ Dependency Tree Data များရရှိရန်အတွက် Raw Data များကို Parsed လုပ်ခဲ့ပါတယ်။ Parsed လုပ်ထားသော ဒေတာများကို CoNLL-U Viewer tool ကို အသုံးပြုပြီး manual အားဖြင့် အချိန်ယူ စစ်ဆေးပြီးပြင်ဆင်ထားပါတယ်။ အဲ့ဒီနောက်မှာ စစ်ဆေးပြင်ဆင်ထားသော Dependency Tree Data များနှင့် မူလရှိပြီးသား Myanmar UD Corpus တို့ကို ပေါင်းစပ်ထားပြီး စာကြောင်းရေ အရေအတွက် ၄၃,၁၆၉ နှင့် Dependency Tree Information များ ပါဝင်သော myUDTree Corpus (version 1.0) ကို ဖွဲ့စည်းထားပါတယ်။

Myanmar UDTree Corpus (version 1.0) မှာ 14 Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) နှင့် 14 Dependency Relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) တို့ကို apply လုပ်ထားပြီး Dependency Tree Data Format အနေဖြင့် CoNLL-U Format ကို အသုံးပြုထားပါတယ်။  

Myanmar Dependency Structure မှာ အများဆုံး အသုံးပြုတဲ့ Dependency Relations တွေကတော့ အောက်ဖော်ပြပါ Dependency Relationsများ ဖြစ်ကြပါတယ်။

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


myUDTree Corpus နှင့် Original Myanmar UD Corpus နှစ်ခုကို အသုံးပြုပြီး တည်ဆောက်ခဲ့တဲ့ Dependency Parsing Models (i.e., jPTDT and UniParse) တွေရဲ့  Accuracies ကို အောက်ပါ Table တွင် ပြထားပါတယ်။

Table 2. Comparison of accuracy values between dependency parsing models  

|Model|UAS <br/>(myPOS ver.1)|LAS <br/>(myPOS ver.1)|UAS <br/>(myPOS ver.3)|LAS <br/> (myPOS ver.3)|
|:----|--------:| -----:|-----:|-----:|
|jPTDP| 85.07%| 81.38%| 86.16%| 82.77%|
|UniParse| 85.67%| 82.72%| 86.27%| 83.36%|


Note: jPTDT Model က Raw Text Data ကို Parsed လုပ်ပေးနိုင်သော်လည်း UniParse Model ဟာဆိုရင်ဖြင့် Raw Text Data များကို Parsed မလုပ်ပေးနိုင်ပါ။ 

## Introduction to CoNLL-U Viewer tool

CoNLL-U Viewer (https://urd2.let.rug.nl/~kleiweg/conllu/) ကို အသုံးပြုပြီး dependency tree structure တွေကို ကြည့်တာ ပုံတွေကို save လုပ်တာ လုပ်နိုင်ပါတယ်။ CoNLL-U Viewer website မှာ CoNLL-U Formart ဖြင့် သိမ်းဆည်းထားတဲ့ text file ကို upload လုပ်ပေးလိုက်ယုံပါပဲ။  


ဥပမာ အနေနဲ့ myUDTree (version 1.0) ထဲမှာ ပါဝင်တဲ့ အောက်ပါ စာကြောင်းငါးကြောင်းကို CoNLL-U Viewer ကို upload လုပ်လိုက်ရင် စာကြောင်း တစ်ကြောင်းချင်းစီအတွက် dependency relationship ပုံတွေကို output အနေနဲ့ ရလာပါလိမ့်မယ်။  

```
1	ကျသင့်	_	VERB	_	_	2	acl	_	_
2	ငွေ	_	NOUN	_	_	4	obl	_	_
3	က	_	ADP	_	_	2	case	_	_
4	ဘယ်လောက်	_	ADJ	_	_	0	root	_	_
5	လဲ	_	PART	_	_	4	mark	_	_
6	။	_	PUNCT	_	_	4	punct	_	_
```

<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence1.png" alt="dependency tree for example sentence no. 1" width="800"/>  
</p>  
<div align="center">
  Fig.1 Dependency tree for the example sentence no. 1: "ကျသင့် ငွေ က ဘယ်လောက် လဲ ။"  
</div> 

<br />

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

<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence2.png" alt="dependency tree for example sentence no. 1" width="800"/>  
</p>  
<div align="center">
  Fig.2 Dependency tree for the example sentence no. 2: "ချစ်မေတ္တာ သင်္ကေတ အနေနဲ့ နှင်းဆီပန်း ကို ပို့ပေး ခဲ့ တယ် ။"  
</div> 

<br />

```
1	ကိုရီးယား	_	PROPN	_	_	4	obl	_	_
2	−	_	PUNCT	_	_	1	punct	_	_
3	မြန်မာ	_	PROPN	_	_	4	compound	_	_
4	အဘိဓါန်	_	NOUN	_	_	7	compound	_	_
5	တစ်	_	NUM	_	_	4	nummod	_	_
6	အုပ်	_	PART	_	_	5	case	_	_
7	ဝယ်	_	VERB	_	_	9	acl	_	_
8	မ	_	PART	_	_	9	case	_	_
9	လို့	_	VERB	_	_	0	root	_	_
10	ပါ	_	PART	_	_	9	mark	_	_
11	။	_	PUNCT	_	_	9	punct	_	_
```

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

## To Do

- Recheck myUDTree ver.1  
- Active learning and Manual UDTree tagging for myUDTree corpus extension  

## Citation

Zar Zar Hlaing, Ye Kyaw Thu, Thepchai Supnithi and Ponrudee Netisopakul, "Graph-based Dependency Parser Building for Myanmar Language", In Proceedings of the 17th International Joint Symposium on Artificial Intelligence and Natural Language Processing (iSAI-NLP 2022), Nov 5 to 7, 2022, Chiang Mai, Thailand, pp. xx-xx. [to appear], [[Slide]](https://github.com/ye-kyaw-thu/papers/blob/master/iSAI-NLP2022/9510_Graph-basedDependencyParserBuildingforMyanmarLanguage.pdf)  

## Reference

1. The concept of Universal Dependencies (UD):  
https://universaldependencies.org/  

2. Hnin Thu Zar Aye, Win Pa Pa, and Ye Kyaw Thu, "Unsupervised Dependency Corpus Annotation for Myanmar Language", In Proceedings of The 21st Conference of the Oriental Chapter of the International Coordinating Committee on Speech Databases and Speech I/O Systems and Assessment (Oriental COCOSDA 2018), May 2018, Miyazaki, Japan  

3. CoNLL-Viewer Tool:  
https://urd2.let.rug.nl/~kleiweg/conllu/?fbclid=IwAR2Flucow_szmuB63-J2vuqSGiXXtCw8I_OUyHvxd4hZfs0oK0140x5oQtY  

4. Neural network models for joint POS tagging and dependency parsing (CoNLL 2017-2018):  
https://github.com/datquocnguyen/jPTDP?fbclid=IwAR2xUeHdT4tGMD0vQ7nor7aXjfuDtaFaoNjwgpuz8ye2xd5uG6laAUOCWho









