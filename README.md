# Automated Redpill Loader (i18n)

本库为 arpl i18n (多语言优化版): 

### 原版：
<b>https://github.com/fbelavenuto/arpl</b>
* [arpl说明](https://github.com/fbelavenuto/arpl/blob/main/README.md)

### 汉化：
<b>https://github.com/wjz304/arpl-zh_CN</b>
* 仅同步汉化原版, 所以功能与原版保持一致.

### i18n: 
<b>https://github.com/wjz304/arpl-i18n</b>
* addons: https://github.com/wjz304/arpl-addons
* modules: https://github.com/wjz304/arpl-modules
* rp-lkms: https://github.com/wjz304/redpill-lkm

## 说明 - Instructions
* [GUIDE](./guide.md)
 

## 翻译 - Translation
* 其他语言的翻译 - Language translation work:
    ```shell
    # If it does not involve adding or deleting, the following process is not required.
    sudo apt install gettext
    git clone https://github.com/wjz304/arpl-i18n.git
    cd arpl-i18n/files/board/arpl/overlayfs/opt/arpl
    xgettext -L Shell --keyword=TEXT *.sh -o lang/arpl.pot
    sed -i 's/charset=CHARSET/charset=UTF-8/' lang/arpl.pot
    # You need to replace the language you need and translate the po file.
    msginit -i lang/arpl.pot -l zh_CN.UTF-8 -o lang/zh_CN.po
    # This process will be automatically processed during packaging.
    msgfmt lang/zh_CN.po -o lang/zh_CN.mo
    ```
* I am not proficient in the language, and even my English is very poor. 
  Developers who are familiar with various languages are welcome to submit PR.


## 教程 - Usage 
* 中文: https://www.bilibili.com/video/BV1jk4y1Y7B7  
    ##### `(From: http://mi-d.cn)`
* English: https://www.youtube.com/watch?v=mmwKCOiHGWA
    ##### `(From: @markstar6449)`


## 打赏一下
* > ### 作者: Ing  
* > QQ群: 21609194 [点击链接加入QQ群](https://qm.qq.com/cgi-bin/qm/qr?k=z5O89os88QEKXCbz-0gwtEz1AeQiCwk3)
* > QQ频道: redpill2syno [点击链接加入QQ频道](https://pd.qq.com/s/5nmli9qgn)
* > TG频道: redpill2syno [点击链接加入TG频道](https://t.me/redpill2syno)
* <img src="https://raw.githubusercontent.com/wjz304/wjz304/master/my/20220908134226.jpg" width="400">



