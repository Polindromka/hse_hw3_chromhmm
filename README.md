# hse_hw3_chromhmm

## Ссылка на colab
```
https://colab.research.google.com/drive/1c_MOk_jdAnOwvdAWKguHrsQt1ANK2dNW?usp=sharing
```
## Гистоновые метки

Name | File
| --- | --- 
H3k36me3StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k36me3StdAlnRep1.bam
H3k9acStdAlnRep1 | wgEncodeBroadHistoneHuvecH3k9acStdAlnRep1.bam
H3k4me2StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k4me2StdAlnRep1.bam
H3k27me3StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k27me3StdAlnRep1.bam
H4k20me1StdAlnRep1 | wgEncodeBroadHistoneHuvecH4k20me1StdAlnRep1.bam
H3k4me3StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k4me3StdAlnRep1.bam
CtcfStdAlnRep1 | wgEncodeBroadHistoneHuvecCtcfStdAlnRep1.bam
H3k27acStdAlnRep1 | wgEncodeBroadHistoneHuvecH3k27acStdAlnRep1.bam
H3k9me1StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k9me1StdAlnRep1.bam
Pol2bStdAlnRep1 | wgEncodeBroadHistoneHuvecPol2bStdAlnRep1.bam
H3k4me1StdAlnRep1 | wgEncodeBroadHistoneHuvecH3k4me1StdAlnRep1.bam
H2azAlnRep1 | wgEncodeBroadHistoneHuvecH2azAlnRep1.bam
H3k79me2AlnRep1 | wgEncodeBroadHistoneHuvecH3k79me2AlnRep1.bam
H3k09me3AlnRep1 | wgEncodeBroadHistoneHuvecH3k09me3AlnRep1.bam
Ezh239875AlnRep1 | wgEncodeBroadHistoneHuvecEzh239875AlnRep1.bam
ControlStdAlnRep1 | wgEncodeBroadHistoneHuvecControlStdAlnRep1.bam

## cellmarkfiletable.txt

Клеточная линия | Гистоновая метка | Файл с гистоновой меткой | Файл с контролем
| --- | --- | --- | ---
Huvec|CtcfStdAlnRep1|CtcfStdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|Ezh239875AlnRep1|Ezh239875AlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H2azAlnRep1|H2azAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k09me3AlnRep1|H3k09me3AlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k4me1StdAlnRep1|H3k4me1StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k4me2StdAlnRep1|H3k4me2StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k4me3StdAlnRep1|H3k4me3StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k9acStdAlnRep1|H3k9acStdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k9me1StdAlnRep1|H3k9me1StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k27acStdAlnRep1|H3k27acStdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k27me3StdAlnRep1|H3k27me3StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k36me3StdAlnRep1|H3k36me3StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H3k79me2AlnRep1|H3k79me2AlnRep1.bam|ControlStdAlnRep1.bam
Huvec|H4k20me1StdAlnRep1|H4k20me1StdAlnRep1.bam|ControlStdAlnRep1.bam
Huvec|Pol2bStdAlnRep1|Pol2bStdAlnRep1.bam|ControlStdAlnRep1.bam

## ChromHMM

Emission | Overlap | Transition 
| --- | --- | ---
![Image](/learnData/emissions_15.png) | ![Image](/learnData/Huvec_15_overlap.png) | ![Image](/learnData/transitions_15.png)

RefSeqTSS | RefSeqTES 
| --- | --- 
![Image](/learnData/Huvec_15_RefSeqTSS_neighborhood.png) | ![Image](/learnData/Huvec_15_RefSeqTES_neighborhood.png)

## Эпигенетические типы
> Чтобы увидеть картинку целиком, необходимо нажать на неё -> Download. Картинка откроется в полном размере в новом окне 

№ | Название | Описание | Картинка
| --- | --- | ---| ---
1 |Heterochromatin | <ul><li>Заметим, что 1-е состояние нпочти не встречается среди выбранных нами гистоновых модификациях, кроме H3k09me3AlnRep1. </li><li>Чаще всего ассоциировано с ядерной ламиной, то есть попаает на участок репрессированного гетерохроматима.</li><li>Данное состояние попадает на интрон гена </li><li>Показывает низкий сигнал.</li><li>Из примерного списка состояний ближе всего к состоянию Heterochromatin</li></ul>| ![Image](/images/image_1.png)
2 | Repressed | <ul><li>Заметим, что 2-е состояние наиболее примерно с равной вероятностью встречается на всех гистоновых модификациях, но чаще всего: <ul><li>H3k09me3AlnRep1  </li><li> H3k36me3StdAlnRep1  </li></ul> </li><li> Данное состояние чаще всего ассоциировано с RefSeqExon и RefSeqTSS.</li><li>Данное состояние нe попало на ген</li><li>Показывает чащего всего высокий сигнал.</li><li>Данное состояние больше всехо похоже на Repressed</li></ul>| ![Image](/images/image_2.png)
3 | Transcribed | <ul><li>Заметим, что 3-е состояние почти не встречается среди выбранных нами гистоновых модификациях, кроме H3k36me3StdAlnRep1. </li><li>Чаще всего ассоциировано с RefSeqGen, RefSeqExon, RefSeqTES.</li><li>Данное состояние попадает на интрон гена </li><li>Показывает низкий сигнал.</li><li>Можем предположить, что это транскрибируемый участок гена, так как имеет очень низкую активность, но попадает на ген.</li></ul>| ![Image](/images/image_3.png)
4 | Transcribed | <ul><li>Заметим, что 4-е состояние почти не встречается среди выбранных нами гистоновых модификациях. </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние попадает на интрон гена </li><li>Показывает низкий сигнал.</li><li>Можем предположить, что это транскрибируемый участок гена, так как имеет очень низкую активность, но попадает на ген.</li></ul>| ![Image](/images/image_4.png)
5 | Heterochromatin | <ul><li>Заметим, что 5-е состояние наиболее часто встречаемое в геноме. </li><li>Чаще всего ассоциировано с ядерной ламиной, то есть попаает на участок репрессированного гетерохроматима.</li><li>Данное состояние попадает на интрон гена </li><li>Показывает низкий сигнал.</li><li>Из примерного списка состояний ближе всего к состоянию Heterochromatin</li></ul>| ![Image](/images/image_5.png)
6 |Repressed | <ul><li>Заметим, что 6-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k27acStdAlnRep1  </li><li> Ezh239875AlnRep1  </li></ul> </li><li> Данное состояние примерно с равной вероятностью встречается на всём геноме, немного чаще ассоциирован с RefSeqTss.</li><li>Данное состояние нe попало на ген или попала на интрон и экзон</li><li>Показывает низкий сигнал.</li><li>Данное состояние больше всехо похоже на Repressed</li></ul>| ![Image](/images/image_6_1.png)
7 | Repressed | <ul><li>Заметим, что 7-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k27acStdAlnRep1  </li><li> Ezh239875AlnRep1  </li></ul> </li><li> Данное состояние примерно с равной вероятностью встречается на всём геноме, немного чаще ассоциирован с ядерной ламиной.</li><li>Данное состояние нe попало на ген или попала на интрон и экзон</li><li>В среднем показывает низкий сигнал.</li><li>Данное состояние больше всехо похоже на Repressed</li></ul>| ![Image](/images/image_7.png)
8 | Enhancer | <ul><li>Заметим, что 8-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>CtcfStdAlnRep1  </li><li> H2azAlnRep1  </li><li> Ezh239875AlnRep1  </li></ul> </li><li> Данное состояние примерно с равной вероятностью встречается на всём геноме.</li><li>Данное состояние попадает на интрон</li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всехо похоже на Enhancer</li></ul>| ![Image](/images/image_8.png)
9 | Promoter | <ul><li>Заметим, что 9-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H2azAlnRep1  </li><li> H3k4me3StdAlnRep1  </li><li> H3k9acStdAlnRep1  </li><li> H3k4me2StdAlnRep1 </li><li>  H3k27acStdAlnRep1 </li><li>H3k4me1StdAlnRep1</li></ul> </li><li>Чаще всего ассоциировано с CpGIslands, RefSeqExon, RefSeqTSS2kb и с ядерной ламиной.</li><li>Данное состояние попадает на экзон </li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всего похоже на Promoter</li></ul>| ![Image](/images/image_9.png)
10 | Enhancer | <ul><li>Заметим, что 10-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H2azAlnRep1  </li><li> H3k4me3StdAlnRep1  </li><li> H3k9acStdAlnRep1  </li><li> H3k4me2StdAlnRep1 </li><li>  H3k27acStdAlnRep1 </li><li> Pol2bStdAlnRep1 </li><li> H3k4me1StdAlnRep1</li><li>  H3k79me2AlnRep1 </li></ul> </li><li>Чаще всего ассоциировано с CpGIslands, RefSeqExon, RefSeqTSS2kb. Но совершенно не ассоциирован с ядерной ламиной.</li><li>Данное состояние частично попадает на экзон и интрон</li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всего похоже на Enhancer</li></ul>| ![Image](/images/image_10.png)
11 | Enhancer | <ul><li>Заметим, что 11-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k9acStdAlnRep1  </li><li> H3k4me2StdAlnRep1  </li><li> H3k27acStdAlnRep1  </li><li> H3k79me2AlnRep1 </li></ul> </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние частично попадает на экзон и интрон</li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всехо похоже на Enhancer</li></ul>| ![Image](/images/image_11.png)
12 | Enhancer | <ul><li>Заметим, что 12-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k27acStdAlnRep1  </li><li> H3k4me1StdAlnRep1  </li></ul> </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние попадает на интрон</li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всего похоже на Enhancer, как и состояние 11</li></ul>| ![Image](/images/image_12.png)
13 |Enhancer | <ul><li>Заметим, что 13-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k4me1StdAlnRep1 </li></ul> </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние попадает на интрон</li><li>Показывает не очень высокий сигнал сигнал.</li><li>Данное состояние больше всего похоже на Enhancer, как и состояние 11 и 12</li></ul>| ![Image](/images/image_13.png)
14 |Enhancer | <ul><li>Заметим, что 14-е состояние наиболее часто встречается на гистоновых модификациях: <ul><li>H3k4me2StdAlnRep1  </li><li> H3k4me1StdAlnRep1  </li><li> H3k79me2AlnRep1 </li></ul> </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние попадает на интрон</li><li>Показывает высокий сигнал.</li><li>Данное состояние больше всехо похоже на Enhancer</li></ul>| ![Image](/images/image_14.png)
15 | Transcribed | <ul><li>Заметим, что 15-е состояние почти не встречается среди выбранных нами гистоновых модификациях, кроме H3k79me2AlnRep1. </li><li>Чаще всего ассоциировано с RefSeqGen.</li><li>Данное состояние попадает на интрон гена </li><li>Показывает очень низкий сигнал.</li><li>Можем предположить, что это транскрибируемый участок гена, так как имеет очень низкую активность, но попадает на ген.</li></ul>| ![Image](/images/image_15.png) 

