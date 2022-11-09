# myUDTree
Universal Dependency Tree for Myanmar Language

We are developing UDTree for Myanmar language and plan to release here after we published our paper. Please wait.

y
29 Aug 2022

## Introduction in English
	
The myUDTree corpus is a Universal Dependency (UD) Corpus that extends the Myanmar UD Corpus (Hnin Thu Zar Aye et al.,2018) including 11,000 sentences of Dependency Tree Data. The extended myUDTree UD Corpus contains 43,196 sentences in total. Universal Dependencies (UD) Corpus is a type of Corpus that is annotated according to the Grammar Rule of the respective languages with Part-of-Speech, Morphological Features, and Syntactic Dependencies. Before building myUDTree, we built a Dependency Parsing Model, a Joint POS Tagging and Graph-based Dependency Parsing (jPTDP) model, using the existing Myanmar UD corpus in order to parse Raw Data with Dependency Information. After building the jPTDP model, we selected 20,000 Myanmar sentences from our developing parallel corpora (i.e., Myanmar-Chinese and Myanmar-Korean), and 12,000 Myanmar sentences from the ASEN MT Corpus built by NECTEC Research Center in Thailand, and these data are parsed by using our built jPTDP model to obtain dependency-tree data. The parsed data were manually checked and corrected using the CoNLL-U Viewer tool. After that, the revised data and the original Myanmar UD corpus were integrated to obtain the myUDTree corpus which contains 43,169 sentences with dependency information. Fourteen (14) Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) and 14 dependency relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) are applied in the original version of Myanmar UD Corpus, and CoNLL-U format is used as a dependency-tree data format. The same number of Universal Part-of-Speech tags and Dependency Relations were also applied in our extended myUDTree corpus. The following dependency relations are the most primarily utilized in Myanmar Dependency Structure.
  
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

myUDTree ရဲ့ Corpus Information ကတော့ အောက်ပါအတိုင်းဖြစ်ပါတယ်။

Table 1 Corpus information of myUDTree  

|Unit|myPOS (ver. 1.0)|Ext-1: my-zh|	Ext-2: my-ko|	Ext-3: ASEAN-MT my| myUDTree|
|Sentences	|11,000	|10,000	|10,052	|12,144	|43,196|
|Words	| 239,598 | 103,909 | 106,864 | 114,134 | 564,505|
|Average Words/Sentence	| 21.78| 10.17|	10.64| 9.40| 	13.07|


## မိတ်ဆက် (Intoduction in Myanmar Language)

myUDTree corpus ဟာ ဆိုရင် Author Hnin Thu Zar Aye et al. (2018) တည်ဆောက်ခဲ့တဲ့ စာကြောင်းရေ ၁၁,၀၀၀ ကို Dependency Tree Data ဖြင့် ဖွဲ့စည်းထားသော Myanmar Universal Dependency (UD) Corpus ကို Extend လုပ်ထားတဲ့ UD Corpus တစ်ခု ဖြစ်ပါတယ်။ Extend လုပ်ထားတဲ့ Myanmar UD Corpus မှာဆိုရင် ဒေတာ စုစုပေါင်းအရေအတွက်အားဖြင့် ၄၃,၁၉၆ ပါဝင်ပါတယ်။ Universal Dependencies (UD) Corpusဆိုသည်မှာ Part-of-Speech ၊ Mophological Features များ နှင့် Syntatic Dependencies များဖြင့် သက်ဆိုင်ရာ ဘာသာစကားများရဲ့ Grammar Rule အရ Annotated လုပ်ထားတဲ့ Corpus အမျိုးအစားဖြစ်ပါတယ်။ myUDTree ကို မတည်ဆောက်ခင်မှာ Dependency Information များဖြင့် Raw Data များကို Parsed လုပ်နိုင်ရန်အတွက် မူလရှိပြီးသား Myanmar UD corpus အသုံးပြု၍ Dependnecy Parsing Model တစ်ခုဖြစ်တဲ့ Joint POS Tagging and Graph-based Dependency Parsing (jPTDP) မော်ဒယ် ကို တည်ဆောက်ခဲ့ပါတယ်။ 

jPTDP မော်ဒယ်ကို တည်ဆောက်ပြီးတဲ့နောက်မှာ လက်ရှိမှာ ပြင်ဆင်နေသာ Parallel Corpora ( i.e. Myanmar-Chinese and Myanmar-Korean) မှ Myanmar Raw Dataစာကြောင်းရေ ၂၀,၀၀၀ နှင့် ထိုင်းနိုင်ငံ NECTEC Research Centerမှ တည်ဆောက်ထားသော ASEN MT Corpus မှ Myanmar Raw Dataစာကြောင်းရေ ၁၂,၀၀၀ တို့ကို jPTDP မော်ဒယ်ကို အသုံးပြု၍ Dependency Tree Data များရရှိရန်အတွက် Raw Data များကို Parsed လုပ်ခဲ့ပါတယ်။ Parsed လုပ်ထားသော ဒေတာများကို CoNLL-U Viewer tool ကို အသုံးပြုပြီး manual အားဖြင့် စစ်ဆေးပြီးပြင်ဆင်ထားပါတယ်။ အဲ့ဒီနောက်မှာ စစ်ဆေးပြင်ဆင်ထားသော Dependency Tree Data များနှင့် မူလရှိပြီးသား Myanmar UD Corpusတို့ကို ပေါင်းစပ်ထားပြီး စာကြောင်းရေ အရေအတွက် ၄၃,၁၆၉ နှင့် Dependency Information များ ပါဝင်သော myUDTree Corpus ကို ဖွဲ့စည်းထားပါတယ်။

Original Version ဖြစ်သော Myanmar UD Corpus မှာ 14 Universal Part-of-Speech tags (i.e., ADJ, ADP, ADV, CCONJ, INTJ, NOUN, NUM, PART, PRON, PROPN, PUNCT, SCONJ, SYM, and VERB) နှင့် 14 Dependency Relations (i.e., acl, advmod, amod, aux, case, compound, dep, iobj, mark, nmod, nsubj, nummod, obj, obl, and punct) တို့ကို apply လုပ်ထားပြီး Dependency Tree Data Format အနေဖြင့် CoNLL-U Formt ကို အသုံးပြုထားပါတယ်။ ထိုနည်းတူ Extend လုပ်ထားတဲ့ myUDTree မှာလည်း ၎င်းနှင့် တူညီသော Universal Part-of-Speech tags နှင့် Dependency Relations ကို အသုံးပြုထားပါတယ်။

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

Table 2 Comparison of accuracy values between dependency parsing models
Models	Original myPOS	Extended myPOS Version 3.0
	UAS	LAS	UAS	LAS
jPTDP	85.07%	81.38%	86.16%	82.77%
UniParse	85.67%	82.72%	86.27%	83.36%


Note: jPTDT Model က Raw Text Data ကို Parsed လုပ်ပေးနိုင်သော်လည်း UniParse Model ဟာဆိုရင်ဖြင့် Raw Text Data များကို Parsed မလုပ်ပေးနိုင်ပါ။ 


## Citation

Zar Zar Hlaing, Ye Kyaw Thu, Thepchai Supnithi and Ponrudee Netisopakul, "Graph-based Dependency Parser Building for Myanmar Language", In Proceedings of the 17th International Joint Symposium on Artificial Intelligence and Natural Language Processing (iSAI-NLP 2022), Nov 5 to 7, 2022, Chiang Mai, Thailand, pp. xx-xx. [to appear], [[Slide]](https://github.com/ye-kyaw-thu/papers/blob/master/iSAI-NLP2022/9510_Graph-basedDependencyParserBuildingforMyanmarLanguage.pdf)  
