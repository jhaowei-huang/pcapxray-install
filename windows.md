# pcapxray-install

Linux, Windows, MaxOS 中，安裝與使用 [Srinivas11789/PcapXray](https://github.com/Srinivas11789/PcapXray)

### Windows
1. git clone 或直接下載 zip - [Srinivas11789/PcapXray](https://github.com/Srinivas11789/PcapXray)

1. 下載安裝 [`Python3.7.7`](https://www.python.org/downloads/release/python-377/)

> 請注意，該工具不支援 Python 3.8 版本 <br>
> 建議使用 [`Python3.7.7 - Windows x86-64 executable installer`](https://www.python.org/ftp/python/3.7.7/python-3.7.7-amd64.exe)
![img](https://i.imgur.com/vNUSUlf.png)

> 請勾選 `Python add to PATH` 選擇 `Customize installation` <br>
![img](https://i.imgur.com/0bZ9CQP.png)
> 請勾選 `安裝 pip` 與 `安裝 td/tk and IDLE` <br>
![img](https://i.imgur.com/kED27ZE.png)
> 可自行修改安裝路徑，其他安裝選項建議參照下圖 <br>
![img](https://i.imgur.com/oX3jkhl.png)

2. 安裝 [`graphviz`](https://graphviz.gitlab.io/_pages/Download/Download_windows.html)

> 版本為 `graphviz - 2.38 Stable Release` <br>
> 請確定 `[安裝路徑]\graphviz\bin` 有被加入系統環境變數 `PATH`
![img](https://i.imgur.com/lts1tb0.png)


3. 使用 `pip3` 安裝 `tk`

```
pip3 install tk
```

4. 使用 `pip3` 安裝 `Pillow`

```
pip3 install Pillow
```

5. 使用 `pip3` 安裝其他所需的套件 (若發生錯誤，請嘗試以`管理員身分`開啟 PowerShell 再執行一次指令)

```
pip3 install -r requirements.txt
```

6. 切換工作路徑至 `PcapXray`底下，執行 `.\Source\main.py`

```
python .\Source\main.py 

or

python3 .\Source\main.py
```

> 部分使用者電腦中有多個版本的 `python` <br>
> 分為 `python` 與 `python3` (通常 python 指的是 2.7.XXX 版本) <br>
> 請利用 `python --version` 或是 `python3 --version` <br>
> 確認哪個執行的版本為 `3.7.XXX`，就以該指令啟動 `.\Source\main.py` <br>

7. 選擇輸入 `.pcap` 檔案路徑

8. 選擇輸出分析報告路徑

> 因為 Windows 的路徑是以`\`表示 <br>
> 建議要手動選擇輸出輸出路徑，以免程式解析錯誤

9. 按下 `Analyze!`，開始分析

10. 按下 `Visualize!`，繪製分析結果
![img](https://i.imgur.com/n9g44so.png)

### 備註

分析的圖片可以直接去輸出路徑查看，程式會在輸出路徑產生 `Report` 資料夾

![img](https://i.imgur.com/i7fp5WJ.png)
![img](https://i.imgur.com/jCj7WoK.png)
