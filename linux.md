# pcapxray-install

Linux, Windows, MaxOS 中，安裝與使用 [Srinivas11789/PcapXray](https://github.com/Srinivas11789/PcapXray)

### Kali-Linux
1. git clone 或直接下載 zip - [Srinivas11789/PcapXray](https://github.com/Srinivas11789/PcapXray)

2. 安裝 [`Python3.7.XXX`](https://www.python.org/downloads/release/python-375/)
```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install python3.7
```
> 請注意，該工具不支援 Python 3.8 版本 <br>
> 需要先更新 package list 確保 apt 安裝的套件是較新的

3. 使用 `apt` 安裝 `pip3`
```
  sudo apt-get install python3-pip
```

4. 使用 `apt` 安裝 `tk`
``` 
  sudo apt-get install python3-tk
```

5. 使用 `apt` 安裝 `graphviz`
```
  sudo apt-get install graphviz
```

6. 使用 `apt` 安裝 `Pillow`
```
  sudo apt-get install python3-pil python3-pil.imagetk
```

7. 使用 `pip3` 安裝其他所需的套件
```
pip3 install -r requirements.txt
```

8. 切換工作路徑至 `PcapXray`底下，執行 `./Source/main.py`
```
python3 ./Source/main.py 
```

> 部分使用者電腦中有多個版本的 `python` <br>
> 可利用 `whereis -b [name]` 或是 `which [name]` 來找到 `python` 的執行檔位置
> ![img](https://i.imgur.com/sUL61oe.png)
> 可以使用 `sudo update-alternatives` 相關指令註冊並切換不同 `python` 版本
> ```
> # 可用上述的 whereis 或 which 指令找到 python3 執行路徑，優先權為必填填入整數即可
> sudo update-alternatives --install python3 [python3 執行路徑] [優先權]
>
> # 設定 python3 指令要執行哪個版本，請注意是選擇選項編號而不是優先權的號碼，如下圖
> sudo update-alternatives --config python3
> ```
> ![img](https://i.imgur.com/GFXERu7.png)

9. 選擇輸入 `.pcap` 檔案路徑

10. 選擇輸出分析報告路徑

11. 按下 `Analyze!`，開始分析

12. 按下 `Visualize!`，繪製分析結果
![img](https://i.imgur.com/ek0luCA.png)
![img](https://i.imgur.com/eMP57wy.png)
