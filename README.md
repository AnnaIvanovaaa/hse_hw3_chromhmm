# Colab

[сcылка](https://colab.research.google.com/drive/1QdDGWlpane_IRf07NQUy-H1zGAGMYz9S?usp=sharing)

# Модификации гистонов
#### Тип клетки: NHEK
##### Контроль: Control.bam (NhekControlStdAlnRep1.bam)
| Модификация      | .bam файл       |
| ------------- |------------------:|
| [H2az](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH2azAlnRep1.bam)     | H2az.bam    |
| [H3k27ac](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k27acStdAlnRep1.bam)     | H3k27ac.bam |
| [H3k27me3](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k27me3StdAlnRep1.bam)  | H3k27me3.bam         |
| [H3k36me3]( http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k36me3StdAlnRep1.bam) | H3k36me3.bam  |
| [Ctcf](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekCtcfStdAlnRep1.bam)     | Ctcf.bam    |
| [Pol2b](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekPol2bStdAlnRep1.bam)     | Pol2b.bam |
| [H4k20me1](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH4k20me1StdAlnRep1.bam)  | H4k20me1.bam         |
| [H3k79me2](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k79me2AlnRep1.bam) | H3k79me2.bam |
| [H3k9ac](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k9acStdAlnRep1.bam)  | H3k9ac.bam         |
| [H3k9me1](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneNhekH3k9me1StdAlnRep1.bam) | H3k9me1.bam |


# ChromHMM
### Emissions
![emissions_10](https://user-images.githubusercontent.com/93247992/160437901-b12b2e1b-b493-4737-b769-b2e2fb976939.png)


### Transitions
![transitions_10](https://user-images.githubusercontent.com/93247992/160437923-a8bd3786-8519-4295-b88f-7998093f7814.png)

### Fold  Enrichment
![NHEK_10_overlap](https://user-images.githubusercontent.com/93247992/160494250-1cdb7aaf-5fe6-4bc1-9c5c-000cbac306d8.png)

#### State 1
![Снимок экрана (217)](https://user-images.githubusercontent.com/93247992/160592623-ba50c656-02e6-4c16-a525-137b6e38bd04.png)
![Снимок экрана (224)](https://user-images.githubusercontent.com/93247992/160594442-15ceadf9-cd19-4745-9eb7-99630ae641cc.png)
Слабые сигналы, есть небольшие пики на метке H3K27m3.

#### State 2
![Снимок экрана (218)](https://user-images.githubusercontent.com/93247992/160589977-94de6dd5-4d2e-4cc6-bd70-ac4fc839adb5.png)
![Снимок экрана (219)](https://user-images.githubusercontent.com/93247992/160590008-15170b57-cbda-4f77-9dc7-244cfc204d9a.png)
Слабый сигнал практически на всех гистоновых метках, иногда появляются средние пики на H2A.Z. 

#### State 3
![Снимок экрана (220)](https://user-images.githubusercontent.com/93247992/160592713-cbea5645-0e44-4c6e-ba04-3769c650e3a9.png)
Сигналы практически отсутсвуют, нет значимых пиков. Состояние не характерно ни для одной метки.

#### State 4
![Снимок экрана (216)](https://user-images.githubusercontent.com/93247992/160586507-de099d9b-e738-49c3-b0f1-51184fcf0100.png)
![Снимок экрана (212)](https://user-images.githubusercontent.com/93247992/160586525-78b3907c-839b-4fcb-ba85-52bce21e7e75.png)
Для данного состояния характерна гистоновая метка CTCF. Это можно сказать по явным пикам, следовательно, данные области являются стат. значимые обогащения сигнала (significant signal enrichment). 

#### State 5
![Снимок экрана (214)](https://user-images.githubusercontent.com/93247992/160592288-aa35c20e-e20d-4a19-8c23-a3e84da63306.png)
![Снимок экрана (215)](https://user-images.githubusercontent.com/93247992/160592327-c71bf3ed-6849-4f69-bf77-d76e7eb8960e.png)
Сигнал очень слабый, есть небольшие пики на H2A.Z.

#### State 6
![Снимок экрана (210)](https://user-images.githubusercontent.com/93247992/160591576-460b1c62-e109-4646-bc1b-602e376674a4.png)
![Снимок экрана (213)](https://user-images.githubusercontent.com/93247992/160591607-ec89899b-4f7f-40fb-a182-109ba6ad4723.png)
Слабый сигнал практически на всех метках, кроме H2A.Z, H3K9ac, H3K27ac - высокая плотность. Pol2 тоже характерен для данного состояния, по пик значительно ниже, чем для приведенных ранее меток.

#### State 7
![Снимок экрана (209)](https://user-images.githubusercontent.com/93247992/160590630-2488e4ef-e5db-43e6-85d8-1ac46dad5770.png)
![Снимок экрана (211)](https://user-images.githubusercontent.com/93247992/160590662-a297824b-b140-4d0a-a1da-9ddf24091605.png)
Характерные гистоновые метки: H3K9ac, H3K27ac, H3K79m2. По скриншотам видно, что среднее значение сигнала по интервалу высокое. 

#### State 8
![Снимок экрана (221)](https://user-images.githubusercontent.com/93247992/160592833-c36f6eb1-be11-4595-9468-7b1531bb0959.png)
Очень сильные сигналы только на метке H3K79m2.

#### State 9
![Снимок экрана (222)](https://user-images.githubusercontent.com/93247992/160593047-640d55fc-fa8e-4e04-b3e4-f1767e73fd7a.png)
Сильный сигнал характерен для метки H3K79m2, на всех остальных он или практически отсутвует, или средний.

#### State 10
![Снимок экрана (223)](https://user-images.githubusercontent.com/93247992/160594165-f3e85d1f-777b-4d79-b417-47f49201b533.png)
Слабый сигнал, состояние не характерно ни для одной гистоновой метки.

| State      | Модификация       | Эпигенетический тип | 
| ------------- |------------------:| ------------|
| 1      | H3K27m3       | poised Promoter |
| 2 | H2A.Z |  Heterochromatin |
| 3      | -      | Heterochromatin |
| 4 | CTCF | Insulator |
| 5      | H2A.Z       | Weak enhancer |
| 6 | H2A.Z, H3K9ac, H3K27ac, Pol2 | Active Promoter |
| 7      | H3K9ac, H3K27ac, H3K79m2 |  Strong enhancer |
| 8 | H3K79m2 | Weak transcribed |
| 9      | H3K79m2       | Transcriptional elongation |
| 10 | - |  Transcriptional elongation\Weak transcribed |

# Дополнительное задание
