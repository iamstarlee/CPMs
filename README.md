# CPMs
2D人体关键点检测

# 数据集下载
http://sam.johnson.io/research/lsp.html
and
http://sam.johnson.io/research/lspet.html

数据集文件夹的结构
data
└── LSP
    ├── lsp_dataset
    │   ├── images
    │   └── visualized
    └── lspet_dataset
        └── images
        
# 训练
## With weighted loss
python -W ignore::UserWarning cpm_train.py --lsp-root ./data/LSP --ckpt-dir ./model  --summary-dir ./summary --cuda

## Without weighted loss
python -W ignore::UserWarning cpm_train.py --lsp-root ./data/LSP --ckpt-dir ./model  --summary-dir ./summary --cuda --wl

