# 抖音直播弹幕爬取 python 实现

## 环境

```
python 3.11.4
```

## 运行

```bash
pip install -r requirements.txt
python main.py
```

## 运行效果

```
2023-08-23 17:10:42 [弹幕] 芳***: 你倒点照片呀，[发怒][发怒][发怒]
2023-08-23 17:10:45 [弹幕] 气***: 快点选喽
2023-08-23 17:10:45 [弹幕] 秀***: 1
2023-08-23 17:10:47 [弹幕] 瑄***: 照片，照片，照片，照片，照片，照片。照片，照片，照片，照片，照片。
2023-08-23 17:10:47 [弹幕] 路***: 你要点那个画呀，大哥
2023-08-23 17:10:48 [弹幕] 用***: 22222222222222222222222222222222222222222222222222
2023-08-23 17:10:49 [弹幕] 用***: 3333333333333333
2023-08-23 17:10:49 [弹幕] 禹***: 22
2023-08-23 17:10:50 [弹幕] 彝***: 2222222222
2023-08-23 17:10:51 [弹幕] 秀***: 1
2023-08-23 17:10:53 [弹幕] 用***: 33333333333333
2023-08-23 17:10:54 [弹幕] 用***: 22222222222222222222222222
2023-08-23 17:10:54 [弹幕] 张***: 照片
2023-08-23 17:10:56 [弹幕] 用***: 我画点画，你好罗嗦
2023-08-23 17:10:58 [弹幕] 😊***: 所以你赶紧点床上
2023-08-23 17:10:59 [弹幕] 用***: 22222222222222222222222222
2023-08-23 17:11:00 [弹幕] #***: 烦死人了，怎么还不点照片[发怒][发怒][发怒][发怒]
2023-08-23 17:11:01 [弹幕] 沫***: 外星人。床上的。这回咱们是。
```

## 打包

```bash
## MacOS
pyinstaller -F main.py --add-data "static/*:static/" # 打包成单个文件
pyinstaller main.py --add-data "static/*:static/" # 打包成文件夹

## Windows
pyinstaller -F main.py --add-data "static/*;static/" # 打包成单个文件
pyinstaller main.py --add-data "static/*;static/" # 打包成文件夹
```

## 配置位置（包括URL）

```
static/config_dev.yml 
```

## ENV设置

```bash
export DY_LIVE_ENV="prod" ## 生效配置 config-<DY_LIVE_ENV>.yml
```
