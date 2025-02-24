# myUDTree

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

Universal Dependency (UD) corpus ဆိုသည်မှာ Part-of-Speech (POS) အပြင် mophological feature များ၊ syntatic dependency များဖြင့် သက်ဆိုင်ရာ ဘာသာစကားရဲ့ grammar rule အရ annotated လုပ်ထားတဲ့ corpus အမျိုးအစားဖြစ်ပါတယ်။ myUDTree ကို မတည်ဆောက်ခင်မှာ dependency information များဖြင့် raw data များကို parsing လုပ်နိုင်ရန်အတွက် မူလရှိပြီးသား စာကြောင်းရေ တစ်သောင်းကျော်သာ ရှိတဲ့ Myanmar UD corpus အသုံးပြု၍ dependnecy parsing model တစ်ခုဖြစ်တဲ့ [Joint POS Tagging and Graph-based Dependency Parsing (jPTDP)](https://github.com/datquocnguyen/jPTDP) မော်ဒယ် ကို တည်ဆောက်ခဲ့ပါတယ်။ 

jPTDP မော်ဒယ်ကို တည်ဆောက်ပြီးတဲ့နောက် လက်ရှိမှာ machine translation သုတေသနအတွက် ပြင်ဆင်နေတဲ့ parallel corpora (i.e. Myanmar-Chinese and Myanmar-Korean) မှ Myanmar raw data စာကြောင်းရေ ၂၀,၀၀၀ နှင့် ထိုင်းနိုင်ငံ [NECTEC Research Center](https://www.nectec.or.th/en/) မှ တည်ဆောက်ထားသော ASEAN MT Corpus မှ Myanmar raw data စာကြောင်းရေ ၁၂,၀၀၀ တို့အား jPTDP model ဖြင့် dependency tree data များ ရရှိရန် parsing လုပ်ခဲ့ပါတယ်။ Parsed လုပ်ထားသော ဒေတာများကို CoNLL-U Viewer tool ကို အသုံးပြုပြီး manual အားဖြင့် အချိန်ယူ စစ်ဆေးပြီးပြင်ဆင်ထားပါတယ်။ အဲ့ဒီနောက်မှာ စစ်ဆေးပြင်ဆင်ထားသော dependency tree data များနှင့် မူလရှိပြီးသား Myanmar UD Corpus ကို parse လုပ်ထားတဲ့ output စာကြောင်းတွေနဲ့ပေါင်းလိုက်ပြီး စာကြောင်းရေ အရေအတွက် ၄၃,၁၆၉ နှင့် dependency tree information များ ပါဝင်သော myUDTree Corpus (version 1.0) ကို ဖွဲ့စည်းထားပါတယ်။

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
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence1b.png" alt="dependency tree for example sentence no. 1" width="800"/>  
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
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/myUDTree-eg-sentence2b.png" alt="dependency tree for example sentence no. 2" width="800"/>  
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
  Fig.3 Dependency tree for the example sentence no. 3: "ထမင်း ကို နည်းနည်း ရ နိုင် ပါ သလား ။"  
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

အောက်ပါ ပုံက အထက်မှာပေးခဲ့တဲ့ ဥပမာစာကြောင်းနံပါတ် ၂ ရဲ့ output graph ကိုပဲ "နှင်းဆီပန်း" ဆိုတဲ့ စာလုံးကို mouse pointer ထောက်ကြည့်ရင် မြင်ရမယ့် အပြာရောင်မြှားအထူနဲ့ ပြပေးမယ့် dependency relationship တွေဖြစ်ပါတယ်။  


<p align="center">
<img src="https://github.com/ye-kyaw-thu/myUDTree/blob/main/ver-1.0/pic/highlight-eg-sent2b-point-word-dict.png" alt="Highlighting demo with sentence no.2" width="800"/>  
</p>  
<div align="center">
  Fig.6 Highlighting demo with example sentence no. 2 when you point the mouse pointer on the word "နှင်းဆီပန်း"  
</div> 

<br />

## Parsing Raw Myanmar Sentences with jPTDP Models

ရှဲလုပ်ထားတဲ့ jPTDP မော်ဒယ်တွေကို သုံးပြီးတော့ raw မြန်မာစာ စာကြောင်း တွေကို ဘယ်လို UDTree parsing လုပ်ရသလဲ ဆိုတာကို အလွယ် ရှင်းပြရရင် ...   

### Clone jPTDP

ပထမဆုံး jPTDP repository ကို ကိုယ့်စက်ထဲကို clone (i.e. download) လုပ်ရအောင် ...  

```
(jPTDP-cpu) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test$ git clone https://github.com/bryant1410/jPTDP
Cloning into 'jPTDP'...
remote: Enumerating objects: 124, done.
remote: Total 124 (delta 0), reused 0 (delta 0), pack-reused 124
Receiving objects: 100% (124/124), 59.34 KiB | 161.00 KiB/s, done.
Resolving deltas: 100% (70/70), done.
(jPTDP-cpu) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test$
```

clone လုပ်ထားတဲ့ folder ထဲကို ဝင်ကြည့်ပြီး အသစ်ရောက်လာတဲ့ python code စတာတွေကို confirm လုပ်ကြည့်ရအောင် ...  

```
(jPTDP-cpu) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ ls
decoder.py  jPTDP.py  learner.py  License.txt  mnnl.py  README.md  sample  utils  utils.py
(jPTDP-cpu) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$
```

### Installation of DyNet

မော်ဒယ် အသစ်ကို Training လုပ်ဖို့ ရှိပြီးသား မော်ဒယ်နဲ့ UDTree parsing လုပ်ဖို့အတွက်က DyNet framework လိုအပ်တယ်။  
အဲဒါကြောင့် DyNet Python library ကို pip နဲ့ install လုပ်ရအောင်။  

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ pip install dynet
DEPRECATION: Python 2.7 will reach the end of its life on January 1st, 2020. Please upgrade your Python as Python 2.7 won't be maintained after that date. A future version of pip will drop support for Python 2.7. More details about Python 2 support in pip, can be found at https://pip.pypa.io/en/latest/development/release-process/#python-2-support
Collecting dynet
  Downloading https://files.pythonhosted.org/packages/19/69/3fe9fd6d2a270ceb5ab2646f596378dcb7be7e5fd7adb8d3b932b98f0656/dyNET-2.1.2-cp27-cp27mu-manylinux1_x86_64.whl (4.2MB)
     |████████████████████████████████| 4.2MB 1.7MB/s 
Collecting cython
  Downloading https://files.pythonhosted.org/packages/72/a4/9e79a693b332eb013e684853abaa54223deb1df0115547f43f81a613d2f9/Cython-0.29.32-cp27-cp27mu-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.9MB)
     |████████████████████████████████| 1.9MB 12.0MB/s 
Requirement already satisfied: numpy in /home/ye/.local/lib/python2.7/site-packages (from dynet) (1.16.6)
Installing collected packages: cython, dynet
Successfully installed cython-0.29.32 dynet-2.1.2
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$
```

### Check/Install Future

Future ဆိုတဲ့ Python package လည်း လိုအပ်လို့ installation လုပ်ရလိမ့်မယ်။  

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ pip install future
DEPRECATION: Python 2.7 will reach the end of its life on January 1st, 2020. Please upgrade your Python as Python 2.7 won't be maintained after that date. A future version of pip will drop support for Python 2.7. More details about Python 2 support in pip, can be found at https://pip.pypa.io/en/latest/development/release-process/#python-2-support
Requirement already satisfied: future in /home/ye/tool/anaconda3/envs/py2.7/lib/python2.7/site-packages (0.18.2)
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$
```

### Prepare Test File

UDTree parsing ကို ဥပမာအဖြစ် ပြဖို့အတွက် raw test file တစ်ဖိုင်ကို prepare လုပ်ခဲ့တယ်။ တကယ်ကတော့ corpus ထဲကနေပဲ စာကြောင်း သုံးကြောင်းကို ဆွဲထုတ်လာတာပါ။    

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ cat raw.txt
စာကြည့်တိုက် ကို သွား ပြီး တော့ စာအုပ် ဖတ် မလို့ ။
သူ ဟာ ပိုက်ဆံရှာ ဖို့ ကို သာလျှင် စဉ်းစား နေ တယ် ။
တူလေး ကို နားဝင်အောင် ဆုံးမ ပြောဆို သည် ။
```

### Converting Raw Data into CONLLU Format

jPTDP model ကို prediction or UDTree parsing လုပ်ခိုင်းဖို့က CONLLU format ကို ပြောင်းပေးဖို့ လိုအပ်တယ်။ အဲဒီအတွက်က utils/ ဆိုတဲ့ folder အောက်က converter.py ကို သုံးပြီး format ပြောင်းခိုင်းလို့ ရတယ်။  

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ python ./utils/converter.py ./raw.txt 
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ ls raw.txt.conllu 
raw.txt.conllu
```

### Check the Converted Output File

CONLLU format အဖြစ် ပြောင်းပြီးသား output ဖိုင်က အောက်ပါအတိုင်းပါ။ ကျွန်တော်တို့ကတော့ column ဆယ်ခု ရှိတယ်ဆိုပြီး မှတ်ထားတယ်။    

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ cat raw.txt.conllu 
1	စာကြည့်တိုက်	_	_	_	_	_	_	_	_
2	ကို	_	_	_	_	_	_	_	_
3	သွား	_	_	_	_	_	_	_	_
4	ပြီး	_	_	_	_	_	_	_	_
5	တော့	_	_	_	_	_	_	_	_
6	စာအုပ်	_	_	_	_	_	_	_	_
7	ဖတ်	_	_	_	_	_	_	_	_
8	မလို့	_	_	_	_	_	_	_	_
9	။	_	_	_	_	_	_	_	_

1	သူ	_	_	_	_	_	_	_	_
2	ဟာ	_	_	_	_	_	_	_	_
3	ပိုက်ဆံရှာ	_	_	_	_	_	_	_	_
4	ဖို့	_	_	_	_	_	_	_	_
5	ကို	_	_	_	_	_	_	_	_
6	သာလျှင်	_	_	_	_	_	_	_	_
7	စဉ်းစား	_	_	_	_	_	_	_	_
8	နေ	_	_	_	_	_	_	_	_
9	တယ်	_	_	_	_	_	_	_	_
10	။	_	_	_	_	_	_	_	_

1	တူလေး	_	_	_	_	_	_	_	_
2	ကို	_	_	_	_	_	_	_	_
3	နားဝင်အောင်	_	_	_	_	_	_	_	_
4	ဆုံးမ	_	_	_	_	_	_	_	_
5	ပြောဆို	_	_	_	_	_	_	_	_
6	သည်	_	_	_	_	_	_	_	_
7	။	_	_	_	_	_	_	_	_

(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ 
```

### Parsing on CPU

DyNet က CPU ပေါ်မှာလည်း အလုပ်လုပ်ပေးတာကြောင့် ရှဲလုပ်ပေးထားတဲ့ myUDTree version 1.0 မော်ဒယ် (နာမည်ကတော့ mypos-ver-3-dep-model) ကို သုံးပြီး parsing လုပ်ခိုင်းကြည့်ရအောင်။  

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ time python jPTDP.py --predict --model ../model/mypos-ver-3-dep-model --params ../model/mypos-ver-3-dep-model.params --test ./raw.txt.conllu --outdir ./ --output raw.txt.conllu.pred
[dynet] random seed: 1895699260
[dynet] allocating memory: 512MB
[dynet] memory allocation done.
Loading pre-trained model
Predicting POS tags and parsing dependencies
The dy.parameter(...) call is now DEPRECATED.
        There is no longer need to explicitly add parameters to the computation graph.
        Any used parameter will be added automatically.

real	0m3.656s
user	0m3.472s
sys	0m0.444s
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ 
```

### Check the Parsed Output File

parsing လုပ်ပြီး ထွက်လာတဲ့ ဖိုင်က အောက်ပါအတိုင်းပါ။ POS tagging ရော၊ UDTree relationship ကိုရော tagging လုပ်ပေးထားတာကို မြင်တွေ့ရပါလိမ့်မယ်။    

```
(py2.7) ye@ykt-pro:/media/ye/project1/paper/isai-nlp2022/conf/zzh/parsing-test/jPTDP$ cat ./raw.txt.conllu.pred 
1	စာကြည့်တိုက်	_	NOUN	_	_	3	obl	_	_
2	ကို	_	ADP	_	_	1	case	_	_
3	သွား	_	VERB	_	_	7	acl	_	_
4	ပြီး	_	SCONJ	_	_	3	mark	_	_
5	တော့	_	PART	_	_	3	case	_	_
6	စာအုပ်	_	NOUN	_	_	7	obl	_	_
7	ဖတ်	_	VERB	_	_	0	root	_	_
8	မလို့	_	PART	_	_	7	mark	_	_
9	။	_	PUNCT	_	_	7	punct	_	_

1	သူ	_	PRON	_	_	3	obl	_	_
2	ဟာ	_	ADP	_	_	1	case	_	_
3	ပိုက်ဆံရှာ	_	VERB	_	_	7	acl	_	_
4	ဖို့	_	PART	_	_	3	mark	_	_
5	ကို	_	ADP	_	_	3	case	_	_
6	သာလျှင်	_	PART	_	_	3	case	_	_
7	စဉ်းစား	_	VERB	_	_	0	root	_	_
8	နေ	_	PART	_	_	7	mark	_	_
9	တယ်	_	ADP	_	_	7	case	_	_
10	။	_	PUNCT	_	_	7	punct	_	_

1	တူလေး	_	NOUN	_	_	5	obl	_	_
2	ကို	_	ADP	_	_	1	case	_	_
3	နားဝင်အောင်	_	NOUN	_	_	5	obl	_	_
4	ဆုံးမ	_	VERB	_	_	5	acl	_	_
5	ပြောဆို	_	VERB	_	_	0	root	_	_
6	သည်	_	ADP	_	_	5	case	_	_
7	။	_	PUNCT	_	_	5	punct	_	_
 
```

## Folder Information

လက်ရှိ myUDTree repository အောက်မှာ ရှိတဲ့ folder tree structure က အောက်ပါအတိုင်း ရှိပါလိမ့်မယ်။  

```
$ tree -L 1
.
├── iSAI-NLP-2022-experiment
├── myPOS-V3-Parsed-DP-Data
├── myUDTree-ver1.0
└── pic

4 directories, 0 files
```

**iSAI-NLP-2022-experiment** ဖိုလ်ဒါက iSAI-NLP 2022 စာတမ်းအတွက် ပြင်ဆင်ခဲ့တဲ့ experiment folder ပါ။ အဲဒီထဲမှာ myPOS ver. 1.0 နဲ့ ပြီးတော့ ဒေတာပိုများတဲ့ myPOS ver. 3.0 နဲ့ training ခဲ့တုန်းက model parameter နဲ့ running log ဖိုင်တွေ ရှိပါလိမ့်မယ်။ မော်ဒယ်ဖိုင်တွေကတော့ filesize ကြီးလို့ GitHub မှာ တင်ဖို့ အဆင်မပြေလို့ link နဲ့ ရှဲလုပ်ပေးထားပါတယ်။   

**myPOS-V3-Parsed-DP-Data** ဖိုလ်ဒါ ကတော့ myPOS ver. 1.0 ကနေ corpus extension လုပ်စဉ်မှာ သုံးခဲ့တဲ့ ဒေတာဖိုင် တစ်ခုချင်းစီရဲ့ UDTree parsing လုပ်ထားပြီးသား၊ manual လည်း စစ်ထားတဲ့ ဖိုင်တွေ ရှိပါလိမ့်မယ်။ ဒီဖိုလ်ဒါက တကယ်က user တွေအတွက်ဆိုတာထက် နောက်ပိုင်း ဆက်လုပ်မယ့် experiment တွေအတွက် reference အဖြစ် သိမ်းထားတာပါ။   

**myUDTree-ver1.0** ဖိုလ်ဒါ အောက်မှာတော့ myUDTree version 1.0 ဒေတာဖိုင်ကို CoNLL-standard format နဲ့ သိမ်းပေးထားပါတယ်။  

**pic** ဖိုလ်ဒါကတော့ အခု ဖတ်နေတဲ့ README ဖိုင်အတွက် ဥပမာအဖြည့် ထည့်ထားတဲ့ UDTree graph ပုံတွေကို သိမ်းထားတဲ့ ဖိုလ်ဒါပါ။  

## Versions Information

On 11 November 2022 we released myUDTree corpus (version 1.0).   

## Citation

If you want to use myUDTree JPTDP models or myUDTree corpus in your research and we'd appreciate if you use the following reference:  

Zar Zar Hlaing, Ye Kyaw Thu, Thepchai Supnithi and Ponrudee Netisopakul, "Graph-based Dependency Parser Building for Myanmar Language", In Proceedings of the 17th International Joint Symposium on Artificial Intelligence and Natural Language Processing (iSAI-NLP 2022), Nov 5 to 7, 2022, Chiang Mai, Thailand, pp. 1-6. [to appear], [[Slide]](https://github.com/ye-kyaw-thu/papers/blob/master/iSAI-NLP2022/9510_Graph-basedDependencyParserBuildingforMyanmarLanguage.pdf)  

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

9. DyNet Framework:  
https://dynet.readthedocs.io/en/latest/python.html

10. Converter from .conllu format to .conll format for Universal Dependencies:  
https://github.com/diegotxegp/conllu-to-conll


## To Do

- Recheck myUDTree ver.1  
- Active learning and Manual UDTree tagging for myUDTree corpus extension  
- DTree parsing experiments for Myanmar language





