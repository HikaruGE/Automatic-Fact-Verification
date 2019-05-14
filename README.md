# Automatic-Fact-Verification
COMP90042 Project 2019

## 文档筛选
    对于claim的处理：
        1.用AllenNLP的NER模型，标注出所有的entity。
        2.用AllenNLP的Constituency Parsing模型，实现了：
            （1）名词短语（NP）的识别
            （2）对属性为‘S’的节点找出其主语，可能是潜在的entity
            （3）去除了找出来的NP的stopwords

    对于wiki的处理：
        0.预处理：lemma，lower，去stopwords
        1.根据wiki的内容做index
        2.根据wiki的标题做index

## 证据过滤模型 
    idea1:用tfidf做特征向量
    idea2:用pre-trained词向量

    模型：SVM（捞），ESIM

    Todo

## 证据声明关系模型
    Todo