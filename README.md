# CPMs
2D人体关键点检测

# 数据集下载
http://sam.johnson.io/research/lsp.html
and
http://sam.johnson.io/research/lspet.html

数据集文件夹的结构

![image](https://user-images.githubusercontent.com/44799727/142198604-a379e5cd-c025-4c0e-a9dd-83b9bfc4836c.png)
        
# 训练
## With weighted loss
python -W ignore::UserWarning cpm_train.py --lsp-root ./data/LSP --ckpt-dir ./model  --summary-dir ./summary --cuda

## Without weighted loss
python -W ignore::UserWarning cpm_train.py --lsp-root ./data/LSP --ckpt-dir ./model  --summary-dir ./summary --cuda --wl

