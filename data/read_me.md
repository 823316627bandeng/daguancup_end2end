# ������Ҫ˼�����

1.Ԥѵ��ʹ�õ���albert��ngram mask���������mlm��������һ��structbert���ᵽ��word struct prediction ����������������������ʣ���ģ������ԭ�������ʡ�

2.΢��ʹ�õ���trick��(1).PGD�Կ�ѵ����(2).UDA�е�TSA��(3).�Զ����ģ�ͼܹ���(4).EMA��(5).lookahead.


# ����ȫ����


##### 1.process data


> run data/code/process_data/process_data.py 
> ���л��� �� GPU -> ���� RTX-3090�� CPU -> inter 10700K


##### 2.build vocab


> run data/code/build_vocab/build_vocab.py
> ���л��� �� GPU -> ˫�� RTX-2080�� CPU -> 


##### 3.pretrain


> run data/code/pretrain_code/run_pretrain.py 
> ���л��� �� GPU -> ˫�� RTX-2080�� CPU -> 


##### 4.finetune


> run data/code/finetune_code/run_classify.py 
> ���л��� �� GPU -> ���� RTX-3090�� CPU -> inter 10700K


##### 5.predict


> run data/code/predict_code/run_predictor.py
> ���л��� �� GPU -> ���� RTX-3090�� CPU -> inter 10700K



##### 6.fusion


> run data/code/fusion_code/run_fusion.py
> ���л��� �� GPU -> ���� RTX-3090�� CPU -> inter 10700K
