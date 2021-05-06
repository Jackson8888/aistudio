# 飞桨常规赛：中文场景文字识别-4月第2名方案

## 项目描述
代码主体用是是PaddleOCR的代码，基于此框架和里面的pre train模型以比赛数据进行finetune得到的结果

## 使用方式
训练模型代码为：

python3 tools/train.py -c configs/rec/rec_r34_vd_none_bilstm_ctc.yml

预测模型代码为：

python3 tools/infer_rec.py -c configs/rec/rec_r34_vd_none_bilstm_ctc.yml -o Global.checkpoints=output/rec_CRNN_aug_341/best_accuracy 
